# Scoring-rubric (alleen voor de Moderator)

De moderator geeft na elke ronde **één signed score** voor de actuele stand van de evidentie:

```
-10 ........ -5 ........ 0 ........ +5 ........ +10
 sterk      neigt     evidentie    neigt      sterk
 GRIEKS     Grieks    in midden    Joods      JOODS
(vroeg John)                              (late John, joods)
```

- **Negatief** = de evidentie ondersteunt per saldo Van Kooten / vroege Johannes (Grieks).
- **Positief** = de evidentie ondersteunt per saldo de late datering / joodse invloed (Joods).
- **0** = in evenwicht.

De score is een **momentopname van de totale bewijsbalans**, niet "wie debatteerde mooier".

## Schaalankers
| Bereik | Betekenis |
|---|---|
| −10 … −7 | Sterk Grieks: pijlers staan grotendeels overeind, tegenargumenten weerlegd |
| −6 … −3 | Neigt Grieks: meer/sterker bewijs vroeg, maar serieuze openstaande bezwaren |
| −2 … +2 | Midden: bewijs in evenwicht of beide kanten grotendeels speculatief |
| +3 … +6 | Neigt Joods: late datering / joods milieu beter onderbouwd |
| +7 … +10 | Sterk Joods: Van Kootens pijlers overtuigend ondergraven |

## Weegcriteria (waarom weegt een argument zwaar, verplicht expliciet maken)
1. **Evidentiële kracht**: direct tekstueel/archeologisch/grammaticaal bewijs > analogie/parallel >
   speculatie/aanname. Een verifieerbare primaire observatie weegt het zwaarst.
2. **Bronkwaliteit**: peer-reviewed artikel of primaire bron > academische blog/instituut >
   populaire media > onverifieerbaar. Noteer de hoogste betrouwbare bron achter een claim.
3. **Weerlegging**: een argument dat door de tegenpartij **overtuigend** is weerlegd, verliest
   gewicht of valt weg. Volg argumenten over rondes heen, een eerder sterk punt kan kelderen.
4. **Methodologische soliditeit**: een grammaticaal/syntactisch patroon dat **generaliseert**
   (over veel teksten geldt) > een ad-hoc-uitzondering. Eén tegenvoorbeeld sloopt geen regel,
   maar veel tegenvoorbeelden wel.
5. **Verifieerbaarheid**: is de geciteerde bron echt opgehaald en zegt hij wat geclaimd wordt?
   Onverifieerbare of (vermoedelijk) verzonnen citaten → **markeren en in gewicht korten of negeren**.

## Anti-fabricatie (hard)
LLM's verzinnen notoir bijbelwetenschappelijke referenties. Behandel elke claim met een citaat dat
je niet kunt plaatsen als **verdacht**. Markeer in de "Weging" met `⚠️ onverifieerbaar` en laat zo'n
claim **niet** de score bepalen. Doe bij twijfel een steekproef-WebFetch op de geciteerde URL.

## Voortgang & convergentie
- Noteer per zijde **hoeveel nieuwe, valide argumenten/bronnen** deze ronde zijn toegevoegd
  (`new_evidence_grieks`, `new_evidence_joods`). 0 nieuwe valide evidentie aan een kant = signaal
  dat die kant uitgeput raakt.
- Zet `concession` als een zijde een punt expliciet opgeeft (welk punt).
- De **orchestrator** beslist over stoppen op basis van `state.json`; jij levert eerlijke scores en
  delta's. Forceer geen kunstmatige stabiliteit en overdrijf geen beweging, wees consistent over
  rondes heen, zodat een echt uitgedebatteerd onderwerp vanzelf stabiliseert.

## Output van de moderator per ronde
1. Append aan het whiteboard onder `### ⚖️ Moderator, Stand van zaken`:
   - **Samenvatting** van de ronde (2–4 zinnen).
   - **Sterkste argument Grieks** / **Sterkste argument Joods** (elk 1 zin + bron).
   - **Weging**: waarom de score zo uitvalt; welke argumenten zwaar/licht wegen en waarom;
     eventuele `⚠️ onverifieerbaar`-markeringen.
   - **Score: X · Δ t.o.v. vorige: Y**.
2. Werk de scorebord-tabel (`## 📊 Scorebord`) boven in het whiteboard bij met een rij voor deze
   ronde: `| N | X | Y | stand in één zin |`.
3. Werk `state.json` bij: voeg een `history`-item toe `{round, score, delta, rationale,
   new_evidence_grieks, new_evidence_joods, concession}` en update `round`.
