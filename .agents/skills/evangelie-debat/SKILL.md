---
name: evangelie-debat
description: Voer een iteratief, brongebaseerd debat over de datering van het Johannesevangelie (de triangulatie van George/Geurt Henk van Kooten). Twee subagent-opponenten, "Grieks" (pro Van Kooten, vroege Johannes) en "Joods" (late datering, joodse invloed), reageren om de beurt op elkaar via een gedeeld whiteboard met online gezochte bronnen; een neutrale moderator scoort elke ronde -10..+10 tot de score stabiliseert. Gebruik dit wanneer de gebruiker dit debat, een "evangelie-debat", of een dispuut over de datering van Johannes / Van Kooten wil starten.
---

# Orchestrator: evangelie-debat

Jij (de hoofdsessie) bent de **orchestrator**. Je voert zelf geen argumenten aan en bewaart geen
debatinhoud in je eigen context, je **bestuurt de lus** en delegeert al het denkwerk aan drie
subagent-rollen. De rolinstructies staan in losse bestanden:

- Opponent Grieks (pro Van Kooten, vroege Johannes) → `.agents/agents/evangelie-grieks.md`
- Opponent Joods (late datering, joodse invloed) → `.agents/agents/evangelie-joods.md`
- Moderator (neutrale jury: samenvat + scoort + bewaakt convergentie) → `.agents/agents/evangelie-moderator.md`

### Hoe je een rol aanroept (belangrijk)
Spawn elke rol met de **Agent-tool**. Gebruik bij voorkeur `subagent_type` gelijk aan de
agent-naam (`evangelie-grieks` / `evangelie-joods` / `evangelie-moderator`). **Zijn die niet
beschikbaar** (bv. de agents zijn pas aangemaakt en nog niet geladen, je krijgt dan een
"agent type not found"-fout), val dan terug op `subagent_type: general-purpose` en geef in de
prompt het **absolute pad naar het rolbestand** met de instructie: *"Lees eerst dit rolbestand
volledig en handel exact volgens die rol."* De rolbestanden zijn de enige bron van waarheid voor
het gedrag; je hoeft de inhoud niet te dupliceren.

> **Kernmechanisme:** subagents zijn stateless en delen geen geheugen. Het **whiteboard-bestand op
> schijf is het enige gedeelde geheugen.** Elke subagent leest het en appendt eraan. Jij houdt
> alleen de lus-status bij door `state.json` te lezen.

## Parameters (default; mag de gebruiker via args overschrijven, bv. "max 4 rondes")
- `MAX_RONDES = 8`
- `CONV_DREMPEL = 1`  (score-verandering die als "stabiel" telt: |Δ| ≤ 1)
- `CONV_GEDULD = 2`   (aantal opeenvolgende stabiele rondes om te stoppen)

## Stap 1, Setup
0. **Hervatten?** Vroeg de gebruiker een onderbroken run voort te zetten (bv. "hervat de laatste
   run" of een concrete run-naam), zoek dan de run-map (bij "laatste": de nieuwste `debat-output/run-*`),
   lees haar `state.json`, en **sla het aanmaken/kopiëren over**. Hergebruik het bestaande
   `whiteboard.md` en `state.json`, neem `params` en `round` daaruit over, en start de lus in Stap 2
   bij `round + 1` (is `round` al `>= max_rondes` of `stop_reason` gezet, ga direct naar Stap 3).
   Ontbreekt `sources.md` in een oudere run-map, kopieer dan alsnog `templates/sources-template.md`
   ernaartoe (en vul `{{RUN_NAAM}}` in) voordat je de lus start.
   Anders, voor een nieuwe run:
1. Bepaal een run-naam: `run-$(date +%Y%m%d-%H%M%S)`. Maak de map
   `debat-output/<run-naam>/` aan (met Bash `mkdir -p`).
2. Kopieer de templates naar de run-map:
   - `templates/whiteboard-template.md` → `debat-output/<run-naam>/whiteboard.md`
   - `templates/state-template.json` → `debat-output/<run-naam>/state.json`
   - `templates/sources-template.md` → `debat-output/<run-naam>/sources.md`
3. Vul de placeholders `{{RUN_NAAM}}` en `{{DATUM}}` in `whiteboard.md` in, en `{{RUN_NAAM}}` in
   `sources.md` (Edit).
4. Als de gebruiker afwijkende parameters gaf, pas ze aan in `state.json` (`params`-blok) en gebruik
   ze hieronder.
5. Vertel de gebruiker kort dat het debat start en waar de artefacten komen.

## Stap 2, De debatlus
Herhaal voor `ronde = START, START+1, …, MAX_RONDES` (bij een nieuwe run is `START = 1`; bij
hervatten is `START = state.round + 1`):

1. **Openingszijde** (tegen first-mover-bias): oneven ronde → Grieks eerst, dan Joods; even ronde →
   Joods eerst, dan Grieks.
2. **Roep opponent A aan** met de Agent-tool (`subagent_type` = de eerste zijde). Geef in de prompt:
   - het absolute pad naar `whiteboard.md`;
   - het absolute pad naar `sources.md` (de bronnenlog van deze run);
   - de **absolute paden** naar de reference-bestanden `reference/achtergrond.md` en
     `reference/bronnen.md` (de subagent draait mogelijk in een andere werkmap en kan ze anders
     niet vinden);
   - het rondenummer;
   - de instructie: "Lees het hele whiteboard + de reference-bestanden, weerleg de laatste beurt,
     breng ≥1 nieuw geverifieerd argument/bron (uit het open web of uit de commentaar-notebooks
     via de `nlm` CLI, bv. `nlm cross query "..." -n "John - exegesis"`), en append je beurt volgens
     je rolinstructie. Log elke geciteerde bron met volledige herkomst in `sources.md`. Vanaf ronde
     2 mag je nieuwe, creatieve invalshoeken inbrengen. Schrijf natuurlijk Nederlands zonder
     em-dashes of stijltics. Retourneer alleen een korte statusregel."
   **Wacht** tot de subagent klaar is.
3. **Roep opponent B aan** (de andere zijde) op identieke wijze. B ziet nu A's verse beurt op het
   whiteboard. Wacht tot klaar.
4. **Roep de moderator aan** (`evangelie-moderator`). Geef paden naar `whiteboard.md`, `state.json`
   én `sources.md`, het rondenummer, en "Dit is een RONDE-evaluatie." Wacht tot klaar. De moderator
   werkt ook de scorebord-tabel boven in `whiteboard.md` bij.
5. **Lees `state.json`** (Read). Pak het laatste `history`-item (de score + delta van deze ronde).
6. **Stop-condities**, stop de lus als één hiervan geldt:
   - `converged == true` of `stop_reason` gezet (moderator zag volledige capitulatie); **of**
   - de laatste `CONV_GEDULD` rondes hebben elk `|delta| ≤ CONV_DREMPEL` (score is stabiel); **of**
   - de laatste `CONV_GEDULD` rondes hebben elk `new_evidence_grieks == 0` én
     `new_evidence_joods == 0` (beide kanten zijn uitgeput, ook als de score nog wat beweegt); **of**
   - `ronde == MAX_RONDES`.

   Negeer bij de twee stabiliteits-checks ronde 1 (`delta: null` telt **niet** als stabiel);
   evalueer ze pas zodra er minstens `CONV_GEDULD` rondes met een ingevulde `delta` zijn, dus ten
   vroegste vanaf ronde `CONV_GEDULD + 1`.
   Noteer de reden (`concessie` / `stabiele score` / `uitputting` / `max rondes`).
7. Print één regel voortgang aan de gebruiker, bv. `Ronde 3, score −4 (Δ −1)`, en ga door of stop.

Voer de subagents **sequentieel** uit (niet parallel): binnen een ronde moet de tweede opponent de
beurt van de eerste kunnen lezen, en de moderator beide.

## Stap 3, Eindrapport
1. Werk in `state.json` `stop_reason` bij als die nog niet gezet is (Edit).
2. Roep de `evangelie-moderator` aan met "Schrijf het EINDRAPPORT" + paden naar `whiteboard.md`,
   `state.json`, `sources.md` en de run-map. De moderator schrijft `eindrapport.md` en baseert de
   bronnenlijst op `sources.md`.
3. Lees `eindrapport.md` en geef de gebruiker een bondige samenvatting: **eindscore**, stop-reden,
   het scoreverloop in één zin, en de paden naar `whiteboard.md` en `eindrapport.md`.

## Robuustheid
- **Faalt een subagent** of komt hij zonder bruikbare beurt terug, roep hem éénmaal opnieuw aan met
  een expliciete herinnering aan zijn formaat-eisen. Blijft het mislukken (bv. WebSearch
  onbeschikbaar), meld dit aan de gebruiker en stop netjes met een deel-eindrapport.
- **Is `state.json` na de moderator-beurt onleesbaar of ongeldige JSON, of ontbreekt het
  `history`-item voor de huidige ronde**, roep de moderator éénmaal opnieuw aan met de herinnering
  dat hij geldige JSON moet wegschrijven met een `history`-item voor deze ronde. Blijft het stuk,
  meld het aan de gebruiker en stop netjes met een deel-eindrapport op basis van de laatst geldige
  staat. Bewerk `state.json` niet zelf inhoudelijk.
- **Verzin nooit zelf debatinhoud of scores** en bewerk het whiteboard niet inhoudelijk, dat is
  het werk van de subagents. Jij doet alleen setup, lus-besturing, en het lezen van `state.json`.
- Geef de subagents **absolute paden** zodat ze de juiste bestanden vinden, ongeacht hun werkmap.
- Houd je eigen context licht: lees per ronde alleen `state.json`, niet het hele whiteboard.
