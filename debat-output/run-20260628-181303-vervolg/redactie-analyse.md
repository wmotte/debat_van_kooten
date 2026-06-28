# Redactie-analyse, run-20260628-181303-vervolg

Kritische anti-tic- en stijlredactie over `whiteboard.md`, `eindrapport.md` en `sources.md`.
Diagnostisch rapport: de debatteksten zijn niet herschreven. Tellingen zijn met grep/ripgrep hard
gemaakt; tics die grep niet vangt zijn steekproefsgewijs beoordeeld. Regelnummers verwijzen naar het
genoemde bestand.

## 1. Samenvatting en eindoordeel

| Bestand | Em-dashes | Anglicismen (lopende tekst) | Top-3 tics | Kwalificatie |
|---|---|---|---|---|
| `whiteboard.md` | 0 | ~22 | "Mijn nieuwe front is" (15x), anker/verankeren (38x), neutraliteitsval/kroongetuige | **6,5 / 10** |
| `eindrapport.md` | 0 | 2 (foundationeel) | neutraliteitsval (4x), kroongetuige/stramien, foundationeel | **7,5 / 10** |
| `sources.md` | 0 | 0 (Engels zit in toegestane queries) | n.v.t. (structureel logboek) | **8,5 / 10** |

Hoofdoordeel. De harde nuldoelstelling op de gedachtestreepjes is volledig gehaald: **nul em-dashes en
nul en-dashes** in alle drie de bestanden. Dat is de grootste winst. De zwakte zit niet in de
interpunctie maar in de **monotone metaforiek** (alles is een "front", een "anker", een "kaart", een
"neutraliteitsval") en in een handvol echte **anglicismen** die in het Nederlands onnodig zijn
(downstream, notch, skew, knockout, gehedged/hedde, foundationeel). Het `whiteboard.md` is het zwaarst
besmet omdat elke opponentbeurt hetzelfde sjabloon opent; `eindrapport.md` is aanzienlijk schoner;
`sources.md` is als structureel logboek vrijwel onberispelijk (de Engelse tekst daarin staat in de
expliciet toegestane `nlm`-queries en eigennamen).

## 2. Harde overtredingen

### 2.1 Gedachtestreepjes (em-dash — / en-dash –)

| Bestand | em-dash (—) | en-dash (–) |
|---|---|---|
| whiteboard.md | 0 | 0 |
| eindrapport.md | 0 | 0 |
| sources.md | 0 | 0 |

**Volledig conform.** Geen enkele overtreding. Koppeltekens en jaartalbereiken (66-70, 85-100) zijn
correct met gewoon koppelteken gezet.

### 2.2 Anglicismen waar Nederlands bestaat (lopende tekst)

De gezochte signaalwoorden marker, timing, case, default, pivot, out-of-the-box, rubric, honest,
genuine komen **niet** als losse Engelse woorden in de lopende tekst voor (de treffer "markeringen" in
"onverifieerbaar-markeringen" is Nederlands; "scholars" staat uitsluitend in de toegestane Engelse
`nlm`-queries in `sources.md`). Wel gevonden, en wel echte overtredingen:

| Anglicisme | Bestand:regel | Aantal | Nederlands alternatief |
|---|---|---|---|
| downstream | whiteboard 1149, 1155, 1189 | 3 | "stroomafwaarts van", "ná", "later dan de brief" |
| notch | whiteboard 1411, 1422, 1446 | 3 | "punt", "stapje", "een streep" |
| (periode-)skew | whiteboard 811, 1003, 1015 | 3 | "vertekening per periode", "scheve verdeling" |
| knockout | whiteboard 352, 1050, 1411 | 3 | "genadeslag", "beslissende klap" |
| gehedged | whiteboard 1047 | 1 | "ingedekt", "met voorbehoud gebracht" |
| hedde (het zwaar) | whiteboard 1417 | 1 | "dekte het zwaar in", "maakte veel voorbehoud" |
| foundationeel/-ele | eindrapport 30, 111; whiteboard 197, 333, 873, 1114 | 6 | "fundamenteel", "grondleggend", "bronevangelie" |
| counterde / counter | whiteboard 318, 652, 1077 | 3 | "pareerde", "antwoordde", "weerlegging" |
| Grikser | whiteboard 35 | 1 | "meer Grieks (van kleur)" |

Randgevallen (verdedigbaar als geciteerd vakjargon, maar in lopende NL-tekst opvallend):
- "red herring" (whiteboard 487, 510): woordelijk citaat van Meeks. Laat staan met aanhalingstekens,
  maar overweeg "dwaalspoor" bij parafrase.
- "Parting of the Ways" (whiteboard 35): ingeburgerde vakterm; "Scheiding der Wegen" kan.
- "theios anēr", "vaticinium ex eventu", "machloket": Grieks/Latijn/Hebreeuws vakjargon, toegestaan.

### 2.3 Pre-/post-machinegeweer

| Patroon | whiteboard | eindrapport | sources |
|---|---|---|---|
| `post-<jaar>` e.d. (post-85, post-70, post-apostolisch) | 12 | 1 | 2 |
| `pre-<jaar>` | 0 | 0 | 3 |
| `vóór-70` (gekoppeld compound) | 18 | n.v.t. | n.v.t. |
| `vóór 70` (los) | 25 | n.v.t. | n.v.t. |

Twee bevindingen. Ten eerste de **post-reeks**: "post-85" en "post-70" worden 12 keer in het
whiteboard als kant-en-klaar Engels compositum gebruikt waar "ná 85" / "ná 70" hoort (het Nederlands
gebruikt het ook in de subagent-rolnaam, dus het is ingesleten). Ten tweede, en hinderlijker voor een
neerlandicus, de **inconsistentie** rond "vóór 70": 18 keer als koppelteken-compound "vóór-70"
(vóór-70 realia, vóór-70 kennis, vóór-70 chalksteen-industrie) tegenover 25 keer los "vóór 70". Kies
één lijn. Voorbijdrijvende voorbeelden: whiteboard 23 "uitsluitingspraktijk van vóór 70" naast 51
"de uitsluitingspraktijk van vóór 70" naast 24 "accurate vóór-70 kennis". Het gekoppelde "vóór-70" als
bijvoeglijke bepaling is de Nederlandse evenknie van het pre-/post-machinegeweer.

### 2.4 Wiskundetekens / schuine strepen in lopende tekst

- Eén wiskundeteken in lopende (regel)tekst: `**≥1 nieuw**` (whiteboard 62, spelregel). Schrijf
  "minstens één nieuw". Verder komen `−10 .. +10` en `Δ` voor; die staan in de score-notatie en zijn
  daar functioneel, geen lopende tekst.
- Schuine strepen: de talloze `grammaticaal/syntactisch`, `halachisch/archeologisch`,
  `liturgisch/exegetisch` staan in de gestructureerde **Type-** en **Aard-velden** van `sources.md` en
  zijn daar legitiem. In lopende prozatekst is geen storende `/`-als-"en/of" gevonden.
- Spelling "kristalliseert": **correct met k** ("uitkristalliseerde", whiteboard 203). Conform.

## 3. Tics en clichés

### 3.1 Het dominante structuurtic: "front"

Dit is de zwaarste stijlkwaal van het whiteboard. Het woord **"front" valt er 43 keer**, in het
eindrapport nog 8 keer. Bijna elke opponentbeurt opent letterlijk met hetzelfde sjabloon:

- **"Mijn nieuwe front is ..."**: 10x (whiteboard 88, 284, 404, 609, 766, 835, 968, 1120, 1203, 1274).
- **"Ik open een (nieuw) front ..."**: 5x (whiteboard 206, 476, 546, 896, 1335).

Samen **15 vrijwel identieke openers**, verdeeld over alle vier de opponenten (geen enkele opponent is
schuldiger dan een andere; het is een gedeeld sjabloon). Daar bovenop komt de bijna altijd
aangekoppelde formule **"een discipline die in deze hele run / dit hele debat nog niet aan bod kwam /
nog niet op de ... lag"** (12x). Het effect is een mechanisch, voorspelbaar ritme: elke beurt = front +
"nog niet eerder gebruikte discipline" + bewijs + "Drie eerlijke grenzen". Aanbeveling: varieer de
aanhef ("Ik verleg het debat naar ...", "Een onbesproken invalshoek is ...", "Hier breng ik ... in").

### 3.2 De strijd-/boksmetaforiek (overdaad)

De hele tekst is in één semantisch veld gegoten: gevecht. Naast "front/frontaal" (whiteboard: frontaal
5x) ook:
- **anker / verankeren / verankerd**: "anker" 22x + "veranker..." 16x in het whiteboard = ~38
  treffers; eindrapport 3 + 1. "Birkat ha-Minim-anker", "laat anker", "verankert zijn christologie".
  Sterk uitgemolken.
- **neutraliteitsval**: whiteboard 3x, eindrapport 4x (= 7x). Een zelfgemunte term die als vast cliché
  gaat functioneren.
- **kroongetuige**: whiteboard 6x, eindrapport 1x (= 7x), vaak "zijn eigen kroongetuige keert zich
  tegen hem".
- **(de) kaart**: "sterkste/beste kaart" 4x.
- **pareren/counterde/het mes terug**: pareer... 6x, counterde 3x, "keer ik hem het mes terug"
  (whiteboard 809).
- **vloer onder ... weg**: 4x.
- **"won de uitwisseling op bewijskracht"**: 3x (vaste moderatorformule).
- **knockout / notch**: zie 2.2 (tevens anglicismen).

Het register is daardoor eentonig agressief. Een neerlandicus zou aanraden minstens de helft van deze
beelden te vervangen door neutrale formuleringen ("steunpunt" i.p.v. "anker", "weerlegde" i.p.v.
"keerde het mes terug", "verschoof een punt" i.p.v. "trok een notch").

### 3.3 Overige clichématige openers en formules

- **"Sterker nog"**: 1x, en wel verstopt over een regeleinde (whiteboard 274-275: "... geen herkomst.
  Sterker / nog dan dat woordveld ..."). Eén keer is aanvaardbaar, maar het is precies de door de norm
  verboden opener; schrap of vervang door "Belangrijker nog".
- **"Precies dat ..."**: niet als kale opener, wel 3x mid-zins ("precies dat feest/genre/register",
  whiteboard 557, 914, 1349). Licht.
- **Concessie-sjabloon "Drie/Twee eerlijke grenzen" + "Ik overspeel/overdrijf dit niet"**: 15x. Elke
  beurt sluit nagenoeg identiek af. Voorspelbaar.
- **Moderator-slotformule "Geen (enkel) citaat oogde verzonnen; geen ⚠️ onverifieerbaar-markeringen"**:
  letterlijk herhaald per ronde (whiteboard 359, 709, 1065, 1424). Functioneel maar woordelijk
  identiek; varieer of comprimeer.
- **"stramien"** (eindrapport 2x) en **"oscilleerden in een vast ritme"** (eindrapport 56): nette
  beelden, maar gestapeld met de rest van de metaforiek.

## 4. Neerlandicus-observaties (zinsbouw, register, terminologie)

1. **Naamwoordstijl / nominalisaties.** Zware abstracte samenstellingen domineren:
   "theologie-ontwikkeling", "verspreidingsvertraging", "uitstotingsmotief", "gemeenschapstraject",
   "dateringsneutraliteit", "relatieve-chronologie-argument". Dit verstijft de zinnen. Waar mogelijk
   verwerkwoordelijken: "doordat de gemeenschap zich ontwikkelde" i.p.v. "het gemeenschapstraject".
2. **Hyphen-stapelcomposita.** "halachisch-archeologisch bewijs", "retorisch-narratologisch front",
   "Birkat ha-Minim-anker", "oudste-evangelie-pijler", "Antiochus-als-θεὸς-ἐπιφανής-contrast"
   (whiteboard 699). Het laatste is een echte tangconstructie binnen één woord. Splitsen.
3. **Lange, ingebedde zinnen.** Diverse zinnen lopen over 50+ woorden met meerdere bijzinnen en
   tussenwerpsels (bijv. eindrapport 19-31, whiteboard 843-861). Begrijpelijk in een betoog, maar de
   leesbaarheid wint bij opknippen.
4. **Anglicistische werkwoordsvorming.** "counterde", "gehedged", "hedde" zijn Engelse stammen met
   Nederlandse uitgang. Vervang door "pareerde", "dekte in".
5. **Consistentie eigennamen/transliteratie.** "Johannophobie" (Duits, whiteboard 776, 1003) naast
   "Johannophobia" (Engels, whiteboard 187, 812); "Yerushalmi" naast "Jeruzalemse Talmoed";
   "Septuaginta" naast "Septuagint" (whiteboard 539, 1244). Kies per term één vorm.
6. **Informele inslag.** "Grikser" (whiteboard 35) en het kale "Goed." (whiteboard 813) wisselen met
   hoog-academisch register; dat botst stilistisch.
7. **Register sources.md.** Voorbeeldig: korte, consequente velden, geen prozatics. Behoud dit model.

## 5. Top-10 concrete verbeterpunten (geprioriteerd)

1. **Breek het "Mijn nieuwe front is ..."-sjabloon** (15x). Varieer de openers van de opponentbeurten;
   dit is de meest in het oog springende tic.
2. **Dun de strijdmetaforiek uit**, met name "anker/verankeren" (~38x) en "front" (43x); vervang de
   helft door neutrale termen (steunpunt, grondslag, invalshoek).
3. **Vervang de echte anglicismen**: downstream (3x → "ná/stroomafwaarts"), notch (3x → "punt"), skew
   (3x → "vertekening"), knockout (3x → "genadeslag"), gehedged/hedde (→ "ingedekt").
4. **"foundationeel/foundationele" (6x) → "fundamenteel/grondleggend"**; ook in het anders schone
   eindrapport (30, 111).
5. **Harmoniseer "vóór 70"**: kies tussen los "vóór 70" (25x) en gekoppeld "vóór-70" (18x); idem
   "post-85" → overweeg "ná 85" (12x).
6. **Verlaag de frequentie van "neutraliteitsval" (7x) en "kroongetuige" (7x)**; deze zelfgemunte
   labels slijten tot cliché.
7. **Varieer de vaste moderator-slotzin** "Geen citaat oogde verzonnen; geen ⚠️
   onverifieerbaar-markeringen" (4x identiek).
8. **Schrap de verboden opener "Sterker nog"** (whiteboard 274-275) en "het mes terug" (809).
9. **Vervang het wiskundeteken** `≥1` (whiteboard 62) door "minstens één" en splits de zwaarste
   hyphen-composita (bijv. whiteboard 699).
10. **Maak transliteraties consistent** (Johannophobie/-phobia; Septuagint/-a) en haal de informele
    "Grikser" (35) weg.

## 6. Wat al goed gaat

- **Nul gedachtestreepjes.** De hoofdregel is in alle drie de bestanden vlekkeloos nageleefd; ook
  jaartalbereiken (66-70, 85-100) staan correct met koppelteken.
- **Spelling "kristalliseert" met k** is correct toegepast.
- **Geen verboden losse Engelse modewoorden** (marker, timing, case, default, pivot, rubric,
  out-of-the-box, honest, genuine) in de lopende tekst.
- **Broncitaten correct afgezonderd.** Grieks, Latijn en Hebreeuws staan tussen aanhalingstekens of
  cursief; de Engelse `nlm`-queries staan in code/aanhaling en zijn per norm toegestaan.
- **`sources.md` is een modelmatig, consequent logboek**: strakke velden, geen prozatics, eerlijke
  caveats (alleen-in-vertaling, niet-opgehaald, 404's).
- **Inhoudelijke eerlijkheid is stilistisch zichtbaar**: concessies en voorbehouden zijn netjes
  gemarkeerd; dat is precies wat de redactienorm op het punt van eerlijkheid vraagt.
- **`eindrapport.md` leest, op enkele tics na (neutraliteitsval, foundationeel, kroongetuige), als
  verzorgd, vloeiend Nederlands** en is het sterkste prozastuk van de run.
