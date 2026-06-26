# AGENTS.md

Projectgids voor agentische tools (LLM-agnostisch). `CLAUDE.md` is een symlink naar dit bestand,
en `.claude/` is een symlink naar `.agents/`, zodat zowel Claude Code als andere tools dezelfde
instructies en dezelfde skill-/agentdefinities gebruiken.

## Wat dit project is
Een orchestratie die een iteratief, brongebaseerd debat voert over de datering van het
Johannesevangelie: de triangulatie van George (Geurt Henk) van Kooten. Twee tegengestelde
opponenten (subagents) reageren om de beurt op elkaar via een gedeeld whiteboard-bestand, een
neutrale moderator scoort elke ronde van −10 (Grieks, vroege Johannes) tot +10 (Joods, late
datering), en het debat stopt zodra de score stabiliseert.

Zie `README.md` voor de uitleg voor mensen.

## Structuur
```
.agents/                      (canoniek; .claude/ is hiernaar een symlink)
  agents/                     subagent-rollen
    evangelie-grieks.md       Opponent Grieks (pro Van Kooten, vroege Johannes)
    evangelie-joods.md        Opponent Joods (late datering, joodse invloed)
    evangelie-moderator.md    neutrale jury: samenvatting + score + convergentie
  skills/evangelie-debat/
    SKILL.md                  orchestrator: de volautomatische debatlus
    reference/                achtergrond.md, scoring-rubric.md, bronnen.md
    templates/                whiteboard-template.md, state-template.json
achtergrondmateriaal/         bronartikel over de Van Kooten-casus (.docx)
debat-output/                 gegenereerde runs (per run een submap)
```

## Het debat starten
- In Claude Code: roep de skill `evangelie-debat` aan (`/evangelie-debat`), of vraag in gewone taal
  "start het evangelie-debat".
- In een andere agentische tool: lees `.agents/skills/evangelie-debat/SKILL.md` en voer de
  orchestratieprocedure daarin uit (run-map aanmaken, templates kopiëren, dan de lus
  opponent A → opponent B → moderator, met convergentiecontrole via `state.json`).

De orchestrator delegeert al het inhoudelijke werk aan de drie rollen in `.agents/agents/`. Die
rollen zijn de enige bron van waarheid voor hun gedrag.

## Belangrijke werkafspraken (gelden voor alle rollen)
- **Gedeeld geheugen is het whiteboard-bestand.** Subagents zijn stateless; ze lezen het hele
  whiteboard en appenden hun beurt. De orchestrator leest alleen `state.json`.
- **Bronnen.** Opponenten gebruiken het open web (WebSearch/WebFetch) én de NotebookLM-commentaren
  via de `nlm` CLI, bijvoorbeeld `nlm cross query "..." -n "John - exegesis"` (notebooks:
  `John/Luke/Matthew/Mark - exegesis`, en meer). Vereist de `nlm` CLI op het PATH met een geldige
  login; anders terugval op het web.
- **Eerlijkheid.** Citeer alleen echt geraadpleegde bronnen; verzin niets. De moderator markeert en
  kort onverifieerbare citaten.
- **Stijl.** Schrijf natuurlijk Nederlands. Geen lange gedachtestreepjes (em-dashes) en geen
  stijltics.
