# AGENTS.md

Projectgids voor agentische tools (LLM-agnostisch). De canonieke locaties zijn dit bestand
(`AGENTS.md`) en de map `.agents/`. Wijst jouw tool naar een andere conventie (bijvoorbeeld
`CLAUDE.md` of `.claude/`), laat die dan naar respectievelijk `AGENTS.md` en `.agents/` verwijzen
of kopieer ze, zodat elke tool dezelfde instructies en dezelfde skill-/agentdefinities gebruikt.

## Wat dit project is
Een orchestratie die een iteratief, brongebaseerd debat voert over de datering van het
Johannesevangelie: de triangulatie van George (Geurt Henk) van Kooten. Vier opponenten (subagents)
debatteren in twee paren, één per as: Vroeg tegen Laat op de datering-as en Grieks-Romeins tegen
Joods op de karakter-as, via een gedeeld whiteboard-bestand. Een neutrale moderator scoort elke ronde
op twee onafhankelijke assen, datering (−10 sterk vroeg .. +10 sterk laat) en karakter (−10 sterk
Grieks-Romeins .. +10 sterk Joods), en het debat stopt zodra beide scores stabiliseren.

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
  skills/evangelie-debat/
    SKILL.md                      orchestrator: de volautomatische debatlus
    reference/                    achtergrond.md, scoring-rubric.md, bronnen.md, primaire-bronnen.md
    templates/                    whiteboard-template.md, state-template.json, sources-template.md
  tools/
    brontekst                     CLI om primaire teksten op te halen (Sefaria + Perseus/Scaife)
achtergrondmateriaal/             bronartikel over de Van Kooten-casus (.docx)
debat-output/                     gegenereerde runs (per run een submap)
```

## Het debat starten
- Ondersteunt jouw tool skills/slash-commando's: roep de skill `evangelie-debat` aan
  (bijvoorbeeld `/evangelie-debat`), of vraag in gewone taal "start het evangelie-debat".
- Anders: lees `.agents/skills/evangelie-debat/SKILL.md` en voer de orchestratieprocedure daarin uit
  (run-map aanmaken, templates kopiëren, dan per ronde de vier opponenten één voor één, gevolgd door
  de moderator, met convergentiecontrole via `state.json`).

De orchestrator delegeert al het inhoudelijke werk aan de vijf rollen in `.agents/agents/` (vier
opponenten plus moderator). Die rollen zijn de enige bron van waarheid voor hun gedrag.

## Belangrijke werkafspraken (gelden voor alle rollen)
- **Gedeeld geheugen is het whiteboard-bestand.** Subagents zijn stateless; ze lezen het hele
  whiteboard en appenden hun beurt. De orchestrator leest alleen `state.json`.
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
  Uitleg en grenzen in `skills/evangelie-debat/reference/primaire-bronnen.md`.
- **Eerlijkheid.** Citeer alleen echt geraadpleegde bronnen; verzin niets. De moderator markeert en
  kort onverifieerbare citaten.
- **Stijl.** Schrijf natuurlijk Nederlands. Geen lange gedachtestreepjes (em-dashes) en geen
  stijltics.
