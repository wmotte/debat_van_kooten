# Evangelie- en Q-debat

Deze repo bevat skills die **iteratieve, brongebaseerde debatten** voeren rond George (Geurt Henk)
van Kootens *Echo's van het goede nieuws: De evangeliën in context, toen en nu* (2025/2026).

Het eerste debat gaat over de datering en het culturele karakter van het Johannesevangelie. Het
tweede debat gaat over **Q**, de hypothetische bron achter de dubbele traditie in Mattheüs en Lucas.

Voor het Johannesdebat debatteren vier subagent-opponenten in **twee paren, één per as**: ze reageren om de beurt op elkaar
via een gedeeld "whiteboard", dragen elke ronde **echte, online gezochte bronnen** aan (ook
grammaticaal en syntactisch), en een **neutrale moderator** scoort de stand van de evidentie op twee
onafhankelijke assen (datering en cultureel karakter). Zodra beide scores stabiliseren, stopt het
debat met een eindrapport.

---

## De vier opponenten (twee per as)

De datering en het culturele karakter zijn twee aparte vragen. Daarom heeft elke as **twee
opponenten**, één per pool, en blijft iedere opponent strikt op zijn eigen as.

| As | Opponent | Standpunt | Kernargumenten |
|---|---|---|---|
| Datering | ⏳ **Vroeg** | Johannes is **vroeg** (vóór 66–70 n.Chr.), mogelijk het oudste evangelie | `estin`-praesens in Joh 5:2 (Betzata); superieure pre-70-topografie; Lukaanse posterioriteit; bron Q overbodig |
| Datering | 🕰️ **Laat** | Johannes is **laat** (post-85 n.Chr.) | praesens historicum is geen dateringsbewijs; `aposynagōgos` / Martyn; externe attestatie (P52); redactielagen (Joh 21) |
| Karakter | 🏛️ **Grieks-Romeins** | Overwegend **Grieks-Romeins** van karakter | genre als antieke biografie (*bios*); Logos-filosofie (Stoa, middenplatonisme); dramatische en retorische vorm; hellenistisch publiek |
| Karakter | ✡️ **Joods** | Overwegend **joods** van karakter | joodse hermeneutiek; Logos met Memra-/wijsheidswortels; feestcyclus; joods-Palestijns milieu (Qumran) |

Van Kootens stelling "vroeg én Grieks-Romeins" is zo geen ingebouwde aanname meer, maar het resultaat
als Vroeg én Grieks-Romeins beiden overtuigen. Sams tegenvoorbeeld "laat én Grieks-Romeins" (via de
Parting of the Ways) is nu een apart scoorbaar kwadrant.

Alle opponenten zoeken **echte bronnen** op het open web en raadplegen daarnaast ingelezen
**commentaar-notebooks** per bijbelboek (`John - exegesis`, `Luke - exegesis`, `Matthew - exegesis`,
`Mark - exegesis`, en meer) via de **`nlm` command-line tool** (NotebookLM), met
`nlm cross query "..." -n "John - exegesis"`. Als notebook staat daarnaast één primaire-tekstcorpus
klaar, `De Complete Dode Zeerollen (English)`, voor Qumran-/Dode Zeerollen-claims (1QS enz.) die niet
in Sefaria of Perseus zitten. Naast deze commentaren toetsen de opponenten toetsbare
beweringen waar mogelijk zelf aan de **primaire teksten**. Daarvoor is er een eigen command-line
tool, `brontekst` (in `.agents/tools/`), die teksten deterministisch ophaalt uit **Sefaria** (joodse
bronnen) en de **Perseus/Scaife**-corpora (klassiek Grieks en Latijn); voor de NT-grondtekst blijven
biblehub/NA28 in gebruik, en voor Qumran het Dode Zeerollen-notebook. Elke bron wordt getagd als primair of secundair. Ze mogen
nieuwe, creatieve invalshoeken inbrengen (papyrologie, tekstkritiek, patristiek, filosofische
receptie, sociaal-historisch, enz.), zolang die op hun eigen as blijven. Ze schrijven in het
Nederlands.

De **moderator** is neutraal en scoort per ronde op **twee onafhankelijke assen**, omdat datering en
cultureel karakter niet hoeven samen te vallen. Een late Johannes kan via de *Parting of the Ways*
juist Grikser zijn, en een vroege Johannes kan diep joods van kleur zijn; "vroeg dus Grieks" is geen
automatisme. De moderator toetst bovendien zelf steekproeven aan de primaire tekst en rapporteert
hoezeer het oordeel op secundaire bronnen rust.

```
DATERING-as                         KARAKTER-as
⏳ Vroeg  <-->  🕰️ Laat              🏛️ Grieks-Romeins  <-->  ✡️ Joods

-10 ..... 0 ..... +10               -10 ..... 0 ..... +10
 vroeg  midden  laat                 Grieks-  midden  Joods
(vóór 70)      (post-85)             Romeins
```

---

## Hoe gebruik je de skill

### Starten
Roep de skill aan in een taalmodel-CLI in deze repo:

```
/evangelie-debat
```

…of in natuurlijke taal, bijvoorbeeld:

> "Start het evangelie-debat."
> "Voer het debat over de datering van Johannes (Van Kooten) uit."

De hoofdsessie fungeert als **orchestrator**: hij maakt een run-map aan, kopieert de templates en
draait de debatlus volautomatisch tot convergentie.

### Q-debat starten
Roep de Q-skill aan in dezelfde repo:

```
/q-debat
```

…of in natuurlijke taal, bijvoorbeeld:

> "Start het Q-debat."
> "Voer een debat over bron Q met een voorstander en tegenstander."

Dit debat gebruikt twee opponenten en één moderator:

| Opponent | Standpunt | Kernargumenten |
|---|---|---|
| 📜 **Voor Q** | Mattheüs en Lucas gebruikten naast Marcus een gedeelde, niet bewaarde bron | dubbele traditie; volgordeverschillen; afwisselende primitiviteit; redactionele waarschijnlijkheid |
| 🪶 **Tegen Q** | Q is overbodig, Lucas kan Mattheüs hebben gekend en gebruikt | Van Kootens latere Lucas; geen bewaard Q-geschrift; Farrer-Goulder-Goodacre-lijn; minor agreements; redactionele vermoeidheid |

De moderator scoort op één as: `−10 = sterk vóór Q`, `0 = midden`, `+10 = sterk tegen Q`.

### Parameters aanpassen (optioneel)
Standaard draait het debat tot maximaal 8 rondes en stopt zodra de score 2 rondes stabiel is
(|Δ| ≤ 1). Je kunt dit bij het starten overschrijven, bijvoorbeeld:

> "Start het evangelie-debat met maximaal 4 rondes."

| Parameter | Default | Betekenis |
|---|---|---|
| `MAX_RONDES` | 8 | Harde bovengrens op het aantal rondes |
| `CONV_DREMPEL` | 1 | Score-verandering die als "stabiel" telt (|Δ| ≤ drempel) |
| `CONV_GEDULD` | 2 | Aantal opeenvolgende stabiele rondes om te stoppen |

### Wat er per ronde gebeurt
1. De **datering-as** debatteert: Opponent **Vroeg** en Opponent **Laat** weerleggen elkaar en
   brengen elk ≥1 nieuw dateringsargument/bron in.
2. De **karakter-as** debatteert: Opponent **Grieks-Romeins** en Opponent **Joods** doen hetzelfde
   over het culturele karakter.
3. De **moderator** vat de ronde samen, weegt de argumenten, markeert onverifieerbare citaten,
   toetst een claim aan de primaire tekst en geeft twee scores (datering op grond van Vroeg/Laat,
   karakter op grond van Grieks-Romeins/Joods, elk −10..+10) met onderbouwing; hij werkt `state.json`
   bij.
4. De orchestrator leest `state.json` en bepaalt of het debat doorgaat of stopt.

De vier opponenten draaien **sequentieel**, zodat elke volgende altijd op de voorgaande beurten kan
reageren; dat is nodig omdat subagents geen geheugen delen. De openingsvolgorde wisselt per ronde
tegen first-mover-bias.

---

## Resultaten bekijken

Elke run schrijft naar een eigen map onder `debat-output/`. Het Johannesdebat gebruikt `run-*`, het
Q-debat gebruikt `q-run-*`:

```
debat-output/run-<datum-tijd>/
  whiteboard.md     # het volledige debat, ronde voor ronde, met bronnen
  state.json        # scoregeschiedenis (ronde, datering, karakter, delta's), machineleesbaar
  sources.md        # bronnenlog: per claim de herkomst, primair/secundair, opgehaald ja/nee
  eindrapport.md    # eindoordeel, scoreverloop, sterkste argumenten, openstaande vragen
debat-output/q-run-<datum-tijd>/
  whiteboard.md     # het volledige Q-debat, ronde voor ronde, met bronnen
  state.json        # scoregeschiedenis op de Q-as
  sources.md        # bronnenlog
  eindrapport.md    # eindoordeel over Q
```

Lees `eindrapport.md` voor de conclusie en `whiteboard.md` voor het volledige verloop met alle
geciteerde bronnen.

Een overzicht van alle uitgevoerde runs met directe links naar de eindrapporten staat in
**[`debat-output/README.md`](debat-output/README.md)**.

---

## Hoe het in elkaar zit

```
.agents/
  agents/
    evangelie-vroeg.md            # subagent: Opponent Vroeg (datering, vóór 66-70)
    evangelie-laat.md             # subagent: Opponent Laat (datering, post-85)
    evangelie-grieks-romeins.md   # subagent: Opponent Grieks-Romeins (karakter, hellenistisch)
    evangelie-joods.md            # subagent: Opponent Joods (karakter, joods)
    evangelie-moderator.md        # subagent: neutrale jury → samenvatting + score op twee assen
    q-voorstander.md              # subagent: Opponent Voor Q
    q-tegenstander.md             # subagent: Opponent Tegen Q
    q-moderator.md                # subagent: neutrale jury → samenvatting + score op de Q-as
  skills/evangelie-debat/
    SKILL.md                  # orchestrator: de volautomatische debatlus
    reference/
      achtergrond.md          # Van Kootens 4 pijlers + tegenargumenten (uit de docx)
      scoring-rubric.md       # twee assen (datering + karakter) + weegcriteria + anti-fabricatie
      bronnen.md              # seed-bibliografie (secundair + primair corpus), gecategoriseerd
      primaire-bronnen.md     # handleiding bij de brontekst-CLI (Sefaria + Perseus/Scaife)
    templates/
      whiteboard-template.md  # format van het gedeelde whiteboard
      state-template.json     # startstructuur voor de scoregeschiedenis (twee assen)
      sources-template.md     # format van de bronnenlog (primair/secundair, opgehaald)
  skills/q-debat/
    SKILL.md                  # orchestrator: volautomatische debatlus over Q
    reference/
      achtergrond.md          # artikelpassage over Q + centrale vragen
      scoring-rubric.md       # Q-as + weegcriteria + anti-fabricatie
      bronnen.md              # seed-zoekroutes voor Q en niet-Q modellen
    templates/
      whiteboard-template.md  # format van het Q-whiteboard
      state-template.json     # startstructuur voor de Q-scoregeschiedenis
      sources-template.md     # format van de Q-bronnenlog
  tools/
    brontekst                 # CLI voor primaire teksten (Sefaria joods + Perseus/Scaife klassiek)
achtergrondmateriaal/         # bronartikel over de Van Kooten-casus (.docx)
debat-output/                 # gegenereerde runs (per run een submap)
  README.md                   # index van alle runs met links naar de eindrapporten
```

### Ontwerpprincipes
- **Whiteboard = gedeeld geheugen.** Subagents zijn stateless; alle debatstaat leeft in
  `whiteboard.md`. Elke agent leest het volledig en appendt zijn beurt.
- **Eén opponent per pool.** In het Johannesdebat zijn dat vier opponenten, twee per as. In het
  Q-debat zijn dat twee opponenten op één as, Voor Q en Tegen Q.
- **Neutrale scoring.** Niet de partijdige opponenten maar een aparte moderator scoort. Bij Johannes
  gebeurt dat op twee onafhankelijke assen; bij Q op één as van sterk vóór Q tot sterk tegen Q.
- **Primair én secundair.** Opponenten en moderator scheiden moderne commentaren (secundair) van
  antieke teksten (primair) en toetsen claims waar mogelijk zelf aan de primaire tekst.
- **Deterministische stop.** Convergentie wordt gemeten aan de scoregeschiedenis in `state.json`,
  niet op gevoel.
- **Anti-fabricatie.** Opponenten mogen alleen echt opgehaalde URL's citeren; de moderator
  markeert en kort onverifieerbare bronnen.
- **Voortgangsplicht.** Elke ronde moet minstens één nieuw argument/bron opleveren, anders
  versnelt de convergentie; dat voorkomt eindeloze herhaling.

---

## Vereisten en aandachtspunten
- Draai de skill **vanuit deze repo** (de subagents en reference-bestanden staan onder `.agents/`).
- De opponenten gebruiken **WebSearch/WebFetch**; een live run kan enkele minuten duren en doet
  meerdere webverzoeken per ronde.
- De **commentaar-notebooks** vereisen de `nlm` CLI (NotebookLM Tools) op het PATH en een geldige
  login (`nlm login`). Ontbreekt die, dan vallen de opponenten automatisch terug op het open web.
- De **`brontekst` CLI** (`.agents/tools/brontekst`) voor primaire teksten heeft alleen `python3` en
  een internetverbinding nodig (Sefaria-API en de Perseus-TEI op GitHub); geen installatie of sleutel.
- De inhoud is bewust **brongedreven en eerlijk**: het doel is winnen op bewijskracht, niet op
  retoriek. Controleer bij twijfel de geciteerde bronnen in `whiteboard.md` zelf.
- Voor een snelle proefrun: start met `MAX_RONDES=2`.
