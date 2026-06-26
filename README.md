# Evangelie-debat, een LLM-skill

Een skill die een **iteratief, brongebaseerd debat** voert over de datering van het
Johannesevangelie: het strijdpunt uit George (Geurt Henk) van Kootens *Echo's van het goede
nieuws: De evangeliën in context, toen en nu* (2025/2026).

Twee tegengestelde subagent-opponenten reageren om de beurt op elkaar via een gedeeld
"whiteboard", dragen elke ronde **echte, online gezochte bronnen** aan (ook grammaticaal en
syntactisch), en een **neutrale moderator** scoort de stand van de evidentie. Zodra de score
stabiliseert, stopt het debat met een eindrapport.

---

## De twee kampen

| Opponent | Standpunt | Kernargumenten |
|---|---|---|
| 🏛️ **Grieks** | Pro Van Kooten: Johannes is het **oudste** evangelie (vóór 66–70 n.Chr.), gelezen in Grieks-Romeinse context | `estin`-praesens in Joh 5:2 (Betzata); superieure pre-70-topografie van Jeruzalem; Lukaanse posterioriteit (Lucas 93–130, leunt op Johannes); bron Q overbodig |
| ✡️ **Joods** | Late datering (**post-85 n.Chr.**) en joodse invloed op het NT | praesens historicum is geen dateringsbewijs; joodse/OT-symboliek en hermeneutiek; `aposynagōgos` / Martyn; joods-Palestijns milieu (Qumran) |

Beide opponenten zoeken **echte bronnen** op het open web en raadplegen daarnaast ingelezen
**commentaar-notebooks** per bijbelboek (`John - exegesis`, `Luke - exegesis`, `Matthew - exegesis`,
`Mark - exegesis`, en meer) via de **`nlm` command-line tool** (NotebookLM), met
`nlm cross query "..." -n "John - exegesis"`. Vanaf de tweede ronde mogen ze ook nieuwe, creatieve
invalshoeken inbrengen (papyrologie, tekstkritiek, patristiek, sociaal-historisch, enz.). Ze
schrijven in het Nederlands.

De **moderator** is neutraal en geeft per ronde één score:

```
-10 ........ -5 ........ 0 ........ +5 ........ +10
 sterk      neigt    evidentie    neigt      sterk
 GRIEKS     Grieks   in midden    Joods      JOODS
(vroeg John)                             (laat John, joods)
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
1. **Opponent A** leest het whiteboard, weerlegt de vorige beurt, zoekt online ≥1 nieuw argument/bron
   en schrijft zijn beurt onderaan.
2. **Opponent B** (de andere zijde) doet hetzelfde en ziet daarbij de verse beurt van A.
3. De **moderator** vat de ronde samen, weegt de argumenten, markeert onverifieerbare citaten en
   geeft een score (−10..+10) met onderbouwing; hij werkt `state.json` bij.
4. De orchestrator leest `state.json` en bepaalt of het debat doorgaat of stopt.

De opponenten draaien **sequentieel**, zodat de tweede altijd op de eerste kan reageren; dat is
nodig omdat subagents geen geheugen delen.

---

## Resultaten bekijken

Elke run schrijft naar een eigen map onder `debat-output/`:

```
debat-output/run-<datum-tijd>/
  whiteboard.md     # het volledige debat, ronde voor ronde, met bronnen
  state.json        # scoregeschiedenis (ronde, score, delta), machineleesbaar
  eindrapport.md    # eindoordeel, scoreverloop, sterkste argumenten, openstaande vragen
```

Lees `eindrapport.md` voor de conclusie en `whiteboard.md` voor het volledige verloop met alle
geciteerde bronnen.

---

## Hoe het in elkaar zit

```
.agents/
  agents/
    evangelie-grieks.md       # subagent: Opponent Grieks (pro Van Kooten)
    evangelie-joods.md        # subagent: Opponent Joods (late datering / joods)
    evangelie-moderator.md    # subagent: neutrale jury → samenvatting + score
  skills/evangelie-debat/
    SKILL.md                  # orchestrator: de volautomatische debatlus
    reference/
      achtergrond.md          # Van Kootens 4 pijlers + tegenargumenten (uit de docx)
      scoring-rubric.md       # schaal -10..+10 + weegcriteria + anti-fabricatie
      bronnen.md              # seed-bibliografie (URL's), gecategoriseerd
    templates/
      whiteboard-template.md  # format van het gedeelde whiteboard
      state-template.json     # startstructuur voor de scoregeschiedenis
achtergrondmateriaal/         # bronartikel over de Van Kooten-casus (.docx)
debat-output/                 # gegenereerde runs (per run een submap)
```

### Ontwerpprincipes
- **Whiteboard = gedeeld geheugen.** Subagents zijn stateless; alle debatstaat leeft in
  `whiteboard.md`. Elke agent leest het volledig en appendt zijn beurt.
- **Neutrale scoring.** Niet de partijdige opponenten maar een aparte moderator scoort.
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
- De inhoud is bewust **brongedreven en eerlijk**: het doel is winnen op bewijskracht, niet op
  retoriek. Controleer bij twijfel de geciteerde bronnen in `whiteboard.md` zelf.
- Voor een snelle proefrun: start met `MAX_RONDES=2`.
