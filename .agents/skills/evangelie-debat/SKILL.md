---
name: evangelie-debat
description: Voer een iteratief, brongebaseerd debat over de datering van het Johannesevangelie (de triangulatie van George/Geurt Henk van Kooten). Vier subagent-opponenten debatteren in twee paren, één per as: "Vroeg" tegen "Laat" op de datering-as en "Grieks-Romeins" tegen "Joods" op de karakter-as, via een gedeeld whiteboard met online gezochte bronnen; een neutrale moderator scoort elke ronde op twee onafhankelijke assen (datering vroeg..laat en karakter Grieks-Romeins..Joods, elk -10..+10) tot beide scores stabiliseren. Gebruik dit wanneer de gebruiker dit debat, een "evangelie-debat", of een dispuut over de datering van Johannes / Van Kooten wil starten.
---

# Orchestrator: evangelie-debat

Jij (de hoofdsessie) bent de **orchestrator**. Je voert zelf geen argumenten aan en bewaart geen
debatinhoud in je eigen context, je **bestuurt de lus** en delegeert al het denkwerk aan vijf
subagent-rollen: vier opponenten (twee per as) en een moderator. De rolinstructies staan in losse
bestanden:

- **Datering-as** (vroeg of laat):
  - Opponent Vroeg (vóór 66-70, pro Van Kootens dateringsargumenten) → `.agents/agents/evangelie-vroeg.md`
  - Opponent Laat (post-85) → `.agents/agents/evangelie-laat.md`
- **Karakter-as** (Grieks-Romeins of joods):
  - Opponent Grieks-Romeins (hellenistisch karakter) → `.agents/agents/evangelie-grieks-romeins.md`
  - Opponent Joods (joods karakter) → `.agents/agents/evangelie-joods.md`
- Moderator (neutrale jury: samenvat + scoort op twee assen + bewaakt convergentie) → `.agents/agents/evangelie-moderator.md`

Elke opponent debatteert **strikt op zijn eigen as**: Vroeg en Laat alleen over de datum,
Grieks-Romeins en Joods alleen over het culturele karakter. Zo blijven de twee assen ontkoppeld.

### Hoe je een rol aanroept (belangrijk)
Spawn elke rol met de **Agent-tool**. Gebruik bij voorkeur `subagent_type` gelijk aan de
agent-naam (`evangelie-vroeg` / `evangelie-laat` / `evangelie-grieks-romeins` / `evangelie-joods` /
`evangelie-moderator`). **Zijn die niet beschikbaar** (bv. de agents zijn pas aangemaakt en nog niet
geladen, je krijgt dan een "agent type not found"-fout), val dan terug op `subagent_type:
general-purpose` en geef in de prompt het **absolute pad naar het rolbestand** met de instructie:
*"Lees eerst dit rolbestand volledig en handel exact volgens die rol."* De rolbestanden zijn de enige
bron van waarheid voor het gedrag; je hoeft de inhoud niet te dupliceren.

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
Per ronde komen **vier opponenten** aan het woord (twee per as), daarna de moderator. Binnen een as
debatteren de twee polen tegen elkaar; de twee assen staan los. Herhaal voor
`ronde = START, START+1, …, MAX_RONDES` (bij een nieuwe run is `START = 1`; bij hervatten is
`START = state.round + 1`):

1. **Volgorde van de ronde** (tegen first-mover-bias, wissel per ronde af):
   - **Oneven ronde:** eerst de datering-as (Vroeg, dan Laat), dan de karakter-as (Grieks-Romeins,
     dan Joods).
   - **Even ronde:** eerst de karakter-as (Joods, dan Grieks-Romeins), dan de datering-as (Laat, dan
     Vroeg).
2. **Roep de vier opponenten één voor één aan** met de Agent-tool, in de volgorde van stap 1
   (`subagent_type` = de agent-naam van die opponent). Geef elke opponent in de prompt:
   - het absolute pad naar `whiteboard.md`;
   - het absolute pad naar `sources.md` (de bronnenlog van deze run);
   - de **absolute paden** naar de reference-bestanden `reference/achtergrond.md`,
     `reference/bronnen.md` en `reference/primaire-bronnen.md` (de subagent draait mogelijk in een
     andere werkmap en kan ze anders niet vinden);
   - het **absolute pad naar de `brontekst`-CLI** (`.agents/tools/brontekst`), zodat de opponent
     primaire teksten kan ophalen ongeacht zijn werkmap;
   - het rondenummer;
   - de instructie: "Lees het hele whiteboard + de reference-bestanden, weerleg de laatste beurt van
     je tegenstander op jouw as, breng ≥1 nieuw geverifieerd argument/bron (uit het open web of uit
     de commentaar-notebooks via de `nlm` CLI, bv. `nlm cross query "..." -n "John - exegesis"`), en
     toets toetsbare claims over primaire teksten met de `brontekst`-CLI (zie `primaire-bronnen.md`).
     Append je beurt volgens je rolinstructie onder het juiste as-kopje. Blijf strikt op je eigen as.
     Log elke geciteerde bron met volledige herkomst in `sources.md`. Creatieve, verrassende
     invalshoeken zijn welkom. Schrijf natuurlijk Nederlands zonder em-dashes of stijltics.
     Retourneer alleen een korte statusregel."
   **Wacht** telkens tot de subagent klaar is voordat je de volgende aanroept, zodat elke opponent de
   verse beurten ziet.
3. **Roep de moderator aan** (`evangelie-moderator`). Geef paden naar `whiteboard.md`, `state.json`
   én `sources.md`, het absolute pad naar de `brontekst`-CLI (`.agents/tools/brontekst`) en
   `reference/primaire-bronnen.md`, het rondenummer, en "Dit is een RONDE-evaluatie." Wacht tot klaar.
   De moderator
   scoort de datering-as op grond van Vroeg/Laat en de karakter-as op grond van Grieks-Romeins/Joods,
   en werkt ook de scorebord-tabel boven in `whiteboard.md` bij.
4. **Lees `state.json`** (Read). Pak het laatste `history`-item (beide scores + delta's van deze ronde).
5. **Stop-condities**, stop de lus als één hiervan geldt:
   - `converged == true` of `stop_reason` gezet (moderator zag volledige capitulatie); **of**
   - de laatste `CONV_GEDULD` rondes hebben elk **beide** assen stabiel, dat wil zeggen
     `|delta_datering| ≤ CONV_DREMPEL` **én** `|delta_karakter| ≤ CONV_DREMPEL`; **of**
   - de laatste `CONV_GEDULD` rondes hebben elk **alle vier** tellingen op nul
     (`new_evidence_vroeg`, `new_evidence_laat`, `new_evidence_grieks_romeins`,
     `new_evidence_joods` alle `0`), dus beide assen zijn volledig uitgeput; **of**
   - `ronde == MAX_RONDES`.

   Negeer bij de stabiliteits-check ronde 1 (`delta_datering`/`delta_karakter: null` telt **niet** als
   stabiel); evalueer hem pas zodra er minstens `CONV_GEDULD` rondes met ingevulde delta's zijn, dus
   ten vroegste vanaf ronde `CONV_GEDULD + 1`. Een ronde telt alleen als stabiel als **beide** assen
   binnen de drempel blijven.
   Noteer de reden (`concessie` / `stabiele score` / `uitputting` / `max rondes`).
6. Print één regel voortgang aan de gebruiker, bv. `Ronde 3, datering −4 (Δ −1), karakter +2 (Δ 0)`,
   en ga door of stop.

Voer de subagents **sequentieel** uit (niet parallel): binnen een ronde moet elke opponent de
voorgaande beurten kunnen lezen, en de moderator alle vier.

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
