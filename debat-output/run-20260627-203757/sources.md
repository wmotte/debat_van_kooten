# 📚 Bronnenlog, run run-20260627-203757

Traceerbaar overzicht van elke geraadpleegde bron, zodat nalezers exact kunnen zien welke
commentaar of webpagina achter een claim zit. Dit is het naslagwerk bij het whiteboard:
het whiteboard bevat de argumenten, dit bestand de volledige herkomst.

**Hoe te lezen.** Per ronde en per zijde één blok. Elke bron krijgt een korte regel met de
claim die hij staaft, gevolgd door de herkomst:

- **Bron:** bij een notebook de exacte notebooktitel én de letterlijk uitgevoerde `nlm`-query;
  bij het web de volledige URL.
- **Specifiek:** bij een notebook de met name in het antwoord genoemde commentator(en), het vers,
  en de teruggegeven verwijsnummers of een korte kernzin uit het antwoord. Noemt de notebook geen
  specifieke auteur, schrijf dan `synthese (geen specifieke auteur genoemd)`, niet "in lijn met X".
  Bij het web: auteur/titel van de pagina.
- **Raakt as:** datering | karakter (welke van de twee score-assen het argument raakt).
- **Aard:** primair (antieke/klassieke tekst) | secundair (modern geleerde/commentaar, incl. nlm).
- **Primair nagezien:** ja/nee/n.v.t. (is een secundaire claim over een primaire tekst zelf tegen
  die primaire tekst gecontroleerd? zo ja, welke tekst en wat kwam eruit).
- **Commando:** het exact gedraaide `brontekst`-commando bij een primaire toets (reproduceerbaarheid),
  anders n.v.t.
- **Opgehaald:** ja/nee (is de URL echt geopend of de query echt uitgevoerd?).
- **Type:** grammaticaal | syntactisch | archeologisch | literair | historisch | tekstkritisch.

> Schrijf een naam alleen toe als de bron die naam daadwerkelijk noemt bij die claim. Verzin nooit
> een toeschrijving, query of verwijsnummer.

<!-- BRONNEN-HIERONDER, append per ronde -->

## Ronde 1

### ⏳ Vroeg
- **Claim:** Naamfrequenties in Johannes komen overeen met pre-70 Palestijns-joods naamgebruik en wijken af van de diaspora; verankert de herkomst van de stof vóór 70 en ondergraaft het late-diaspora-model.
  - **Bron:** nlm "John - exegesis", query: `Does the Gospel of John show accurate pre-70 Palestinian Jewish personal-name frequencies (onomastics, Bauckham, Tal Ilan), and what does the naming and disambiguation of named figures imply for the date of composition?` ; plus web: https://biblicalscholarship.wordpress.com/2008/07/07/a-summary-of-chapter-4-of-richard-bauckhams-jesus-and-the-eyewitnesses/
  - **Specifiek:** Richard Bauckham (op grond van Tal Ilan, *Lexicon of Jewish Names in Late Antiquity*, deel I Palestina 330 v.Chr.-200 n.Chr.) [verwijsnrs 1-6]; kritiek Ruth Edwards [7-8] over tijdspanne en diaspora-ruis; "protective anonymity" (Theissen/Bauckham) [9-13] wordt door Bauckham voor een iets latere datum ingezet. Verssamenhang: Joh 11-12 (Lazarus, Maria, Martha), 18:10 (Malchus).
  - **Raakt as:** datering · **Aard:** secundair · **Primair nagezien:** nee (Tal Ilans dataset niet via brontekst beschikbaar)
  - **Commando:** n.v.t.
  - **Opgehaald:** ja · **Type:** historisch
- **Claim:** Post-70 auteur Josephus beschrijft de verwoeste tempel in verleden tijd (ἦν / ἵδρυτο); dient als controlegeval dat het praesens *estin* in Joh 5:2 presentisch weegt, niet louter stilistisch.
  - **Bron:** brontekst perseus, Flavius Josephus, *Bellum Judaicum* 5.184
  - **Specifiek:** Griekse tekst BJ 5.184: "Τὸ δʼ ἱερὸν ἵδρυτο μέν ... τὰ γὰρ πέριξ ἀπόκρημνος ἦν καὶ κατάντης." Verleden tijd voor de niet meer bestaande tempel.
  - **Raakt as:** datering · **Aard:** primair · **Primair nagezien:** ja (Josephus BJ 5.184 via Perseus TEI; verleden tijd bevestigd)
  - **Commando:** `brontekst perseus "urn:cts:greekLit:tlg0526.tlg004.perseus-grc2:5.184"`
  - **Opgehaald:** ja · **Type:** grammaticaal

### 🕰️ Laat
- **Claim:** Een post-70 auteur (1 Clemens, circa 96 n.Chr.) beschrijft de verdwenen tempelcultus in het praesens; daarmee is het praesens *estin* in Joh 5:2 geen dwingend bewijs voor een datum vóór 70.
  - **Bron:** brontekst perseus, 1 Clemens (Epistula ad Corinthios I) 41 ; aanvullend web: https://jimmyakin.com/2015/01/references-to-the-temple-operating-after-a-d-70.html
  - **Specifiek:** Griekse tekst 1 Clem 41:2: "οὐ πανταχοῦ, ἀδελφοί, προσφέρονται θυσίαι ... ἀλλ' ἢ ἐν Ἱερουσαλὴμ μόνῃ· κἀκεῖ δὲ οὐκ ἐν παντὶ τόπῳ προσφέρεται". Tegenwoordige tijd voor de na 70 niet meer bestaande tempeldienst. Gangbare datering circa 95-96; minderheid (Carrier) dateert vroeger (eerlijk gemarkeerd).
  - **Raakt as:** datering · **Aard:** primair · **Primair nagezien:** ja (1 Clemens 41 via Perseus/First1KGreek TEI; praesens προσφέρονται/προσφέρεται bevestigd)
  - **Commando:** `brontekst perseus "urn:cts:greekLit:tlg1271.tlg001.1st1K-grc1:41"`
  - **Opgehaald:** ja · **Type:** grammaticaal
- **Claim:** Johannes vooronderstelt de synoptici en is literair later (rond 90-100); de "kleine overeenkomsten" die Van Kooten voor Lukan posteriority gebruikt, zijn omkeerbaar en passen bij Johannes die Lucas/Marcus herschrijft.
  - **Bron:** nlm "John - exegesis", query: `What is the strongest internal evidence that John knew and used the Synoptic Gospels (Mark and Luke), and that John is therefore literarily later than them? Cite Barrett, Neirynck, or others on Johannine knowledge of the Synoptics and what it implies for relative dating.`
  - **Specifiek:** Frans Neirynck (Leuvense school) [10],[15],[16],[17],[18]: Joh 21:1-14 als herschrijving van Lucas 5:1-11; gedeelde minor agreements met Lucas (Martha, Annas/Lazarus, rechteroor, Pilatus' drievoudige onschuldverklaring). C.K. Barrett [11],[12],[13],[14]: zeldzame gedeelde details (tweehonderd denariën Mc 6:37/Joh 6:7; *pistikos* en driehonderd denariën Mc 14:3-5/Joh 12:3-5). Implicatie voor datering [19]-[23]: eindcompositie 90-100 n.Chr.
  - **Raakt as:** datering · **Aard:** secundair · **Primair nagezien:** n.v.t.
  - **Commando:** n.v.t.
  - **Opgehaald:** ja · **Type:** literair

### 🏛️ Grieks-Romeins
- **Claim:** Johannes' herkenningsscènes (Maria bij het graf, blindgeborene, Thomas) volgen structureel Aristoteles' *anagnorisis* (omslag van onwetendheid naar kennis) samengevoegd met *peripeteia*; samen met dramatische ironie (vgl. Sophocles), de toneelenscenering en de *bios*-genrebepaling maakt dit het culturele eindkarakter Grieks-Romeins.
  - **Bron:** nlm "John - exegesis", query: `To what extent do scholars read the recognition scenes in John (the man born blind in ch.9, Mary Magdalene at the tomb in ch.20, Thomas) as Greek-style anagnorisis/recognition drama in the sense of Aristotle's Poetics? Cite Kasper Bro Larsen or others on John as Greek drama, dramatic irony, and the bios genre (Burridge).` ; plus primaire tekst Aristoteles *Poetica* 11.4-11.5 via brontekst perseus ; plus web: https://www.mdpi.com/2077-1444/17/6/702
  - **Specifiek:** Richard Burridge [1],[2] (*bios*-genre); Jo-Ann Brant en George Parsenios [4],[5],[6] (Johannes geënt op klassiek Grieks theater); David Wead en Paul Duke [8],[9],[10] (johanneïsche ironie vergeleken met Sophocles, voortbouwend op Connop Thirlwall); Kasper Bro Larsen [16],[17],[18] (*Recognizing the Stranger: Recognition Scenes in the Gospel of John*, Brill 2008; type-scène: ontmoeting, uitstel, herkenningsteken, omslag, reactie); toepassingen op Joh 20:14-16 (Maria, "Mariam"/"Rabbouni") [19],[20],[21], Joh 20:28 (Thomas) [22],[23],[24], Joh 9 (blindgeborene, trapsgewijze herkenning) [25]-[31]. Web: MDPI *Religions* 2025/2026, "Johannine Anagnorisis: Current Scholarship and Future Perspectives" (overzichtsartikel, bevestigt lopend onderzoeksveld). Primaire tekst: *Poetica* 11.4 "ἀναγνώρισις δέ ... ἐξ ἀγνοίας εἰς γνῶσιν μεταβολή"; 11.5 "καλλίστη δὲ ἀναγνώρισις, ὅταν ἅμα περιπετείᾳ γένηται".
  - **Raakt as:** karakter · **Aard:** primair en secundair · **Primair nagezien:** ja (Aristoteles *Poetica* 11.4 en 11.5 via Perseus TEI; definitie van *anagnorisis* als omslag onwetendheid→kennis en de koppeling met *peripeteia* letterlijk bevestigd)
  - **Commando:** `./.agents/tools/brontekst perseus "urn:cts:greekLit:tlg0086.tlg034.perseus-grc2:11.4"` en `... :11.5`
  - **Opgehaald:** ja · **Type:** literair en filosofisch

### ✡️ Joods
- **Claim:** De johanneïsche herkenningsclimaxen draaien om het absolute *egō eimi*, de LXX-weergave van het goddelijke *ani hu* (Jes 43:10; Deut 32:39); de onderliggende "dan zul je weten dat Ik het ben"-structuur is de profetische herkenningsformule (Ezechiël ~60x), niet Aristoteles' *anagnorisis*. Daarmee is de "omslag van onwetendheid naar kennis" een joods-theologisch schema, geen Grieks plotmechanisme.
  - **Bron:** nlm "John - exegesis", query 1: `How do scholars relate the Johannine ego eimi (I am) sayings and recognition scenes to the Hebrew Bible, especially Deutero-Isaiah's ani hu / 'that you may know that I am he' (Isaiah 43:10) and the Joseph recognition narrative (Genesis 45 'I am Joseph')? Is John's recognition language rooted in Jewish divine self-revelation rather than only Greek anagnorisis?` ; query 2: `On John 8:28, 8:24, 13:19 and the ego eimi sayings: which commentators (e.g. Brown, Catrin Williams, Ball, Bauckham) argue the absolute 'I am' derives from Deutero-Isaiah ani hu and Deut 32:39, and that the Ezekiel recognition formula 'then you will know that I am Yahweh' underlies John? Name the scholars.` ; plus primaire teksten via brontekst sefaria.
  - **Specifiek:** D.A. Carson [9] (Jes 40-55 en Deut 32:39 als achtergrond van Joh 8:24,28,58; *ani hu* op zichzelf toegepast = volle godheidsclaim); Marianne Meye Thompson [10,11] (parallel Jes 43:10 met Joh 8:24,28; 13:19); Paul A. Rainbow, Raymond E. Brown, Johannes Beutler, Gerard Sloyan [1,4,12,13] (*egō eimi* terug naar *ani hu* van Deutero-Jesaja en Deut); Brian Neil Peterson [14-17] en Hassell Bullock [18] (Ezechiël-herkenningsformule "dan zul je weten dat Ik JHWH ben", ~60x, achter Joh 8:28); Brown [19] (OT-formule Ex 6:7 als parallel). Verssamenhang Joh 8:28; 18:5-6; 9:9. Primaire toets: Jes 43:10 MT "כִּי־אֲנִי הוּא ... לְמַעַן תֵּדְעוּ וְתַאֲמִינוּ" en Deut 32:39 "אֲנִי אֲנִי הוּא" bevestigd.
  - **Raakt as:** karakter · **Aard:** primair en secundair · **Primair nagezien:** ja (Jes 43:10 en Deut 32:39 via Sefaria; *ani hu* en de "opdat jullie weten"-structuur letterlijk aanwezig)
  - **Commando:** `./.agents/tools/brontekst sefaria "Isaiah 43:10"` en `./.agents/tools/brontekst sefaria "Deuteronomy 32:39"`
  - **Opgehaald:** ja · **Type:** exegetisch en literair
- **Claim:** Het "menselijke" zelfidentificatie-gebruik van *egō eimi* (blindgeborene "ik ben het", Joh 9:9) heeft zijn premier-voorbeeld in Gen 45:3-4, Jozef "Ik ben Jozef" (*ani Yosef*, LXX *egō eimi*); herkenning-door-zelfonthulling is ook in narratieve vorm een Hebreeuws-bijbels type-scène.
  - **Bron:** primaire tekst Gen 45:3-4 via brontekst sefaria; plus nlm "John - exegesis" (zelfde query 1 hierboven: vermelding LXX *egō eimi* voor Gen 45:4 en Bultmanns *Rekognitionsformel*-classificatie).
  - **Specifiek:** Rudolf Bultmann [13,14] (*egō eimi* als *Rekognitionsformel*, "Wie ben jij?"); Gen 45:4 LXX *egō eimi* genoemd [15]; toepassing op Joh 9:9 [15,16]. Primaire toets: Gen 45:3 "אֲנִי יוֹסֵף" en 45:4 "אֲנִי יוֹסֵף אֲחִיכֶם" bevestigd in MT (Sefaria).
  - **Raakt as:** karakter · **Aard:** primair en secundair · **Primair nagezien:** ja (Gen 45:3-4 via Sefaria; *ani Yosef* / "Ik ben Jozef" bevestigd)
  - **Commando:** `./.agents/tools/brontekst sefaria "Genesis 45:3"` en `./.agents/tools/brontekst sefaria "Genesis 45:4"`
  - **Opgehaald:** ja · **Type:** literair en exegetisch

### ⚖️ Moderator (verificatie)
- **Bron bestaat / lezing klopt?** Laats scharnierclaim, 1 Clemens 41:2 gebruikt het praesens voor de na 70 verdwenen offercultus → bevestigd tegen de primaire tekst: προσφέρονται en προσφέρεται (en het participium προσφερόμενον) staan letterlijk in 1 Clem 41. De praesensvormen kloppen.
  - **Nuance (gewicht begrensd):** het praesens leest plausibel als gnomisch-beschrijvend van de door de Tora voorgeschreven cultische orde, niet noodzakelijk als bewering dat er ten tijde van schrijven feitelijk geofferd werd; daardoor is het een iets minder exacte tegenhanger van het topografische *estin* over een fysiek bouwwerk in Joh 5:2. Conclusie: het ondergraaft de dwingendheid van het *estin*-argument, maar maakt het niet betekenisloos.
  - **Commando:** `./.agents/tools/brontekst perseus "urn:cts:greekLit:tlg1271.tlg001.1st1K-grc1:41"`
- **Controle Vroeg-comparandum:** Josephus *BJ* 5.184 gebruikt verleden tijd voor de verwoeste tempel → bevestigd: ἵδρυτο (plusquamperfectum) en ἦν (imperfectum) staan er.
  - **Commando:** `./.agents/tools/brontekst perseus "urn:cts:greekLit:tlg0526.tlg004.perseus-grc2:5.184"`
- **Overige citaten:** geen `⚠️ onverifieerbaar`-markeringen deze ronde; de web- en notebookverwijzingen zijn concreet en navolgbaar.

## Ronde 2

### ⏳ Vroeg
- **Claim:** Johannes gebruikt voor plaatsen gewoonlijk de imperfectum ἦν ("was") (Joh 11:18 Betanië, 18:1 hof, 19:41 hof), maar uitgerekend bij het bad Betzata het praesens ἔστιν (Joh 5:2); dit interne tijdsvormcontrast weerlegt het bezwaar dat ἔστιν "slechts een historisch praesens" is en wijst presentisch op een nog bestaand bouwwerk (vóór 70).
  - **Bron:** nlm "John - exegesis", query: `Does the Gospel of John use the imperfect (ēn, 'was') for topographical/place descriptions elsewhere (e.g. John 11:18 Bethany 'was' near Jerusalem; John 18:1 'there was a garden'; John 19:41 'there was a garden in the place'), in contrast to the present estin in John 5:2 ('there is in Jerusalem a pool')? Do commentators note this internal contrast and argue that John's normal habit is past tense for places, making the present estin in 5:2 marked/deliberate and best explained if the pool still stood (before 70)? Name scholars (Morris, Carson, Westcott, Robinson, Barrett).` ; plus grondtekst via biblehub: https://biblehub.com/text/john/11-18.htm , https://biblehub.com/text/john/18-1.htm , https://biblehub.com/text/john/19-41.htm
  - **Specifiek:** Leon Morris [3],[5] (contrast in Johannes' tijdsvormen; ἦν in 18:1 wijst op reeds verwoeste hof, ἔστιν in 5:2 "most natural reading points to a pool in existence at the time"); J.A.T. Robinson [7],[8] (ἔστιν als argument voor compositie vóór de Joodse Oorlog); Daniel Wallace [7],[9] (εἰμί nergens anders in het NT als historisch praesens); tegenstem D.A. Carson [6] ("would be conclusive were it not for" Johannes' frequente historisch praesens), Westcott [10] en Barrett (late consensus); aanvulling [8],[12],[13] (baden mogelijk voortbestaand als pagaan Asclep-heiligdom). Verssamenhang Joh 5:2; 11:18; 18:1; 19:41.
  - **Raakt as:** datering · **Aard:** primair en secundair · **Primair nagezien:** ja (Joh 11:18 ἦν, 18:1 ἦν, 19:41 ἦν via biblehub/NA28 bevestigd als imperfectum; tegenover ἔστιν in 5:2)
  - **Commando:** n.v.t. (NT via biblehub; brontekst dekt het NT niet), https://biblehub.com/text/john/11-18.htm ; https://biblehub.com/text/john/18-1.htm ; https://biblehub.com/text/john/19-41.htm
  - **Opgehaald:** ja · **Type:** grammaticaal en syntactisch
- **Claim:** De door Laat als laat ingezette epiloog bevat zelf een aanwijzing voor een nog levende getuige: Joh 21:24 koppelt het praesens-participium ὁ μαρτυρῶν ("die getuigt") en ἐστιν aan de aoristus ὁ γράψας ("die schreef"); de natuurlijke lezing is een ooggetuige die nog leefde bij de eindredactie, wat de datering vroeg trekt.
  - **Bron:** nlm "John - exegesis", query: `On John 21:23-24: can the correction of the rumor that the beloved disciple would not die be read as written while the disciple was still alive but very old (rather than after his death)? And does the present participle 'ho marturōn' (the one who IS bearing witness) in 21:24, together with 'houtos estin' (this IS the disciple), suggest the witness was still living when this was written? Name commentators who argue John 21 supports an early or first-century date and that the appendix at most dates the final certification, not chapters 1-20.` ; plus grondtekst via biblehub: https://biblehub.com/text/john/21-24.htm
  - **Specifiek:** Andreas Köstenberger en D.A. Carson [8] (praesens-participium "who is testifying" = leerling onmiskenbaar nog in leven bij het schrijven); Leon Morris [9] (praesens "not easy to fit ... to the hypothesis that he had died"); William Hendriksen [10] (twee tijden = twee ideeën: nog mondeling getuigend, recent geschreven); tegenstem Raymond Brown en Francis Moloney [11-13] (praesens vereist geen levende getuige; getuigenis "leeft voort"); voor 21:23 als levende-leerling-lezing: Morris [1], F.F. Bruce [2-4], Carson [5], Hendriksen [6], met ook Westcott, Zahn, Bernard, Hoskyns [7]; Westcott [20-22] (epiloog door dezelfde hand, alleen 21:24-certificering door de oudsten toegevoegd; kerntradities vroeg); Robinson [16] (correctie 21:23 logisch kort na de marteldood van Petrus, circa 65). Verssamenhang Joh 21:23-24. Primaire toets: 21:24 ἐστιν (praesens ind.), ὁ μαρτυρῶν (praesens participium), ὁ γράψας (aoristus participium) bevestigd.
  - **Raakt as:** datering · **Aard:** primair en secundair · **Primair nagezien:** ja (Joh 21:24 via biblehub/NA28; μαρτυρῶν praesens participium, ἐστιν praesens, γράψας aoristus bevestigd)
  - **Commando:** n.v.t. (NT via biblehub; brontekst dekt het NT niet), https://biblehub.com/text/john/21-24.htm
  - **Opgehaald:** ja · **Type:** grammaticaal en syntactisch

### ✡️ Joods
- **Claim:** Joh 7:37-38 ("stromen van levend water", laatste grote dag) en Joh 8:12 ("licht van de wereld", vrouwenvoorhof) veronderstellen de Soekot-tempelliturgie: waterlibatie *nisuch ha-mayim* en nachtelijke verlichting van de voorhoven, alleen bewaard in joodse bronnen.
  - **Bron:** nlm "John - exegesis", query: `How do commentators connect John 7:37-39 ('rivers of living water', the last great day of the feast) and John 8:12 ('I am the light of the world') to the Sukkot Temple liturgy: the water-libation ceremony (nisuch ha-mayim / Simchat Beit ha-Sho'evah) and the nightly illumination of the Temple court described in Mishnah Sukkah? Name scholars (Brown, Beasley-Murray, Keener, Hoskyns, Yee) who argue John's symbolism presupposes this specifically Jewish festival ritual.` ; plus primaire teksten Misjna Soekka 4:9, 5:1, 5:3 via brontekst sefaria.
  - **Specifiek:** George Beasley-Murray [4],[5],[14] (procession naar Siloam, gouden kruik, Waterpoort; vier gouden kandelaars en de pitten van priestergordels); Craig Keener [6] (waterritueel verbonden met gebed om herfstregens); Raymond Brown [11],[12],[18],[19],[20] (eschatologische rivieren uit Jezus als nieuwe tempel; Joh 8:12 in de schatkamer in de vrouwenvoorhof waar de lampen brandden); E.C. Hoskyns [13] (christologische lezing van 7:38); Gale Yee [17],[23],[24] (lampenlicht als Gods licht; Jezus vervangt de liturgische instituties). Verssamenhang Joh 7:37-39; 8:12. Primaire toets: Soekka 4:9 (נסוך המים, gouden kruik van 3 log uit de Siloam, Waterpoort), 5:1 (שמחת בית השואבה), 5:3 (geen voorhof in Jeruzalem onverlicht) bevestigd.
  - **Raakt as:** karakter · **Aard:** primair en secundair · **Primair nagezien:** ja (Misjna Soekka 4:9, 5:1, 5:3 via Sefaria; waterlibatie en verlichting letterlijk aanwezig)
  - **Commando:** `./.agents/tools/brontekst sefaria "Mishnah Sukkah 4:9"` ; `./.agents/tools/brontekst sefaria "Mishnah Sukkah 5:1"` ; `./.agents/tools/brontekst sefaria "Mishnah Sukkah 5:3"`
  - **Opgehaald:** ja · **Type:** liturgisch en exegetisch
- **Claim:** Joh 7:22-23 is een *qal wachomer* (van licht naar zwaar), de eerste van Hillels zeven *middot*; vrijwel dezelfde redenering staat op naam van R. Elazar ben Azarja in b. Yoma 85b, waar de term קל וחומר letterlijk valt. De discoursvorm van Johannes is rabbijns-halachisch.
  - **Bron:** nlm "John - exegesis", query: `In John 7:22-23 Jesus argues that if circumcision is performed on the Sabbath so the law of Moses is not broken, then healing a whole man on the Sabbath is permitted. Do commentators identify this as a rabbinic qal wahomer (a fortiori, 'light and heavy') argument, one of Hillel's seven middot / rules of exegesis, and as evidence that the Johannine Jesus debates like a Jewish rabbi using halakhic reasoning? Name scholars (Brown, Keener, Daube, Dodd, Lincoln).` ; plus primaire tekst b. Yoma 85b via brontekst sefaria.
  - **Specifiek:** Charles Puskas [2] (eerste van Hillels zeven *middot*); Raymond Brown [6],[8] (*a minori ad maius*, "quite common in rabbinic logic"); C.H. Dodd [12] (intieme bekendheid met rabbijnse methoden); David Daube [21] (*The New Testament and Rabbinic Judaism*); Andrew Lincoln [22]-[26] ("lawsuit"-motief); Urban von Wahlde [3],[13],[27] (verankert Jezus in authentieke joodse rechtscontext); parallel b. Yoma 85b (R. Elazar ben Azarja) [11],[14]-[17]. Verssamenhang Joh 7:22-23. Primaire toets: b. Yoma 85b bevat קל וחומר letterlijk, met besnijdenis als "één van 248 ledematen" versus het hele lichaam.
  - **Raakt as:** karakter · **Aard:** primair en secundair · **Primair nagezien:** ja (b. Yoma 85b via Sefaria; קל וחומר en het besnijdenis-argument bevestigd)
  - **Commando:** `./.agents/tools/brontekst sefaria "Yoma 85b"`
  - **Opgehaald:** ja · **Type:** exegetisch en literair

### 🕰️ Laat
- **Claim:** Joh 21 is een latere redactionele epiloog; Joh 21:23 (correctie van het gerucht dat de geliefde leerling niet zou sterven) veronderstelt diens reeds ingetreden dood en Joh 21:24 ("wij weten", οἴδαμεν) is de stem van een redactiekring; de eindvorm dateert ná de ooggetuige-generatie, rond 90-100.
  - **Bron:** nlm "John - exegesis", query: `Is John 21 a later redactional appendix added by an editorial circle after the death of the Beloved Disciple? How do commentators read John 21:23 (the rumor that the disciple would not die, corrected because he had died) and John 21:24 ('we know that his testimony is true') as evidence that the final form of the Gospel postdates the founding eyewitness generation, implying a date in the 90s or later? Name scholars (Brown, Bultmann, Schnackenburg, Lindars, Barrett).` ; plus primaire teksten Joh 21:23 en 21:24 via biblehub/NA28
  - **Specifiek:** Rudolf Bultmann [29],[30],[31] (hfst. 21 "incontestably" een tweede hand / kerkelijke redacteur; dood van de leerling als bewijs van posthume redactie); Raymond E. Brown [15],[22],[25],[32],[33] (meertraps-compositie; finale redacteur voegt hfst. 21 toe; parousie-crisis; "wij" van 21:24 = redactiekring); C.K. Barrett [34],[35] ("wij" als stem van de apostolische kerk); Barnabas Lindars en Rudolf Schnackenburg [36]-[40] (epiloog/supplement door redacteur binnen de johanneïsche school); dateringsimplicatie 90-100 [26],[27],[7],[23],[28]. Primaire toets: Joh 21:23 "ὁ μαθητὴς ἐκεῖνος οὐκ ἀποθνήσκει"; Joh 21:24 "καὶ οἴδαμεν ὅτι ἀληθὴς αὐτοῦ ἡ μαρτυρία ἐστίν" (οἴδαμεν = perfectum indicatief actief 1e p. mv.).
  - **Raakt as:** datering · **Aard:** primair en secundair · **Primair nagezien:** ja (Joh 21:23-24 via biblehub/NA28; οὐκ ἀποθνήσκει en οἴδαμεν letterlijk bevestigd)
  - **Commando:** n.v.t. (NT via biblehub; brontekst dekt het NT niet), https://biblehub.com/text/john/21-23.htm en https://biblehub.com/text/john/21-24.htm
  - **Opgehaald:** ja · **Type:** literair en grammaticaal
- **Claim:** P52 legt geen vroege datum vast; paleografisch lijkende handen komen tot circa 152 n.Chr. voor, dus de *terminus ante quem* verruimt en is verenigbaar met een compositie in de jaren 90-100.
  - **Bron:** https://www.cambridge.org/core/journals/harvard-theological-review/article/abs/use-and-abuse-of-p52-papyrological-pitfalls-in-the-dating-of-the-fourth-gospel/676A4EA909EB03046F89DB8CE1F050BE (via WebSearch-samenvatting)
  - **Specifiek:** Brent Nongbri, "The Use and Abuse of P52: Papyrological Pitfalls in the Dating of the Fourth Gospel," *Harvard Theological Review* 98, no. 1 (2005): 23-48. Paleografische datering is circulair; handen vergelijkbaar met P52 gedateerd tot 152 n.Chr.; P52 kan decennia jonger of een eeuw ouder zijn; P52 alleen bewijst niet het bestaan van Johannes in de vroege 2e eeuw.
  - **Raakt as:** datering · **Aard:** secundair · **Primair nagezien:** n.v.t. (papyrologische/paleografische claim, geen tekstlezing om te toetsen)
  - **Commando:** n.v.t.
  - **Opgehaald:** ja · **Type:** tekstkritisch en historisch

### 🏛️ Grieks-Romeins
- **Claim:** De gepredikte egō-eimi-uitspraken (Joh 6:35; 8:12; 10:7,11; 15:1) delen hun literaire vorm met de hellenistisch-Egyptische Isis-aretalogie en de Hermetische openbaringstaal; dit verklaart de kosmische zelfpredicatie "het licht van de wereld" beter dan de Soekot-liturgie de literaire vorm doet.
  - **Bron:** nlm "John - exegesis", query: `Do commentators compare the Johannine 'I am' (ego eimi) self-predications, especially the predicate ones (I am the bread of life, the light of the world, the good shepherd, the true vine), to the Hellenistic-Egyptian Isis aretalogies ('I am Isis...') and Greco-Oriental revelatory self-predication (Offenbarungsrede)? Name scholars such as Bultmann, Dodd, Eduard Norden, or Catrin Williams who set the I-am form against this Hellenistic religious background.`
  - **Specifiek:** Rudolf Bultmann [1,4,5,6] (Offenbarungsreden als bron; Isis-spreuken als "identificatieformule", incipit "I am all that has been..."); Eduard Schweizer [6,7]; Eduard Norden *Agnostos Theos* en G.P. Wetter [8,9] (oosters-hellenistische herkomst van de formule); George W. MacRae en Jan Bergman [3] (Isis-aretalogie als achtergrond van de gepredikte johanneïsche "Ik ben"); C.H. Dodd [12,13,14] (Corpus Hermeticum; "the messenger of light am I"; licht/leven/waarheid wijdverbreid in de 1e-eeuwse hellenistische wereld). Tegenstem (eerlijk genoteerd): Catrin Williams en David Mark Ball [15,16] en Heinrich Zimmermann [9] (voor het absolute egō eimi, Joh 8:58, is ani hoe/Deutero-Jesaja bepalend; heidense parallellen voor het absolute gebruik schaars). Verssamenhang Joh 6:35; 8:12; 10:7,11; 15:1.
  - **Raakt as:** karakter · **Aard:** secundair · **Primair nagezien:** nee (Isis-aretalogie via Diodorus Siculus 1.27 niet beschikbaar in canonical-greekLit/First1KGreek, ophalen gaf 404; de nlm-output citeert het incipit en noemt de geleerden)
  - **Commando:** `./.agents/tools/brontekst perseus "urn:cts:greekLit:tlg0060.tlg001.perseus-grc2:1.27.4"` (mislukt, 404), n.v.t. als geslaagde toets
  - **Opgehaald:** ja (nlm-query uitgevoerd) · **Type:** literair en filosofisch
- **Claim:** Het argument a fortiori (qal wachomer) is geen distinctief joodse vorm maar een gemeenschappelijke Griekse retorische topos; Aristoteles, Rhetorica 2.23.4, "ἐκ τοῦ μᾶλλον καὶ ἧττον". De redeneervorm van Joh 7:22-23 bewijst dus geen joods eindkarakter.
  - **Bron:** brontekst perseus, Aristoteles, *Rhetorica* 2.23.4
  - **Specifiek:** Griekse tekst Rhet. 2.23.4: "ἄλλος ἐκ τοῦ μᾶλλον καὶ ἧττον, οἷον εἰ μηδʼ οἱ θεοὶ πάντα ἴσασιν, σχολῇ οἵ γε ἄνθρωποι ...". De koinos topos "uit het meer en het minder" (a fortiori) staat letterlijk als Griekse retorische gemeenplaats, vóór Hillel en los van de halacha. Aanvullend: Raymond Brown benoemt de johanneïsche figuur als "a minori ad maius" (Latijnse, niet rabbijnse term), zie ronde-1/2-vermelding in nlm "John - exegesis".
  - **Raakt as:** karakter · **Aard:** primair · **Primair nagezien:** ja (Aristoteles *Rhetorica* 2.23.4 via Perseus TEI; topos ἐκ τοῦ μᾶλλον καὶ ἧττον letterlijk bevestigd)
  - **Commando:** `./.agents/tools/brontekst perseus "urn:cts:greekLit:tlg0086.tlg038.perseus-grc2:2.23.4"`
  - **Opgehaald:** ja · **Type:** retorisch en filosofisch

### ⚖️ Moderator (verificatie)
- **Scharnierende toetsing, qal wachomer tegen beide primaire teksten.** De karakter-as draaide deze ronde om de vraag of de a-fortiori-redenering van Joh 7:22-23 distinctief joods (Joods) of een gedeelde Griekse topos (Grieks-Romeins) is. Ik legde beide kanten tegen de tekst.
  - **Griekse kant bevestigd:** Aristoteles *Rhetorica* 2.23.4 bevat de topos "ἄλλος ἐκ τοῦ μᾶλλον καὶ ἧττον" letterlijk, met het voorbeeld "εἰ μηδʼ οἱ θεοὶ πάντα ἴσασιν, σχολῇ οἵ γε ἄνθρωποι" (als zelfs de goden niet alles weten, dan de mensen al helemaal niet). De a-fortiori-figuur is dus een gecodificeerde Griekse gemeenplaats, los van de halacha.
  - **Commando:** `./.agents/tools/brontekst perseus "urn:cts:greekLit:tlg0086.tlg038.perseus-grc2:2.23.4"`
  - **Joodse kant bevestigd:** b. Yoma 85b bevat קל וחומר letterlijk, met R. Elazar ben Azarja: "וּמָה מִילָה שֶׁהִיא אֶחָד מִמָּאתַיִם וְאַרְבָּעִים וּשְׁמוֹנָה אֵיבָרִים ... קַל וָחוֹמֶר לְכׇל גּוּפוֹ" (zoals de besnijdenis, één van de 248 ledematen, de sabbat opzij zet, des te meer de redding van het hele lichaam). De halachische toepassing op Tora-geboden staat er als geclaimd.
  - **Commando:** `./.agents/tools/brontekst sefaria "Yoma 85b"`
  - **Uitkomst:** het twistpunt is tweesnijdend. De kale logische vorm is gedeeld en niet joods-exclusief; de codificatie onder de middot en de toepassing op Tora-recht is wél joods. Geen van beide polen wint dit sub-argument; het gewicht ervan op de karakter-as is grotendeels neutraal, wat de erkende Soekot-liturgie tot de doorslaggevende joodse bijdrage van de ronde maakt.
- **Overige citaten:** geen `⚠️ onverifieerbaar`-markeringen. Wel weegt het Isis-aretalogie-argument van Grieks-Romeins lichter omdat de primaire Isis-tekst (Diodorus 1.27) deze ronde niet kon worden opgehaald (404 in de Perseus-repo); het is een echte, klassieke secundaire positie (Bultmann, Norden, Wetter, MacRae, Bergman, Dodd), maar dit keer niet primair getoetst.

## Ronde 3

### ⏳ Vroeg
- **Claim:** Uitblijven van een vervullingsglosse bij Joh 11:48 (τόπος = tempel) op de redactionele laag, vergeleken met de synoptische vaticinia ex eventu (Mt 22:7; Lc 19:43-44; 21:20), als aanwijzing voor een datum vóór 70.
  - **Bron:** nlm "John - exegesis", query: `Does John 11:48 'the Romans will come and take away both our place (ton topon) and our nation' refer to the temple, and how do commentators weigh John's lack of any explicit reference to the fulfilled destruction of Jerusalem in AD 70, compared with the redactional fulfilment glosses in Matthew 22:7 and Luke 19:43-44 and 21:20-24, as an argument bearing on the date of John before or after 70?` ; plus NT-grondtekst via biblehub/NA28.
  - **Specifiek:** pro-vroeg J.A.T. Robinson [12], Leon Morris, W.F. Albright [10-11] ("een van de sterkste bewijzen voor een datum vóór 70"; Robinson: John is het boek waar een verwijzing naar de val het meest verwacht zou zijn); τόπος als tempel: J. Ramsey Michaels, Adolf Schlatter, Walter Bauer, Arthur W. Pink [1-4]; tegenstem D.A. Carson, Craig Blomberg [13-15], B.F. Westcott [17-20] (replacement-theologie Joh 2:19-21), D. Moody Smith en Robert Fortna [4, 21-22] (voorspelling-na-de-feiten). Verteller-glossen Joh 2:21-22 genoemd door Robinson/Morris [12].
  - **Raakt as:** datering · **Aard:** primair en secundair · **Primair nagezien:** ja (NT-grondtekst Joh 11:48; 11:51-52; 2:21-22; Mt 22:7; Lc 19:43-44; 21:20 via biblehub/NA28 interlinear; τὸν τόπον staat in 11:48, de glosse in 11:51-52 is uitsluitend christologisch, de synoptische siege-glossen staan als geciteerd)
  - **Commando:** n.v.t. (NT zit niet in brontekst; biblehub/NA28 geraadpleegd)
  - **Opgehaald:** ja · **Type:** literair en grammaticaal
- **Claim:** Lucas gebruikt Josephus (Theudas + Judas de Galileeër/census, Hand 5:36-37 versus *Ant.* 20.97-102), dus Lucas ná 93; dat versterkt de relatieve ordening Johannes vóór Lucas (pijler 3) en ontkracht Neiryncks Johannes-herschrijft-Lucas.
  - **Bron:** brontekst perseus, Josephus *Antiquitates* 20.97 en 20.102; argument toegeschreven aan Steve Mason; NT Hand 5:36-37 via biblehub/NA28.
  - **Specifiek:** *Ant.* 20.97 "γόης τις ἀνὴρ Θευδᾶς ὀνόματι" onder procurator Fadus; 20.102 "οἱ παῖδες Ἰούδα τοῦ Γαλιλαίου ... Κυρινίου τῆς Ἰουδαίας τιμητεύοντος" (zonen van Judas de Galileeër, census onder Quirinius). Dezelfde twee figuren, gekoppeld, in dezelfde volgorde als Hand 5:36-37. Mason: Lucas put uit *Antiquitates* (verschenen 93-94).
  - **Raakt as:** datering · **Aard:** primair · **Primair nagezien:** ja (beide Josephus-passages opgehaald; Griekse tekst bevestigt Θευδᾶς in 20.97 en Ἰούδα τοῦ Γαλιλαίου + Κυρινίου in 20.102)
  - **Commando:** `./.agents/tools/brontekst perseus "urn:cts:greekLit:tlg0526.tlg001.perseus-grc2:20.97"` en `./.agents/tools/brontekst perseus "urn:cts:greekLit:tlg0526.tlg001.perseus-grc2:20.102"`
  - **Opgehaald:** ja · **Type:** literair en historisch

### 🕰️ Laat
- **Claim:** De redactionele naad bij Joh 14:31 ("ἐγείρεσθε, ἄγωμεν ἐντεῦθεν") gevolgd door de hoofdstukken 15-17 vóór het werkelijke vertrek in Joh 18:1 toont dat 15-17 een latere invoeging zijn en dat het boek in fasen groeide door een johanneïsche school; de eindvorm dateert 90-100.
  - **Bron:** nlm "John - exegesis", query: `Is the Johannine Farewell Discourse a composite that grew in stages? How do commentators read the seam at John 14:31 ('Rise, let us go from here', egeiresthe agōmen enteuthen) followed by chapters 15-17 before they actually depart in 18:1, as evidence that chapters 15-17 are a later insertion and that the Gospel is the product of staged redaction by a Johannine school over time? What does this displacement/aporia imply for the date of the final form? Name scholars (Bultmann, Brown, Schnackenburg, Lindars).` ; plus grondtekst Joh 14:31 en 18:1 via biblehub
  - **Specifiek:** Rudolf Bultmann [20,21,22-27] (oorspronkelijke verplaatsing van bladen; eindvorm door "ecclesiastical redactor"); Raymond E. Brown [16,23,28,29-31] (13:31-14:31 als vroegere uitgave; redacteur voegt 15-17 toe na 14:31 zonder de geografische breuk glad te strijken); Rudolf Schnackenburg [32-35] (opeenvolgende lagen, evoluerende theologie van de school; 15-17 paraenetisch op gemeenschapsoverleving); Barnabas Lindars [31,36-39] (homilieën over een lange periode verzameld); synthese *relecture* [40-43]; dateringsimplicatie eindvorm 90-100 [44-52]. Verssamenhang Joh 14:31; 18:1. Primaire toets: Joh 14:31 "ἐγείρεσθε, ἄγωμεν ἐντεῦθεν" en Joh 18:1 "ἐξῆλθεν ... πέραν τοῦ χειμάρρου τῶν Κέδρων" bevestigd.
  - **Raakt as:** datering · **Aard:** primair en secundair · **Primair nagezien:** ja (Joh 14:31 en 18:1 via biblehub/NA28; de naad-formule en het latere vertrek bevestigd)
  - **Commando:** n.v.t. (NT via biblehub; brontekst dekt het NT niet), https://biblehub.com/text/john/14-31.htm en https://biblehub.com/text/john/18-1.htm
  - **Opgehaald:** ja · **Type:** literair en grammaticaal
- **Claim:** Johannes verwerkt de tempelval niet door voorspelling maar door vervangingschristologie (Joh 2:19-22 tempel = Jezus' lichaam; Joh 4:21-24 "niet op deze berg en niet in Jeruzalem"), wat het best verklaarbaar is als laat-eerste-eeuws antwoord op het trauma ná 70; Joh 11:48 is prediction-after-the-fact. Dit draait Vroegs stilzwijgen-argument om.
  - **Bron:** nlm "John - exegesis", query: `Does the Gospel of John lack any Olivet/eschatological discourse predicting the temple's destruction (no parallel to Mark 13)? How do commentators explain John's 'silence' about the fall of Jerusalem in AD 70: do they argue John transposed temple-destruction into replacement christology (John 2:19-22 the temple as Jesus' body; John 4:21-24 'neither on this mountain nor in Jerusalem'), and that this replacement theology is most intelligible after 70? Do Moody Smith and Fortna read John 11:48 as a prophecy after the event? Name scholars.` ; plus grondtekst Joh 2:19-22, 4:21-24, 11:48 via biblehub
  - **Specifiek:** Andreas Köstenberger, Stephen Motyer, Alan Kerr, Mary Coloe [6,8-10] (vervangingstheologie als post-70 antwoord op "hoe aanbid je zonder tempel"); B.F. Westcott [1] ("in John the judgment has been wrought"; Johannes laat zien hoe het ware godsvolk de tempelval overleeft); Joh als functioneel equivalent van de synoptische apocalyps [2,3] (Paracleet i.p.v. cataclysme); D. Moody Smith [23] ("written in the knowledge of what transpired a generation or so after Jesus' death"); Robert Fortna [24] ("purely ironic, a prediction-after-the-fact"); Raymond E. Brown, Craig Koester [25,26,27]. Verssamenhang Joh 2:19-22; 4:21-24; 11:48. Geen Olivetrede-parallel met Marcus 13 [1,2]. Primaire toets: NT-grondtekst via biblehub (geen brontekst).
  - **Raakt as:** datering · **Aard:** primair en secundair · **Primair nagezien:** ja (Joh 2:19-22, 4:21-24, 11:48 via biblehub/NA28)
  - **Commando:** n.v.t. (NT via biblehub; brontekst dekt het NT niet), https://biblehub.com/text/john/2-19.htm ; https://biblehub.com/text/john/4-21.htm ; https://biblehub.com/text/john/11-48.htm
  - **Opgehaald:** ja · **Type:** literair en historisch
- **Claim (weerlegging):** Re-toets van Josephus *Ant.* 20.97 en 20.102 voor de Lucas-Josephus-weerlegging: Theudas onder Fadus (44-46) en Judas de Galileeër met de census onder Quirinius (jaar 6), dus Lucas' "Judas ná Theudas" is chronologisch omgekeerd; meerderheid (Schürer) leest dit als bewijs dat Lucas Josephus níet overschreef.
  - **Bron:** brontekst perseus, Josephus *Antiquitates* 20.97 en 20.102
  - **Specifiek:** *Ant.* 20.97 "Φάδου δὲ τῆς Ἰουδαίας ἐπιτροπεύοντος γόης τις ἀνὴρ Θευδᾶς ὀνόματι"; 20.102 "οἱ παῖδες Ἰούδα τοῦ Γαλιλαίου ... Κυρινίου τῆς Ἰουδαίας τιμητεύοντος ... Ἰάκωβος καὶ Σίμων, οὓς ἀνασταυρῶσαι προσέταξεν Ἀλέξανδρος". Census Quirinius = jaar 6; Theudas onder Fadus = 44-46; zonen van Judas onder Alexander = 46-48. Argument tegen Mason-afhankelijkheid (minderheidslezing).
  - **Raakt as:** datering · **Aard:** primair · **Primair nagezien:** ja (beide passages opgehaald; chronologische omkering bevestigd)
  - **Commando:** `./.agents/tools/brontekst perseus "urn:cts:greekLit:tlg0526.tlg001.perseus-grc2:20.97"` en `./.agents/tools/brontekst perseus "urn:cts:greekLit:tlg0526.tlg001.perseus-grc2:20.102"`
  - **Opgehaald:** ja · **Type:** historisch

### 🏛️ Grieks-Romeins
- **Claim:** De afscheidsrede (Joh 13-17) is naar literaire vorm een Grieks-Romeinse consolatie (filosofische sterfbedscène à la Plato's *Phaedo*; consolatio van Cicero/Seneca, "rouw niet, mijn heengaan is tot jullie voordeel", Joh 14:27-28; 16:6-7) en een symposion (maaltijd plus lang vriendengesprek over de hoogste thema's, met de wijnstok op de plaats van de wijn), niet een halachische seder.
  - **Bron:** nlm "John - exegesis", query: `Do commentators read the Johannine Farewell Discourse (John 13-17) and especially John 15:13 ('greater love has no one than this, that someone lay down his life for his friends') and John 15:14-15 ('I no longer call you servants but friends') against Greco-Roman literary forms: the philosopher's deathbed/consolation scene (Socrates in Plato's Phaedo), the symposium genre, and the Greek philosophical friendship topos of dying for one's friend (Plato Symposium, Aristotle Nicomachean Ethics, Damon and Pythias)? Name scholars such as George Parsenios (Departure and Consolation), or others who set John's farewell against Greco-Roman consolation and friendship literature.`
  - **Specifiek:** George L. Parsenios, *Departure and Consolation: The Johannine Farewell Discourses in Light of Greco-Roman Literature* [1-4] (Phaedo-model; Socrates onderwijst zijn kring vlak voor de executie); consolatoire retoriek van Cicero en Seneca [5],[2],[6] (Joh 14:27-28; 16:6-7); Harold W. Attridge [7],[8],[9] (symposion-genre; Plato's *Symposium* en Joh's Laatste Avondmaal beide met een theorie van liefde; wijnstok-beeldspraak i.p.v. wijn). Verssamenhang Joh 13-17.
  - **Raakt as:** karakter · **Aard:** secundair · **Primair nagezien:** n.v.t.
  - **Commando:** n.v.t.
  - **Opgehaald:** ja · **Type:** literair
- **Claim:** Joh 15:13-15 is een Grieks-filosofische vriendschapstopos: "groter liefde dan voor je vrienden te sterven" (τὴν ψυχὴν θεῖναι ὑπὲρ τῶν φίλων) als de maxime van het sterven voor de vriend (Plato *Symp.* 179 ὑπεραποθνῄσκειν, Alkestis; Aristoteles *EN* 9.8/1169a κἂν δέῃ ὑπεραποθνήσκειν), plus de herijking slaaf-tot-vriend langs parrhēsia en gedeelde kennis (de slaaf "weet niet wat zijn heer doet"), de antieke vriendschapsdefinitie, niet een halachische categorie.
  - **Bron:** brontekst perseus (Plato *Symposion* 179; Aristoteles *Ethica Nicomachea* 9.8 = Bekker 1169a) plus nlm "John - exegesis" (zelfde query hierboven)
  - **Specifiek:** Primaire toets: Plato *Symp.* 179 "ὑπεραποθνῄσκειν γε μόνοι ἐθέλουσιν οἱ ἐρῶντες" en Alkestis "ἐθελήσασα μόνη ὑπὲρ τοῦ αὑτῆς ἀνδρὸς ἀποθανεῖν", door de goden geëerd; Achilles "ὑπεραποθανεῖν" voor Patroklos. Aristoteles *EN* 9.8 (1169a) "ἀληθὲς δὲ περὶ τοῦ σπουδαίου καὶ τὸ τῶν φίλων ἕνεκα πολλὰ πράττειν ... κἂν δέῃ ὑπεραποθνήσκειν". Secundair: Richard Bauckham [10] (Joh 15:13 vat een gangbare Grieks-Romeinse vriendschapsmaxime samen; nuance: Grieken prezen het als ideaal/mythe, Jezus voert het uit; Damon en Phintias via Diodorus Siculus [12]); David Konstan [19-21] (klassieke vriendschapsdeugden pistis, parrhēsia); Klaus Scholtissek [18] (hellenistische *Freundschaftsethik* bij Joh 15:13); doulos vs philos onderscheiden door parrhēsia en gedeelde kennis, Aristoteles' "levend werktuig" [14-17]; Gail R. O'Day en Dorothy A. Lee [22],[13],[23] (versmelting *philia* en *agapē*). Verssamenhang Joh 15:13-15. Aristoteles *EN* 1169a valt in Perseus' boek-hoofdstukschema onder 9.8.
  - **Raakt as:** karakter · **Aard:** primair en secundair · **Primair nagezien:** ja (Plato *Symp.* 179: ὑπεραποθνῄσκειν + Alkestis bevestigd; Aristoteles *EN* 9.8/1169a: κἂν δέῃ ὑπεραποθνήσκειν voor vrienden bevestigd)
  - **Commando:** `./.agents/tools/brontekst perseus "urn:cts:greekLit:tlg0059.tlg011.perseus-grc2:179"` en `./.agents/tools/brontekst perseus "urn:cts:greekLit:tlg0086.tlg010.perseus-grc2:9.8"`
  - **Opgehaald:** ja · **Type:** literair en filosofisch

### ✡️ Joods
- **Claim:** De Paracleet als "Geest der waarheid" (τὸ πνεῦμα τῆς ἀληθείας, Joh 14:17; 15:26; 16:13) heeft een uitsluitend joods-Palestijnse pre-christelijke titel: Qumran 1QS 3-4 (Verhandeling over de Twee Geesten) en het Testament van Juda 20; de forensische functie (getuigen, aanklagen) ondergraaft Bauckhams uitweg en de term is hoe dan ook joods, niet hellenistisch. Located binnen de afscheidsrede die Grieks-Romeins opeist.
  - **Bron:** nlm "John - exegesis", query: `Is the Johannine Paraclete and the 'Spirit of truth' (pneuma tes aletheias, John 14:17, 15:26, 16:13) related to the Qumran Treatise of the Two Spirits in the Community Rule (1QS 3-4), the 'spirit of truth' versus 'spirit of deceit/error'? Which commentators (e.g. Raymond Brown) argue this dualism is the Jewish-Palestinian background of the Farewell Discourse?` ; plus primaire tekst Testament van Juda 20 via brontekst sefaria
  - **Specifiek:** Raymond E. Brown [1,2] (Qumran + Testament van Juda als de enige pre-christelijke vindplaatsen van de titel "Spirit of Truth"; joods-Palestijnse achtergrond van de Paracleet; 1QS: "Spirit of Truth"/"Prince of Lights" tegenover "Angel of Darkness"/"Spirit of Falsehood"); Urban C. von Wahlde [5-7] (eindredactie en 1 Joh 4:1-6 nemen het Qumran-paradigma over); Otto Betz [8,9] (Paracleet = Geest der waarheid + forensische trekken van Michaël); John Breck, D. Moody Smith [10-12]; tegenstem Leon Morris en Andreas Köstenberger [13,14] ("coincidence of language, not thought"; John heeft geen tegen-geest), Richard Bauckham [15-17] (forensische, niet dualistische context; "spirit of truth" als natuurlijke vroeg-joodse formatie als "spirit of wisdom"), Riku Tuppurainen [18]. Primaire toets Testament van Juda 20:1-5: "two spirits ... the spirit of truth and the spirit of deceit" (רוח האמת ורוח הכזב) en "the spirit of truth testifieth all things, and accuseth all" (ותעיד... ותאשים) bevestigd.
  - **Raakt as:** karakter · **Aard:** primair en secundair · **Primair nagezien:** ja (Testament van Juda 20 via Sefaria: titel "geest van waarheid" en forensische functie "getuigt/klaagt aan" bevestigd; let op: basis is Grieks, Sefaria-Hebreeuws is retroversie [Wikisource], Engels = R.H. Charles 1908; 1QS niet in Sefaria, dus voor Qumran nagezien: nee)
  - **Commando:** `./.agents/tools/brontekst sefaria "The Testaments of the Twelve Patriarchs, The Testament of Judah the Fourth Son of Jacob and Leah 20"`
  - **Opgehaald:** ja · **Type:** exegetisch en literair
- **Claim:** De wijnstok van Joh 15:1-8 is het profetische Israël-wijngaardbeeld (Jesaja 5:7, Psalm 80), niet symposionwijn; "de ware (ἀληθινός) wijnstok" herleest dat als Jezus die het ontrouwe Israël vervult.
  - **Bron:** nlm "John - exegesis", query: `In John 15:1-8 'I am the true vine', is the background the Old Testament image of Israel as God's vine/vineyard (Psalm 80, Isaiah 5:1-7, Jeremiah 2:21, Ezekiel 19, Hosea 10)? Do commentators read 'true vine' as a contrast where Jesus replaces unfruitful Israel-as-vine? Also: is the Farewell Discourse a Jewish testament/farewell-speech genre (Deuteronomy, Genesis 49, Testaments of the Twelve Patriarchs)?` ; plus primaire teksten Jesaja 5:1-7 en Psalm 80:9-17 via brontekst sefaria
  - **Specifiek:** synthese (kernclaim "commentators unanimously agree"; geen enkele auteur bij naam aan de Israël-vine-claim toegeschreven). ἀληθινός als "ware/echte" vervulling van Israël [7,12,13]; Jezus vervangt Israël met zichzelf [11,20]. Testament-genre: Genesis 49, Deuteronomium 31-33, Testamenten van de Twaalf Patriarchen [21-31]; bouwstenen verzamelen-aankondigen-troosten-vermanen-waarschuwen-opvolger-gebed; "heb elkaar lief" als kernbestanddeel van de Testamenten [36,37]; opvolger = Paracleet [40,41]; slotgebed = Joh 17 [21-23]. Primaire toets: Jesaja 5:7 "כִּי כֶרֶם יְהֹוָה צְבָאוֹת בֵּית יִשְׂרָאֵל" en Psalm 80:9 "גֶּפֶן מִמִּצְרַיִם תַּסִּיעַ" + oordeel/verbranding bevestigd.
  - **Raakt as:** karakter · **Aard:** primair en secundair · **Primair nagezien:** ja (Jesaja 5:1-7 en Psalm 80:9-17 via Sefaria; Israël-wijngaard en oordeelsmotief bevestigd)
  - **Commando:** `./.agents/tools/brontekst sefaria "Isaiah 5:1-7"` en `./.agents/tools/brontekst sefaria "Psalms 80:9-17"`
  - **Opgehaald:** ja · **Type:** exegetisch en literair

### ⚖️ Moderator (verificatie)
- **Scharnierende toetsing datering-as, Lucas-na-Josephus tegen de primaire tekst.** Vroeg en Laat lazen Josephus *Ant.* 20.97 en 20.102 verschillend; ik legde beide passages zelf na.
  - **Bevestigd:** 20.97 "Φάδου δὲ τῆς Ἰουδαίας ἐπιτροπεύοντος γόης τις ἀνὴρ Θευδᾶς ὀνόματι" (Theudas onder procurator Fadus, 44-46); 20.102 "οἱ παῖδες Ἰούδα τοῦ Γαλιλαίου ... Κυρινίου τῆς Ἰουδαίας τιμητεύοντος ... Ἰάκωβος καὶ Σίμων, οὓς ἀνασταυρῶσαι προσέταξεν Ἀλέξανδρος" (zonen van Judas de Galileeër, census onder Quirinius = jaar 6, gekruisigd onder Alexander 46-48).
  - **Uitkomst:** de koppeling Theudas-Judas bestaat in Josephus zoals geclaimd, maar de tekst toont juist de chronologische omkering (Judas' census jaar 6 ligt decennia vóór Theudas onder Fadus) die de meerderheid (Schürer) tégen Masons afhankelijkheidsthese inbrengt. Het argument geeft Vroeg geen netto dateringswinst en is bovendien onder Vroegs eigen premisse (Lucas gebruikte Johannes) omkeerbaar naar laat. Gewicht: grotendeels neutraal/averechts.
  - **Commando:** `./.agents/tools/brontekst perseus "urn:cts:greekLit:tlg0526.tlg001.perseus-grc2:20.97"` en `... :20.102`
- **Scharnierende toetsing karakter-as, Geest der waarheid tegen het Testament van Juda 20.** Joods claimde dat de forensische functie (getuigen, aanklagen) al joods is en Bauckhams uitweg ondergraaft.
  - **Bevestigd:** Testament van Juda 20 bevat "twee geesten ... de geest van waarheid en de geest van bedrog" (רוח האמת ורוח הכזב) en, beslissend, "de geest van waarheid getuigt over alles en klaagt allen aan" (ותעיד... ותאשים / "the spirit of truth testifieth all things, and accuseth all"). De forensische functie staat er als geclaimd.
  - **Caveat (gewicht licht begrensd):** het Sefaria-Hebreeuws is een Wikisource-retroversie en het Engels is R.H. Charles (1908); het Griekse origineel van de Testamenten kan christelijke redactie bevatten, en 1QS staat niet in Sefaria (Qumran niet primair toetsbaar hier). De dualistische twee-geesten-stof is echter de erkende Qumran-motief en breed-joods (Bauckham noemt "geest van waarheid" zelf een natuurlijke vroeg-joodse formatie), dus de joodse herkomst van het concept blijft staan ondanks de redactiekwestie.
  - **Commando:** `./.agents/tools/brontekst sefaria "The Testaments of the Twelve Patriarchs, The Testament of Judah the Fourth Son of Jacob and Leah 20"`
- **Overige citaten:** geen `⚠️ onverifieerbaar`-markeringen. De Israël-wijngaard-claim (Jes 5:7, Ps 80) leunt op een notebook-synthese zonder auteurstoeschrijving ("commentators unanimously"), maar de primaire teksten zijn bevestigd en de Israël-als-wijngaard-lezing is een standaardgegeven, dus dat is geen bezwaar. Het consolatie/symposion-argument (Parsenios, Attridge) is concreet maar niet primair getoetst.

---

# 📑 Bibliografie

Geconsolideerd uit de per-ronde-log hierboven. Elke regel verwijst naar de ronde(n) waarin de bron is
ingezet. Primaire teksten dragen het exact gedraaide `brontekst`-commando, zodat elke lezing
herhaalbaar is.

## A. Primaire antieke teksten (via de `brontekst`-CLI)

Alle hieronder met **primair nagezien: ja**, tenzij anders vermeld.

| Tekst | Plaats | Bevestigd | Commando | Ronde |
|---|---|---|---|---|
| Flavius Josephus, *Bellum Judaicum* | 5.184 | ἵδρυτο / ἦν (verleden tijd voor de verwoeste tempel) | `brontekst perseus "urn:cts:greekLit:tlg0526.tlg004.perseus-grc2:5.184"` | 1 |
| Clemens Romanus, *Epistula ad Corinthios I* (1 Clemens) | 41 | προσφέρονται / προσφέρεται (praesens voor de verdwenen cultus) | `brontekst perseus "urn:cts:greekLit:tlg1271.tlg001.1st1K-grc1:41"` | 1 |
| Aristoteles, *Poetica* | 11.4; 11.5 | *anagnorisis* = ἐξ ἀγνοίας εἰς γνῶσιν μεταβολή; koppeling met *peripeteia* | `brontekst perseus "urn:cts:greekLit:tlg0086.tlg034.perseus-grc2:11.4"` (en `:11.5`) | 1 |
| Aristoteles, *Rhetorica* | 2.23.4 | topos ἐκ τοῦ μᾶλλον καὶ ἧττον (a fortiori als Griekse gemeenplaats) | `brontekst perseus "urn:cts:greekLit:tlg0086.tlg038.perseus-grc2:2.23.4"` | 2 |
| Plato, *Symposion* | 179 | ὑπεραποθνῄσκειν + Alkestis (sterven voor de geliefde) | `brontekst perseus "urn:cts:greekLit:tlg0059.tlg011.perseus-grc2:179"` | 3 |
| Aristoteles, *Ethica Nicomachea* | 9.8 (Bekker 1169a) | κἂν δέῃ ὑπεραποθνήσκειν voor vrienden | `brontekst perseus "urn:cts:greekLit:tlg0086.tlg010.perseus-grc2:9.8"` | 3 |
| Flavius Josephus, *Antiquitates Judaicae* | 20.97; 20.102 | Θευδᾶς onder Fadus; zonen van Judas de Galileeër, census onder Quirinius (chronologische omkering) | `brontekst perseus "urn:cts:greekLit:tlg0526.tlg001.perseus-grc2:20.97"` (en `:20.102`) | 3 |
| Jesaja (Tanakh) | 43:10 | אֲנִי הוּא + "opdat jullie weten en geloven" | `brontekst sefaria "Isaiah 43:10"` | 1 |
| Deuteronomium (Tanakh) | 32:39 | אֲנִי אֲנִי הוּא | `brontekst sefaria "Deuteronomy 32:39"` | 1 |
| Genesis (Tanakh) | 45:3; 45:4 | אֲנִי יוֹסֵף ("Ik ben Jozef", LXX *egō eimi*) | `brontekst sefaria "Genesis 45:3"` (en `45:4`) | 1 |
| Misjna *Soekka* | 4:9; 5:1; 5:3 | waterlibatie (נסוך המים), *Simchat Beit ha-Sho'evah*, verlichting van de voorhoven | `brontekst sefaria "Mishnah Sukkah 4:9"` (en `5:1`, `5:3`) | 2 |
| Babylonische Talmoed, *Yoma* | 85b | קל וחומר met het besnijdenis-argument (R. Elazar ben Azarja) | `brontekst sefaria "Yoma 85b"` | 2 |
| *Testament van Juda* (Test. XII Patriarchen) | 20 | "geest van waarheid" + forensische functie (getuigt/klaagt aan). **Caveat:** Sefaria-Hebreeuws is Wikisource-retroversie, Engels = R.H. Charles (1908); Grieks origineel kan christelijke redactie dragen | `brontekst sefaria "The Testaments of the Twelve Patriarchs, The Testament of Judah the Fourth Son of Jacob and Leah 20"` | 3 |
| Jesaja (Tanakh) | 5:1-7 | כֶּרֶם יְהֹוָה צְבָאוֹת בֵּית יִשְׂרָאֵל (Israël als wijngaard) | `brontekst sefaria "Isaiah 5:1-7"` | 3 |
| Psalmen (Tanakh) | 80:9-17 | גֶּפֶן מִמִּצְרַיִם (wijnstok uit Egypte) + oordeelsmotief | `brontekst sefaria "Psalms 80:9-17"` | 3 |
| Diodorus Siculus, *Bibliotheca Historica* (Isis-aretalogie) | 1.27.4 | **niet opgehaald** (404 in canonical-greekLit/First1KGreek; argument bleef secundair) | `brontekst perseus "urn:cts:greekLit:tlg0060.tlg001.perseus-grc2:1.27.4"` | 2 |

## B. Nieuwtestamentische grondtekst (biblehub / NA28)

Het NT zit niet in de `brontekst`-corpora; deze verzen zijn via biblehub-interlinear tegen NA28 nagezien.

- **Johannes 5:2** ἔστιν (praesens, Betzata), kernvers datering-as. Rondes 1-2.
- **Johannes 11:18; 18:1; 19:41** ἦν (imperfectum voor plaatsen), tijdsvormcontrast met 5:2. Ronde 2. <https://biblehub.com/text/john/11-18.htm>, `/18-1.htm`, `/19-41.htm`
- **Johannes 21:23-24** οὐκ ἀποθνήσκει; ὁ μαρτυρῶν (praesens part.), ἐστιν, ὁ γράψας (aoristus part.), οἴδαμεν (perf.), epiloog/eindredactie. Ronde 2. <https://biblehub.com/text/john/21-23.htm>, `/21-24.htm`
- **Johannes 14:31** ἐγείρεσθε, ἄγωμεν ἐντεῦθεν; **18:1** ἐξῆλθεν, redactionele naad. Ronde 3. <https://biblehub.com/text/john/14-31.htm>, `/18-1.htm`
- **Johannes 2:19-22; 4:21-24; 11:48 (τὸν τόπον); 11:51-52**, vervangingschristologie en het stilzwijgen-argument. Ronde 3. <https://biblehub.com/text/john/2-19.htm>, `/4-21.htm`, `/11-48.htm`
- **Matteüs 22:7; Lucas 19:43-44; 21:20**, synoptische vaticinia ex eventu als vergelijkingspunt. Ronde 3.
- **Handelingen 5:36-37** (Theudas + Judas de Galileeër), naast Josephus *Ant.* 20.97-102. Ronde 3.

## C. Secundaire literatuur (in het debat bij naam genoemd)

Datering-as:
- Richard Bauckham, *Jesus and the Eyewitnesses* (onomastiek, "protective anonymity").
- Tal Ilan, *Lexicon of Jewish Names in Late Antiquity*, deel I (Palestina 330 v.Chr.-200 n.Chr.).
- Ruth Edwards (kritiek op de onomastiek: tijdspanne en diaspora-ruis).
- Brent Nongbri, "The Use and Abuse of P52: Papyrological Pitfalls in the Dating of the Fourth Gospel," *Harvard Theological Review* 98, nr. 1 (2005): 23-48.
- Frans Neirynck en C.K. Barrett (Johannes' kennis van de synoptici; minor agreements).
- Leon Morris, D.A. Carson, B.F. Westcott, Daniel Wallace (tijdsvorm ἔστιν/ἦν; Joh 21).
- J.A.T. Robinson, *Redating the New Testament* (ἔστιν en het stilzwijgen bij Joh 11:48).
- Andreas Köstenberger, William Hendriksen, F.F. Bruce (levende getuige in Joh 21:24).
- Rudolf Bultmann, Raymond E. Brown, Francis Moloney, Rudolf Schnackenburg, Barnabas Lindars (Joh 21 en de afscheidsrede als gefaseerde schoolredactie).
- W.F. Albright; J. Ramsey Michaels, Adolf Schlatter, Walter Bauer, Arthur W. Pink (τόπος = tempel).
- Craig Blomberg, D. Moody Smith, Robert Fortna (Joh 11:48 als prediction-after-the-fact).
- Stephen Motyer, Alan Kerr, Mary Coloe, Craig Koester (vervangingschristologie als post-70 antwoord).
- Steve Mason (Lucas put uit Josephus' *Antiquitates*) tegenover Emil Schürer (meerderheidskritiek).

Karakter-as:
- Kasper Bro Larsen, *Recognizing the Stranger: Recognition Scenes in the Gospel of John* (Brill, 2008).
- Richard Burridge (*bios*-genre); Jo-Ann Brant en George Parsenios (Johannes en het Griekse theater).
- David Wead en Paul Duke (johanneïsche ironie, vgl. Sophocles/Thirlwall).
- George L. Parsenios, *Departure and Consolation* (afscheidsrede als consolatio); Harold W. Attridge (symposion-genre).
- Marianne Meye Thompson, Paul A. Rainbow, Johannes Beutler, Gerard Sloyan, D.A. Carson (egō eimi uit *ani hu* / Deutero-Jesaja en Deut 32:39).
- Brian Neil Peterson, Hassell Bullock (Ezechiël-herkenningsformule); Rudolf Bultmann (*Rekognitionsformel*; Offenbarungsreden).
- Eduard Norden, *Agnostos Theos*; G.P. Wetter; George W. MacRae; Jan Bergman; C.H. Dodd; Eduard Schweizer (Isis-aretalogie / hellenistische openbaringstaal). Tegenstem: Catrin Williams, David Mark Ball, Heinrich Zimmermann (absolute egō eimi blijft joods).
- Charles Puskas, Raymond E. Brown, C.H. Dodd, David Daube (*The New Testament and Rabbinic Judaism*), Andrew Lincoln, Urban C. von Wahlde (*qal wachomer* / halachische redeneervorm).
- George Beasley-Murray, Craig Keener, E.C. Hoskyns, Gale Yee (Soekot-liturgie).
- Richard Bauckham, David Konstan, Klaus Scholtissek, Gail R. O'Day, Dorothy A. Lee (vriendschapstopos Joh 15:13-15).
- Raymond E. Brown, Urban C. von Wahlde, Otto Betz, John Breck, D. Moody Smith (Paracleet / "Geest der waarheid" en Qumran 1QS). Tegenstem: Leon Morris, Andreas Köstenberger, Richard Bauckham, Riku Tuppurainen.

## D. Webbronnen

- Samenvatting Bauckham, *Jesus and the Eyewitnesses* hfst. 4: <https://biblicalscholarship.wordpress.com/2008/07/07/a-summary-of-chapter-4-of-richard-bauckhams-jesus-and-the-eyewitnesses/> (ronde 1).
- Jimmy Akin, "References to the Temple Operating After A.D. 70": <https://jimmyakin.com/2015/01/references-to-the-temple-operating-after-a-d-70.html> (ronde 1).
- "Johannine Anagnorisis: Current Scholarship and Future Perspectives," *Religions* (MDPI): <https://www.mdpi.com/2077-1444/17/6/702> (ronde 1).
- Nongbri, "The Use and Abuse of P52," HTR 98 (2005), via Cambridge Core: <https://www.cambridge.org/core/journals/harvard-theological-review/article/abs/use-and-abuse-of-p52-papyrological-pitfalls-in-the-dating-of-the-fourth-gospel/676A4EA909EB03046F89DB8CE1F050BE> (ronde 2).
- biblehub interlinear (NA28-grondtekst), zie de verzen onder B.

## E. Commentaar-notebook (NotebookLM via `nlm`)

Notebook **"John - exegesis"**, doorzocht met `nlm cross query "..." -n "John - exegesis"`. De exact
uitgevoerde queries en de met name genoemde commentatoren staan per claim in de log hierboven (rondes
1-3). Gebruikt voor onder meer: onomastiek, synoptische afhankelijkheid, tijdsvormcontrast, Joh 21 en
21:23-24, het stilzwijgen bij Joh 11:48, de naad bij Joh 14:31, vervangingschristologie, anagnorisis,
egō eimi / *ani hu*, Soekot-liturgie, *qal wachomer*, Isis-aretalogie, afscheidsrede als
consolatie/symposion, vriendschapstopos, Paracleet / Geest der waarheid en de Israël-wijngaard.

## Toetsstatus in één oogopslag

- **Primair getoetst en bevestigd:** vijftien antieke passages via `brontekst` (rij A, met succes opgehaald)
  plus de NT-verzen via biblehub/NA28 (rij B).
- **Niet primair toetsbaar gebleken (tijdens het debat):** Diodorus Siculus 1.27.4 (404; Isis-argument
  bleef secundair); Qumran 1QS (niet in Sefaria, **na afloop alsnog getoetst**, zie Naschrift);
  Tal Ilans naamdataset (niet via `brontekst`).
- **Met caveat:** Testament van Juda 20 (retroversie/redactiekwestie).
- **Geen `⚠️ onverifieerbaar`-markeringen** door de moderator in enige ronde; één notebook-synthese
  (Israël-wijngaard) zonder auteurstoeschrijving, maar met bevestigde primaire teksten.

---

# 🔎 Naschrift (na afloop van het debat), primaire toetsing Qumran 1QS

De ronde-3-claim over de Geest der waarheid leunde mede op de Gemeenschapsregel (1QS), die niet in
Sefaria of de Perseus-repos staat en tijdens het debat niet kon worden getoetst. Na afloop is dit
gedaan via het NotebookLM-corpus `De Complete Dode Zeerollen (English)` (de Dode Zeerollen in Engelse
vertaling, via notebook, niet de Hebreeuwse grondtekst).

- **Claim:** 1QS, Verhandeling over de Twee Geesten (kol. III-IV), bevat de titel "geest van waarheid",
  de tegenstelling Prince of Light versus Angel of Darkness, en een licht/duister-dualisme; dit verankert
  de joodse, voor-christelijke herkomst van de johanneïsche Paracleet als "Geest der waarheid".
  - **Bron:** nlm "De Complete Dode Zeerollen (English)", query 1: `In the Community Rule (1QS), the Treatise of the Two Spirits: does it speak of a 'spirit of truth' versus a 'spirit of deceit/falsehood'? Quote the relevant lines.` ; query 2: `In the Community Rule (1QS), Treatise of the Two Spirits (cols 3-4): does it use the exact title 'spirit of truth'? does it name a 'Prince of Lights' versus an 'Angel of Darkness'? is this a dualistic light-versus-darkness scheme? Quote the exact lines.`
  - **Specifiek (letterlijke regels uit de notebook-output):** "the spirits of truth and injustice";
    "the spirit of truth (to cleanse him) of all abomination and injustice" (1QS IV); "all the children
    of righteousness are ruled by the Prince of Light ... the children of injustice are ruled by the Angel
    of Darkness" (1QS III); "those born of truth spring from a fountain of light, but those born of
    injustice spring from a source of darkness" (1QS III).
  - **Raakt as:** karakter · **Aard:** primair · **Primair nagezien:** ja (via notebook, Engelse vertaling)
  - **Commando:** `nlm cross query "<zie query 1 en 2 hierboven>" -n "De Complete Dode Zeerollen (English)"`
  - **Opgehaald:** ja · **Type:** literair en exegetisch
- **Gevolg voor de scores:** geen wijziging van richting of grootte. De karakter-as blijft +4; dit punt
  telde in ronde 3 al mee en de scores van een afgesloten debat worden niet met terugwerkende kracht
  herschreven. Wel verschuift een met voorbehoud gewogen winstpunt naar een primair bevestigd winstpunt
  en is de openstaande Qumran-vraag gesloten. De datering-as wordt niet geraakt.

<!--
FORMAT (kopieer per bron; opponenten en moderator vullen aan):

## Ronde N

### ⏳ Vroeg
- **Claim:** <korte trefwoorden>
  - **Bron:** nlm "John - exegesis", query: `<exacte querytekst>`
  - **Specifiek:** Wallace [3], Morris [7] bevestigen; Carson [12] contra. Vers Joh 5:2.
  - **Raakt as:** datering · **Aard:** secundair · **Primair nagezien:** ja (biblehub Joh 5:2: *estin* staat er)
  - **Commando:** n.v.t. (NT via biblehub; brontekst dekt het NT niet)
  - **Opgehaald:** ja · **Type:** syntactisch

### 🕰️ Laat
- **Claim:** <korte trefwoorden>
  - **Bron:** https://volledige-url
  - **Specifiek:** auteur/titel van de pagina
  - **Raakt as:** datering · **Aard:** secundair · **Primair nagezien:** nee
  - **Opgehaald:** ja · **Type:** literair

### 🏛️ Grieks-Romeins
- **Claim:** <korte trefwoorden>
  - **Bron:** ...
  - **Specifiek:** ...
  - **Raakt as:** karakter · **Aard:** primair | secundair · **Primair nagezien:** ...
  - **Commando:** `brontekst perseus "urn:cts:greekLit:...:..."` (of n.v.t.)
  - **Opgehaald:** ... · **Type:** filosofisch | literair | retorisch

### ✡️ Joods
- **Claim:** ...
  - **Bron:** ...
  - **Specifiek:** ...
  - **Raakt as:** karakter · **Aard:** ... · **Primair nagezien:** ...
  - **Commando:** `brontekst sefaria "Targum Onkelos, Genesis 1:1"` (of n.v.t.)
  - **Opgehaald:** ... · **Type:** ...

### ⚖️ Moderator (verificatie)
- **Bron bestaat?** <claim/bron> → <bevestigd, of ⚠️ onverifieerbaar>
- **Lezing klopt tegen primaire tekst?** <claim> → <welke primaire tekst geraadpleegd + uitkomst>
  - **Commando:** <het gedraaide brontekst-commando of de geraadpleegde URL>
-->
