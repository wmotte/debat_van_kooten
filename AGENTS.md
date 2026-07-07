# AGENTS.md

Projectgids voor agentische tools (LLM-agnostisch). De canonieke locaties zijn dit bestand
(`AGENTS.md`) en de map `.agents/`. Wijst jouw tool naar een andere conventie (bijvoorbeeld
`CLAUDE.md` of `.claude/`), laat die dan naar respectievelijk `AGENTS.md` en `.agents/` verwijzen
of kopieer ze, zodat elke tool dezelfde instructies en dezelfde skill-/agentdefinities gebruikt.

## Wat dit project is
Een set orchestraties voor iteratieve, brongebaseerde debatten rond George (Geurt Henk) van Kootens
reconstructie van de evangeliën. Het eerste debat gaat over de datering en het culturele karakter van
het Johannesevangelie. Vier opponenten (subagents) debatteren in twee paren, één per as: Vroeg tegen
Laat op de datering-as en Grieks-Romeins tegen Joods op de karakter-as. Een neutrale moderator scoort
elke ronde op twee onafhankelijke assen.

Het tweede debat gaat over de synoptische bron Q. Daar debatteren twee opponenten, Voor Q en Tegen Q,
op één as: is Q de beste verklaring voor de dubbele traditie, of is Q overbodig omdat Lucas Mattheüs
kan hebben gebruikt? Ook daar bewaakt een neutrale moderator de score en convergentie.

Zie `README.md` voor de uitleg voor mensen.

## Structuur
```
.agents/                          (canonieke map met skill-/agentdefinities)
  agents/                         subagent-rollen
    evangelie-vroeg.md            Opponent Vroeg (datering-as, vóór 66-70)
    evangelie-laat.md             Opponent Laat (datering-as, post-85)
    evangelie-grieks-romeins.md   Opponent Grieks-Romeins (karakter-as, hellenistisch)
    evangelie-joods.md            Opponent Joods (karakter-as, joods)
    evangelie-moderator.md        neutrale jury: samenvatting + score op twee assen + convergentie
    q-voorstander.md              Opponent Voor Q (gedeelde bronhypothese)
    q-tegenstander.md             Opponent Tegen Q (Lucas gebruikt Mattheüs, Q overbodig)
    q-moderator.md                neutrale jury: samenvatting + score op de Q-as + convergentie
  skills/evangelie-debat/
    SKILL.md                      orchestrator: de volautomatische debatlus
    reference/                    achtergrond.md, scoring-rubric.md, bronnen.md, primaire-bronnen.md
    templates/                    werkdossier-template.md, state-template.json, sources-template.md
  skills/q-debat/
    SKILL.md                      orchestrator: debat over de synoptische bron Q
    reference/                    achtergrond.md, scoring-rubric.md, bronnen.md
    templates/                    werkdossier-template.md, state-template.json, sources-template.md
  tools/
    brontekst                     CLI om primaire teksten op te halen (Sefaria + Perseus/Scaife)
achtergrondmateriaal/             bronartikel over de Van Kooten-casus (.docx)
debat-output/                     gegenereerde runs (per run een submap)
```

## Het debat starten
- Ondersteunt jouw tool skills/slash-commando's: roep de skill `evangelie-debat` aan
  (bijvoorbeeld `/evangelie-debat`), of vraag in gewone taal "start het evangelie-debat".
- Voor het Q-debat: roep de skill `q-debat` aan (bijvoorbeeld `/q-debat`), of vraag in gewone taal
  "start het Q-debat".
- Anders: lees `.agents/skills/evangelie-debat/SKILL.md` en voer de orchestratieprocedure daarin uit
  (run-map aanmaken, templates kopiëren, dan per ronde de vier opponenten één voor één, gevolgd door
  de moderator, met convergentiecontrole via `state.json`).
- Voor Q lees je analoog `.agents/skills/q-debat/SKILL.md` en draai je per ronde de twee opponenten,
  gevolgd door de moderator.

De orchestrator delegeert al het inhoudelijke werk aan de rollen in `.agents/agents/`. Die rollen zijn
de enige bron van waarheid voor hun gedrag.

## Belangrijke werkafspraken (gelden voor alle rollen)
- **Gedeeld geheugen is het werkdossier-bestand.** Subagents zijn stateless; ze lezen het hele
  werkdossier en appenden hun beurt. De orchestrator leest alleen `state.json`.
- **Bronnen.** Opponenten gebruiken het open web (WebSearch/WebFetch) én de NotebookLM-commentaren
  via de `nlm` CLI, bijvoorbeeld `nlm cross query "..." -n "John - exegesis"` (notebooks:
  `John/Luke/Matthew/Mark - exegesis`, en meer). Naast de commentaren staat er één primaire-tekstcorpus
  als notebook klaar: `De Complete Dode Zeerollen (English)`, de route voor Qumran-/Dode Zeerollen-claims
  (1QS enz.) die niet in Sefaria of Perseus staan; het is een Engelse vertaling via notebook, dus tag een
  treffer als primair maar markeer de vertaal-/notebookherkomst. Vereist de `nlm` CLI op het PATH met een
  geldige login; anders terugval op het web.
- **Primaire teksten.** Voor het toetsen van een claim aan de échte primaire tekst is er de
  `brontekst` CLI in `.agents/tools/` (alleen `python3` nodig): `brontekst sefaria "<ref>"` voor
  joodse bronnen (Sefaria) en `brontekst perseus "<cts-urn>"` voor klassiek Grieks/Latijn
  (Perseus/Scaife). Voor Qumran (niet in beide databases) zie het Dode Zeerollen-notebook hierboven.
  Uitleg en grenzen in `skills/evangelie-debat/reference/primaire-bronnen.md`. Voor het Q-debat is de
  primaire tekst meestal de Griekse tekst van Mattheüs, Marcus en Lucas; die zit niet in `brontekst`,
  dus gebruik daarvoor betrouwbare NT-edities, interlinears of commentaar-notebooks en noteer de route.
- **Eerlijkheid.** Citeer alleen echt geraadpleegde bronnen; verzin niets. De moderator markeert en
  kort onverifieerbare citaten.
- **Stijl.** Schrijf natuurlijk Nederlands. Geen lange gedachtestreepjes (em-dashes) en geen
  stijltics.
