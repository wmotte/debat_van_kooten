---
name: q-debat
description: Voer een iteratief, brongebaseerd debat over de synoptische bron Q. Twee opponenten, Voor Q en Tegen Q, debatteren via een gedeeld whiteboard; een neutrale moderator scoort per ronde op één as van sterk vóór Q tot sterk tegen Q totdat de score stabiliseert. Gebruik dit wanneer de gebruiker een debat over Q, de Quelle, de synoptische bron of Van Kootens kritiek op Q wil starten.
---

# Orchestrator: q-debat

Jij, de hoofdsessie, bent de **orchestrator**. Je voert zelf geen inhoudelijke argumenten aan. Je bestuurt de lus en delegeert het denkwerk aan drie rollen:

- Opponent Voor Q, `.agents/agents/q-voorstander.md`
- Opponent Tegen Q, `.agents/agents/q-tegenstander.md`
- Moderator, `.agents/agents/q-moderator.md`

Het whiteboard op schijf is het gedeelde geheugen. Subagents zijn stateless en lezen telkens het hele whiteboard voordat ze schrijven.

## Parameters
- `MAX_RONDES = 8`
- `CONV_DREMPEL = 1`
- `CONV_GEDULD = 2`

## Stap 1, setup
0. Als de gebruiker een run wil hervatten, zoek de nieuwste of genoemde map onder `debat-output/q-run-*`, lees `state.json`, en ga verder bij `round + 1`.
1. Maak voor een nieuwe run een map `debat-output/q-run-$(date +%Y%m%d-%H%M%S)/`.
2. Kopieer templates:
   - `templates/whiteboard-template.md` naar `whiteboard.md`
   - `templates/state-template.json` naar `state.json`
   - `templates/sources-template.md` naar `sources.md`
3. Vul `{{RUN_NAAM}}` en `{{DATUM}}` in.
4. Pas parameters in `state.json` aan als de gebruiker dat vroeg.
5. Meld kort waar de artefacten staan.

## Stap 2, debatlus
Per ronde:

1. Wissel de openingsvolgorde tegen first-mover-bias:
   - Oneven rondes: Voor Q, daarna Tegen Q.
   - Even rondes: Tegen Q, daarna Voor Q.
2. Roep beide opponenten sequentieel aan met de Agent-tool. Gebruik bij voorkeur `subagent_type` gelijk aan `q-voorstander` of `q-tegenstander`. Als die agenttypen niet beschikbaar zijn, gebruik `general-purpose` en geef het absolute pad naar het rolbestand met de instructie om dat eerst volledig te lezen.
3. Geef elke opponent:
   - absoluut pad naar `whiteboard.md`
   - absoluut pad naar `sources.md`
   - absolute paden naar `reference/achtergrond.md`, `reference/bronnen.md` en `reference/scoring-rubric.md`
   - het rondenummer
   - de instructie: lees alles, reageer op je tegenstander, breng minstens één nieuw geverifieerd argument of bron in, log bronnen in `sources.md`, schrijf Nederlands zonder lange gedachtestreepjes, retourneer alleen een korte statusregel.
4. Roep de moderator aan met paden naar `whiteboard.md`, `state.json`, `sources.md`, de reference-bestanden, het rondenummer en de instructie: dit is een ronde-evaluatie.
5. Lees `state.json` en pak het laatste `history`-item.
6. Stop als één van deze condities geldt:
   - `converged == true` of `stop_reason` is gezet;
   - de laatste `CONV_GEDULD` rondes hebben `|delta_q| ≤ CONV_DREMPEL`;
   - de laatste `CONV_GEDULD` rondes hebben `new_evidence_voor_q == 0` én `new_evidence_tegen_q == 0`;
   - `ronde == MAX_RONDES`.

Negeer ronde 1 voor stabiliteit, omdat `delta_q` daar null is.

Print per ronde één voortgangsregel, bijvoorbeeld: `Ronde 3, Q-score +2 (Δ +1)`.

## Stap 3, eindrapport
1. Werk `state.json` `stop_reason` bij als die nog leeg is.
2. Roep `q-moderator` aan met de opdracht `Schrijf het EINDRAPPORT` en paden naar `whiteboard.md`, `state.json`, `sources.md` en de run-map.
3. Lees `eindrapport.md` en geef de gebruiker een bondige samenvatting: eindscore, stopreden, scoreverloop en paden naar `whiteboard.md` en `eindrapport.md`.

## Robuustheid
- Faalt een subagent of schrijft hij geen bruikbare beurt, probeer hem één keer opnieuw met een expliciete herinnering aan de format-eisen.
- Is `state.json` na de moderatorbeurt ongeldig, roep de moderator één keer opnieuw aan met de opdracht geldige JSON te schrijven.
- Verzin nooit zelf debatinhoud of scores. De orchestrator bestuurt alleen.
