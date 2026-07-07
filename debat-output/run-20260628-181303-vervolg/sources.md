# 📚 Bronnenlog, run run-20260628-181303-vervolg

Traceerbaar overzicht van elke geraadpleegde bron, zodat nalezers exact kunnen zien welke
commentaar of webpagina achter een claim zit. Dit is het naslagwerk bij het werkdossier:
het werkdossier bevat de argumenten, dit bestand de volledige herkomst.

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
- **Claim:** Joh 18:31 (geen capitale jurisdictie voor het Sanhedrin) weerspiegelt accuraat de Romeinse vóór-70 provinciale ordening (*ius gladii* voorbehouden aan de prefect); verdedigd door romanist Sherwin-White en exegeten Bruce, Carson, Morris, Blinzler.
  - **Bron:** nlm "John - exegesis", query: `Does John 18:31 ('it is not lawful for us to put anyone to death') accurately reflect the Roman removal of capital jurisdiction (ius gladii) from the Jewish Sanhedrin before AD 70? Which commentators discuss the historical accuracy of Sanhedrin capital jurisdiction in the Johannine passion narrative, and is this legal detail integral to the evangelist's own composition rather than a detachable source aside?`
  - **Specifiek:** Verdedigers A.N. Sherwin-White [6,8,2,5] ("most jealously guarded of all the attributes of government"), F.F. Bruce, D.A. Carson, Leon Morris, Josef Blinzler [6,2,3,7]; tegenstanders Lietzmann, Winter, Juster, Burkill [1,2,3]; mediërend E. Mary Smallwood [10]. Vers Joh 18:31.
  - **Raakt as:** datering · **Aard:** secundair · **Primair nagezien:** ja (NT-tekst, zie volgende entry)
  - **Commando:** n.v.t. (notebook)
  - **Opgehaald:** ja · **Type:** juridisch
- **Claim:** Het Griekse Joh 18:31 luidt "οὐκ ἔξεστιν ἡμῖν ἀποκτεῖναι οὐδένα"; ἔξεστιν staat op verteltijd, geen schrijftijd-argument.
  - **Bron:** https://biblehub.com/interlinear/john/18-31.htm
  - **Specifiek:** interlineaire grondtekst Joh 18:31 (NA/biblehub).
  - **Raakt as:** datering · **Aard:** primair · **Primair nagezien:** ja (biblehub interlinear, de clausule staat er letterlijk)
  - **Commando:** n.v.t. (NT zit niet in brontekst-databases; via biblehub)
  - **Opgehaald:** ja · **Type:** grammaticaal/tekstkritisch
- **Claim:** De juridische realia van Joh 18:30-31 is johanneïsche redactie (niet bronlaag) en de theologische spil van het zevenscènig proces, dat de kruisvervulling (12:32-33; 18:32) opzet; de vóór-70-accuratesse zit dus op de eindredactionele compositielaag.
  - **Bron:** nlm "John - exegesis" (zelfde query als hierboven)
  - **Specifiek:** Robert Fortna [11] identificeert Joh 18:30-31 als johanneïsche redactie, niet de onderliggende bron; "theological linchpin of John's seven-scene trial narrative" [12,13,15,17,18]. Vers Joh 18:30-32.
  - **Raakt as:** datering · **Aard:** secundair · **Primair nagezien:** n.v.t.
  - **Commando:** n.v.t. (notebook)
  - **Opgehaald:** ja · **Type:** literair/juridisch
- **Claim:** Onafhankelijke joodse traditie dateert het verlies van de halsrechtspraak op ca. 30 (veertig jaar vóór de verwoesting), wat de constitutionele toestand achter Joh 18:31 bevestigt.
  - **Bron:** Sefaria, Sanhedrin 41a
  - **Specifiek:** baraita "Veertig jaar vóór de verwoesting van de Tempel werd het Sanhedrin verbannen uit de Kamer van Gehouwen Steen"; R. Yitzhak bar Avudimi: zij berechtten geen halszaken (דיני נפשות) meer ("the court's power to judge capital cases was nullified").
  - **Raakt as:** datering · **Aard:** primair · **Primair nagezien:** ja (de passage staat letterlijk in de opgehaalde tekst)
  - **Commando:** `./.agents/tools/brontekst sefaria "Sanhedrin 41a"`
  - **Opgehaald:** ja · **Type:** juridisch/historisch

### 🕰️ Laat
- **Claim:** De externe receptiegeschiedenis (Ignatius circa 107-110; eerste commentaar Heracleon circa 160-180; orthodoxe verankering pas Irenaeus circa 180) en al haar concurrerende reconstructies (Bauer-Brown-Barrett "Johannophobia" én de tegenpool Charles Hill) convergeren op een compositie in de late eerste eeuw, nooit vóór 70; Van Kootens "oudste/foundationele evangelie" wordt door de receptie niet gereproduceerd.
  - **Bron:** nlm "John - exegesis", query: `What is the earliest external attestation of the Fourth Gospel? Does Ignatius of Antioch (c. 107-110) show knowledge of Johannine theology or language? When was the first commentary on John written (Heracleon the Valentinian)? Discuss the pattern of early heterodox reception versus delayed orthodox reception of John, and what this implies for a late-first-century composition window. Which scholars discuss this (Hill, orthodox Johannophobia)?`
  - **Specifiek:** Ignatius-parallellen (Woord uit stilzwijgen cf. Joh 1:1; "levend water"/"kom tot de Vader" cf. Joh 4:10/7:38; "de deur" cf. Joh 10:9) [10-18]; gedeeld-milieu-lezing Koester, Schoedel [19,20] vs. literaire ontlening Braun, Hill, Kieffer, Nagel [11,21,22]; eerste commentaar Heracleon circa 160-180 [3,23-31]; Johannophobia-paradigma J.N. Sanders, Bauer, Barrett, Haenchen, Koester, Brown [28,33-54]; Hill ontmantelt het en plaatst compositie in late eerste eeuw [31,67,104-115]. Vers: Joh 1:1; 4:10; 7:38; 10:9.
  - **Raakt as:** datering · **Aard:** secundair · **Primair nagezien:** n.v.t. (Ignatius niet in Perseus-repo; `brontekst perseus "urn:cts:greekLit:tlg1443.tlg004.perseus-grc1:8"` gaf 404)
  - **Commando:** n.v.t. (notebook)
  - **Opgehaald:** ja · **Type:** historisch/receptiegeschiedenis
- **Claim (rebuttal Vroeg):** De "veertig jaar"-baraita over het verlies van de halsrechtspraak staat óók in de eeuwen ná 70 geredigeerde Jeruzalemse Talmoed; accurate vóór-70 juridische realia is daarmee aantoonbaar dateringsneutraal. Aanvullend: de juridische accuratesse is omstreden (Lietzmann, Winter, Juster, Burkill, Goguel, Barrett), en Blomberg concedeert dat Joh 18:31 een compositie in de jaren 80-90 toelaat.
  - **Bron:** Sefaria, Jeruzalemse Talmoed Sanhedrin 1:1; plus nlm "John - exegesis", query: `Did the Sanhedrin actually lose all capital jurisdiction before AD 70, or is John 18:31 a theological construction? Which commentators argue the loss of capital power is historically contested (Stephen, James the Just, the temple balustrade inscription)? And does accurate legal memory of a pre-70 constitutional fact tell us anything about the DATE of composition, given that the Babylonian Talmud preserves the same fact centuries later?`
  - **Specifiek:** Yerushalmi Sanhedrin 1:1, letterlijk "Forty years before the Temple was destroyed, criminal jurisdiction was removed from Israel" (קוֹדֶם לְאַרְבָּעִים שָׁנָה ... נִיטְלוּ דִינֵי נְפָשׁוֹת). Notebook: tegenstanders historiciteit Lietzmann, Winter, Juster, Burkill, Goguel, Barrett [4-6]; Blomberg [12]: "comfortably allows for the Gospel's final composition in the 80s or 90s CE".
  - **Raakt as:** datering · **Aard:** primair (Yerushalmi) + secundair (notebook) · **Primair nagezien:** ja (Yerushalmi Sanhedrin 1:1, de zin staat letterlijk in de opgehaalde Hebreeuwse en Engelse tekst)
  - **Commando:** `/Users/ckleier/Desktop/projects/studiedag_ad_fontes/.agents/tools/brontekst sefaria "Jerusalem Talmud Sanhedrin 1:1"`
  - **Opgehaald:** ja · **Type:** juridisch/historisch

### 🏛️ Grieks-Romeins
- **Claim:** John kadert zijn christologische hoogtepunten in keizerlijke titulatuur; Thomas' "mijn Heer en mijn God" (Joh 20:28) spiegelt/contesteert Domitianus' geëiste "dominus et deus noster", en "redder van de wereld" (Joh 4:42) is een keizerlijke eretitel. Deze lezing veronderstelt een Grieks-Romeins referentiekader.
  - **Bron:** nlm "John - exegesis", query: `Does the Gospel of John engage Roman imperial cult titulature? Discuss 'Savior of the world' (sōtēr tou kosmou, John 4:42) and Thomas's confession 'my Lord and my God' (ho kyrios mou kai ho theos mou, John 20:28) in relation to imperial titles like Soter, Kyrios, and Domitian's 'dominus et deus'. Which scholars argue John uses or subverts Greco-Roman imperial ideology (Lance Byron Richey, Warren Carter, Richard Cassidy)?`
  - **Specifiek:** Richard Cassidy (*John's Gospel in New Perspective*) [21-23], Warren Carter (*John and Empire*) [24-29], Lance Byron Richey (*Roman Imperial Ideology and the Gospel of John*) [30-34]; *sōtēr tou kosmou* als keizerlijke titel voor Caesar t/m Hadrianus [1-3]; Domitianus' *dominus et deus noster* via Suetonius [13-17]. Verzen Joh 4:42; 20:28.
  - **Raakt as:** karakter · **Aard:** secundair · **Primair nagezien:** ja (Suetonius, zie volgende entry)
  - **Commando:** n.v.t. (notebook)
  - **Opgehaald:** ja · **Type:** historisch
- **Claim:** Domitianus eiste de aanspreektitel "dominus et deus noster"; staat letterlijk bij Suetonius, primair getoetst.
  - **Bron:** Perseus/Scaife, Suetonius *Divus Domitianus* 13.2
  - **Specifiek:** "pari arrogantia ... sic coepit: 'dominus et deus noster hoc fieri iubet.' unde institutum posthac, ut ne scripto quidem ac sermone cuiusquam appellaretur aliter." De formule staat woordelijk in de opgehaalde Latijnse tekst.
  - **Raakt as:** karakter · **Aard:** primair · **Primair nagezien:** ja (Perseus lat2, de zin staat er letterlijk)
  - **Commando:** `./.agents/tools/brontekst perseus "urn:cts:latinLit:phi1348.abo022.perseus-lat2:13.2"`
  - **Opgehaald:** ja · **Type:** literair/historisch
- **Claim:** "Redder van de wereld" (*sōtēr*) is epigrafisch een keizerlijke eretitel; de Priene-kalenderinscriptie eert Augustus als de gezonden "redder" die de oorlog beëindigt.
  - **Bron:** https://en.wikipedia.org/wiki/Priene_calendar_inscription
  - **Specifiek:** IK Priene 14 / OGIS 458 (9 v.Chr.), Augustus "sent ... as a savior, both for us and for our descendants, that he might end war and arrange all things"; rede van hogepriester Apollonius van Azanië.
  - **Raakt as:** karakter · **Aard:** primair (inscriptie) via secundaire weergave · **Primair nagezien:** nee (niet tegen het epigrafisch grondcorpus zelf getoetst, alleen via vertaling)
  - **Commando:** n.v.t. (inscriptie niet in Perseus/Sefaria)
  - **Opgehaald:** ja · **Type:** epigrafisch/historisch

### ✡️ Joods
- **Claim:** De stenen kruiken van Joh 2:6 ("voor de reiniging van de Joden") reflecteren de halacha dat stenen vaatwerk onvatbaar is voor rituele onreinheid (Lev 11:32-33 contra aardewerk), en sluiten aan op de archeologisch geattesteerde vóór-70 chalksteen-industrie (Yitzhak Magen, Hizma; chalksteen + mikwaot bij Khirbet Qana).
  - **Bron:** nlm "John - exegesis", query: `In John 2:6 the six water jars are specified as STONE jars 'for the Jewish rites of purification'. Why stone specifically? Discuss the halachic principle that stone vessels are not susceptible to ritual impurity (Mishnah Kelim, Parah), and the archaeological evidence for the chalk/stone vessel industry in early Roman Judea and Galilee (Yitzhak Magen). Which commentators note that this detail reflects authentic Jewish purity halacha?`
  - **Specifiek:** Marianne Meye Thompson en Urban C. von Wahlde [4,8,11] (Magen-archeologie, Hizma-werkplaats, vaten van 80-120 liter, chalksteen + mikwaot bij Khirbet Qana); Leon Morris, Paul A. Rainbow, Jo-Ann A. Brant [1,6,7] (Mishnah Kelim/Parah); Gary M. Burge, George Martin, Raymond E. Brown [2,3,12] (aardewerk onherstelbaar onrein vs. herbruikbaar steen); Craig L. Blomberg, Craig R. Koester, Amy-Jill Levine [5,9,13]. Vers Joh 2:6.
  - **Raakt as:** karakter · **Aard:** secundair · **Primair nagezien:** ja (Mishnah Kelim 10:1: כְּלֵי אֲבָנִים onder de vaten die beschermen; Mishnah Parah 3:2: כּוֹסוֹת שֶׁל אֶבֶן, stenen bekers in het rode-koe-ritueel; beide staan letterlijk in de opgehaalde tekst)
  - **Commando:** `./.agents/tools/brontekst sefaria "Mishnah Kelim 10:1"` en `./.agents/tools/brontekst sefaria "Mishnah Parah 3:2"`
  - **Opgehaald:** ja · **Type:** halachisch/archeologisch
- **Claim:** "Redder van de wereld" (*sōtēr tou kosmou*, Joh 4:42) heeft zijn matrix in Deutero-Jesaja's monotheïstisch universalisme (Jes 45:21-22, God als enige *moshia* die "alle einden der aarde" redt), niet primair in de keizercultus; bovendien uitgesproken door Samaritanen met een Taheb-verwachting (Deut 18:15-18), voor wie een Romeins kader het minst plausibel is.
  - **Bron:** nlm "John - exegesis", query: `Is 'Savior of the world' (sōtēr tou kosmou, John 4:42) better explained from Deutero-Isaiah's monotheistic universalism (Isaiah 45:21-22, God as the only mošiaʿ who saves all the ends of the earth) and the Samaritan Taheb expectation, rather than from Roman imperial cult? Note that the confession is spoken by SAMARITANS. Which commentators connect sōtēr to the Hebrew mošiaʿ as a divine title and to the Samaritan setting?`
  - **Specifiek:** Richard Bauckham [2,3,4] (verwijst expliciet naar Jes 45:21-24 LXX, "I am God and there is no other besides me, a righteous one and a Savior... Turn to me and be saved"); Marianne Meye Thompson [1] (Jes 43:3,11; 45:15,21-22; 49:26, universele strekking); David F. Ford, Ruth Edwards [5,6,7]; Gerald L. Borchert [11] en D.A. Carson [12] (Taheb-setting). Vers Joh 4:42.
  - **Raakt as:** karakter · **Aard:** secundair · **Primair nagezien:** ja (Jesaja 45:21-22: אֵל־צַדִּיק וּמוֹשִׁיעַ en פְּנוּ־אֵלַי וְהִוָּשְׁעוּ כׇּל־אַפְסֵי־אָרֶץ staan letterlijk in de opgehaalde tekst)
  - **Commando:** `./.agents/tools/brontekst sefaria "Isaiah 45:21-22"`
  - **Opgehaald:** ja · **Type:** exegetisch/literair

### ⚖️ Moderator (verificatie, ronde 1)
- **Bron bestaat / lezing klopt?** Laats scharnierclaim dat de "veertig jaar"-baraita over het verlies van de halsrechtspraak ook in de Jeruzalemse Talmoed staat → bevestigd. De zin staat letterlijk: "Forty years before the Temple was destroyed, criminal jurisdiction was removed from Israel" (קוֹדֶם לְאַרְבָּעִים שָׁנָה ... נִיטְלוּ דִינֵי נְפָשׁוֹת). Hiermee is aangetoond dat correcte vóór-70 juridische realia dateringsneutraal is.
  - **Commando:** `/Users/ckleier/Desktop/projects/studiedag_ad_fontes/.agents/tools/brontekst sefaria "Jerusalem Talmud Sanhedrin 1:1"`
- **Bron bestaat / lezing klopt?** Joods' scharnierclaim dat *sōtēr tou kosmou* (Joh 4:42) zijn matrix heeft in Deutero-Jesaja → bevestigd. Jesaja 45:21-22 bevat woordelijk אֵל־צַדִּיק וּמוֹשִׁיעַ ("een rechtvaardige God en een verlosser") en פְּנוּ־אֵלַי וְהִוָּשְׁעוּ כׇּל־אַפְסֵי־אָרֶץ ("wendt u tot Mij en wordt verlost, alle einden der aarde"). De combinatie *moshia* plus universele reikwijdte staat er.
  - **Commando:** `/Users/ckleier/Desktop/projects/studiedag_ad_fontes/.agents/tools/brontekst sefaria "Isaiah 45:21-22"`
- **Overig:** Geen citaat oogde verzonnen; notebook-toeschrijvingen waren concreet (auteur plus vers). De Priene-inscriptie is door Grieks-Romeins zelf eerlijk gemarkeerd als alleen via vertaling (Wikipedia) nagezien, niet tegen het epigrafisch grondcorpus; dat ene punt weegt daarom iets lichter.

## Ronde 2

### ⏳ Vroeg
- **Claim (weerlegging Laat):** Gerealiseerde eschatologie is geen betrouwbare dateringsklok: zij zit al in de oudste traditie (Mt 12:28 // Lc 11:20; Lc 17:21), Johannes behoudt een sterke toekomstige eschatologie (6:39,40,44,54; 11:24; 12:48; 5:28-29; 14:3; 21:22), en Brown noemt theologische ontwikkeling een "onbetrouwbare chronometer"; de parousievertraging-als-motor (Schweitzer/Werner) is door Käsemann afgewezen, en Carson noemt datering op ontwikkeltrajecten "extreem zwak".
  - **Bron:** nlm "John - exegesis", query: `Is realized eschatology a reliable criterion for DATING the Gospel of John late? Do commentators note that realized eschatology is already present in the EARLIEST Jesus tradition (e.g. the Beelzebul saying 'the kingdom of God has come upon you', Matthew 12:28 // Luke 11:20; Luke 17:21 'the kingdom is among you'), and that the 'delay of the parousia' as an engine of theological development (Martin Werner, Frühkatholizismus) has been criticized? Also: does John RETAIN a strong FUTURE eschatology (6:39,40,44,54 'I will raise him up on the last day'; 5:28-29; 14:3 'I will come again'; 21:22), so that present and future coexist rather than the present replacing the future? Do Brown or Schnackenburg actually treat realized eschatology as a chronological dating clock, or do they reject that?`
  - **Specifiek:** Raymond E. Brown [1,21,22] (theologische ontwikkeling = "onbetrouwbare chronometer"; niets in Johannes' theologie sluit eerste-eeuwse datering uit; veel niet later dan Romeinen, jaren 50); Brown [23] landt niettemin ná 70 op grond van de nadruk-als-antwoord-op-de-vertraging; Ernst Käsemann [4] (Schweitzer-volgelingen / parousievertraging als "doodlopende weg"); Leon Morris [11] ("de laatste dag" exclusief johanneïsch); Jörg Frey [8,19,20] (verwerpt Bultmanns kerkelijke redacteur); Schnackenburg/Blank [19,24,25]; D.A. Carson [26] ("extreem zwak"). Verzen Lc 17:21; Mt 12:28; Joh 5:24-29; 6:39-54; 14:3; 21:22.
  - **Raakt as:** datering · **Aard:** secundair · **Primair nagezien:** n.v.t. (NT-verzen niet apart getoetst; brontekst dekt het NT niet)
  - **Commando:** n.v.t. (notebook)
  - **Opgehaald:** ja · **Type:** theologisch/historisch
- **Claim:** De aposynagōgos-passages (Joh 9:22; 12:42; 16:2) vereisen geen datum ná 85; de Martyn-these (Birkat ha-Minim / synode van Jamnia) is op alle drie pijlers afgebroken.
  - **Bron:** nlm "John - exegesis", query: `The aposynagōgos passages in John (9:22, 12:42, 16:2, 'they would be put out of the synagogue') are the backbone of J. Louis Martyn's argument that John reflects the Birkat ha-Minim (curse on heretics) formalized at the council of Jamnia/Yavneh c. 85-90, hence a post-85 date. How strong is this for DATING? Do commentators (e.g. Adele Reinhartz, Jonathan Bernier, Daniel Boyarin) argue that (a) the 'council of Jamnia' is largely a scholarly construct/legend, (b) the Christian-specific clause (notzrim/minim) in the Birkat ha-Minim is a later addition and did not function as a universal expulsion mechanism, and (c) expulsion or exclusion from the synagogue/community already existed BEFORE AD 70? Does the expulsion motif therefore NOT require a late date?`
  - **Specifiek:** Daniel Boyarin [6] (Javne als latere terugprojectie; decreten in "limbo of unestablished hypotheses" [7]); Wayne Meeks [5,6] ("red herring in Johannine research"); Adele Reinhartz, Reuven Kimelman [5,6,8,9] (notzrim latere toevoeging, geen universeel mechanisme, geen rabbijnse diaspora-jurisdictie [5,8,10]); Jonathan Bernier, Edward W. Klink, Leon Morris [11-13] (lokale informele uitsluiting bestond vóór 70). Verzen Joh 9:22; 12:42; 16:2.
  - **Raakt as:** datering · **Aard:** secundair · **Primair nagezien:** n.v.t.
  - **Commando:** n.v.t. (notebook)
  - **Opgehaald:** ja · **Type:** historisch
- **Claim:** Formele uitsluiting uit een joodse geloofsgemeenschap bestond ruim vóór 70 (Ezra 10:8; 1QS-strafcode), zodat het uitstotingsmotief geen late ondergrens nodig heeft.
  - **Bron:** Sefaria, Ezra 10:8; en nlm "De Complete Dode Zeerollen (English)", query: `Does the Community Rule (1QS) contain a penal code with rules for EXPULSION or exclusion from the community (the Yahad)? Quote the provisions for permanent expulsion / being sent away from the community for serious offenses, and temporary exclusion from the pure meal. This is to establish that formal expulsion from a Jewish religious community existed in Palestine BEFORE AD 70.`
  - **Specifiek:** Ezra 10:8 woordelijk וְה֥וּא יִבָּדֵ֖ל מִקְּהַ֥ל הַגּוֹלָֽה ("themselves excluded from the congregation of the returning exiles"). 1QS: permanente expulsie "shall be expelled from the Council of the Community and shall return no more" (overtreding Wet van Mozes; laster tegen de gemeente); tijdelijke uitsluiting van de "pure Meal" voor lichtere vergrijpen. (DZR-notebook = Engelse vertaling.)
  - **Raakt as:** datering · **Aard:** primair · **Primair nagezien:** ja (Ezra 10:8 via brontekst sefaria, de afzonderingsformule staat letterlijk in de opgehaalde Hebreeuwse en Engelse tekst; 1QS-strafcode via DZR-notebook, Engelse vertaling)
  - **Commando:** `/Users/ckleier/Desktop/projects/studiedag_ad_fontes/.agents/tools/brontekst sefaria "Ezra 10:8"`
  - **Opgehaald:** ja · **Type:** historisch

### 🕰️ Laat
- **Claim:** De gerealiseerde eschatologie van Johannes (5:24-25, "de ure komt en is nu") is een doelbewuste verwerking van de uitgebleven parousie; afgezet tegen Paulus' nog nabije wederkomstverwachting in 1 Tess 4:15 (omstreeks 50) meet dit een ontwikkeling die een tweedegeneratie-datum (jaren 80-90) veronderstelt.
  - **Bron:** nlm "John - exegesis", query: `Do commentators argue that the developed Paraclete/Spirit theology in John 14-16 (the Spirit as Jesus' continuing presence, who 'reminds' the disciples of all Jesus said, 14:26, and 'guides into all truth', 16:13) functions to address the death of the founding eyewitness generation and the prolonged absence/delay of Jesus' return, thereby reflecting a LATE composition by a second-generation community? Also: does John show a shift from futurist to 'realized' eschatology (e.g. 5:24-25 'the hour is coming and now is') that scholars (Brown, Schnackenburg, Bultmann, Gary Burge, C.H. Dodd) read as a sign of theological development away from the imminent expectation of the earliest communities? What does this imply for DATING the final form of the Gospel?`
  - **Specifiek:** C.H. Dodd [16] (gerealiseerde eschatologie als verwerking van de parousievertraging); Rudolf Bultmann [17-20] (demythologisering; 5:28-29 toegeschreven aan latere "ecclesiastical redactor"); Raymond Brown, Rudolf Schnackenburg, Gary Burge [4,21-24] (nadruk op het "reeds" als troost voor een door de vertraging teleurgestelde gemeente); dateringsconclusie jaren 80-90 [23,29]. Verzen Joh 4:23; 5:24-25; 5:28-29.
  - **Raakt as:** datering · **Aard:** secundair · **Primair nagezien:** ja (Joh 5:25 "ἔρχεται ὥρα καὶ νῦν ἐστιν" en 1 Tess 4:15 "ἡμεῖς οἱ ζῶντες οἱ περιλειπόμενοι εἰς τὴν παρουσίαν τοῦ Κυρίου" beide via biblehub interlinear bevestigd; NT zit niet in de brontekst-databases Sefaria/Perseus)
  - **Commando:** n.v.t. (NT via biblehub: https://biblehub.com/interlinear/john/5-25.htm en https://biblehub.com/interlinear/1_thessalonians/4-15.htm)
  - **Opgehaald:** ja · **Type:** historisch
- **Claim:** De Paraklen-leer (Joh 14:16,26; 16:13) functioneert als antwoord op het wegvallen van de ooggetuigen en de vertraagde wederkomst: de Geest als blijvende inwonende tegenwoordigheid van Jezus die directe toegang en traditiewaarborg garandeert voor een post-apostolische gemeente, wat een tweedegeneratie-compositie impliceert.
  - **Bron:** nlm "John - exegesis" (zelfde query als hierboven)
  - **Specifiek:** Raymond Brown [1-7] (de twee crises van de johanneïsche gemeenschap: dood van de ooggetuigen en parousievertraging; Geest als "alter ego" van Christus die directe toegang waarborgt, latere gelovigen geen tweederangs); Gary Burge [3,8,10] (Paracleet demythologiseert de apocalyptische verwachting: Jezus al teruggekeerd in de inwonende Geest). Verzen Joh 14:16,26; 16:13.
  - **Raakt as:** datering · **Aard:** secundair · **Primair nagezien:** n.v.t.
  - **Commando:** n.v.t. (notebook)
  - **Opgehaald:** ja · **Type:** historisch/sociaal-historisch
- **Claim (weerlegging Vroeg):** De evangelist glosseert de overdracht aan Pilatus juist wél (Joh 18:32, verklarende terzijde over de doodssoort), en zijn glos-gewoonte (4:9, 2:6) wijst op een publiek van buitenstaanders op afstand, niet op een nabij vóór-70 Judees publiek; het ontbreken van één glos draagt geen dateringsgewicht.
  - **Bron:** NT-tekst Joh 18:32; 4:9; 2:6 (standaardtekst, gebruikt in weerlegging)
  - **Specifiek:** Joh 18:32 verklarende terzijde "opdat het woord van Jezus vervuld zou worden, waarmee hij aanduidde welke dood hij sterven zou"; 4:9 glos "Joden hebben geen omgang met Samaritanen".
  - **Raakt as:** datering · **Aard:** primair (NT) · **Primair nagezien:** nee (bekende NT-verzen, niet apart via biblehub getoetst voor deze weerlegging)
  - **Commando:** n.v.t. (NT niet in brontekst-databases)
  - **Opgehaald:** n.v.t. · **Type:** literair

### ✡️ Joods
- **Claim:** Joh 10:22-39 (Inwijdingsfeest/Chanoeka, "het was winter") verankert zijn christologie in de consecratietaal van het feest: het "geheiligd" (ἡγίασεν, Joh 10:36) correspondeert met de herwijding van altaar en tempel (חנוכת המזבח, 25 Kislev) zodat Jezus zich als de ware geconsacreerde tempel/altaar presenteert; ondecodeerbaar zonder joods-liturgisch kader.
  - **Bron:** nlm "John - exegesis", query: `John 10:22-39 is set explicitly at the Feast of Dedication (Hanukkah/Encaenia), 'and it was winter'. In John 10:36 Jesus says the Father 'consecrated/sanctified' (hēgiasen) him and sent him into the world. Do commentators argue there is a deliberate wordplay between Hanukkah (the festival of the RE-DEDICATION/consecration of the altar and temple after Antiochus, 1 Maccabees 4) and Jesus presenting himself as the one whom the Father CONSECRATED, i.e. as the true sanctified temple/altar? How does the Maccabean/Hanukkah setting shape the Christology of John 10? Which scholars (e.g. Raymond Brown, C.H. Dodd, Gale Yee, Craig Koester) discuss the Dedication/consecration theme behind John 10:36?`
  - **Specifiek:** Raymond E. Brown [7,17] (sectietitel "Jesus is consecrated in place of the temple altar"); Richard Bauckham [9,18] (Jezus als eschatologisch nieuw brandofferaltaar); Francis J. Moloney [6] ("sign and shadow" volmaakt); Craig R. Koester [11,12] (Antiochus-contrast, anti-blasfemie); Mary L. Coloe, Gale A. Yee, D.A. Carson, Beasley-Murray, Keener, Köstenberger, VanderKam [16,19]. Vers Joh 10:22,30,33,36.
  - **Raakt as:** karakter · **Aard:** secundair · **Primair nagezien:** ja (1 Makkabeeën 4:54-59: חנוכת המזבח, "inwijding van het altaar", acht dagen vanaf 25 Kislev, staat letterlijk in de opgehaalde Hebreeuwse en Engelse tekst)
  - **Commando:** `./.agents/tools/brontekst sefaria "The Book of Maccabees I 4:54-59"`
  - **Opgehaald:** ja · **Type:** liturgisch/exegetisch
- **Claim:** Thomas' "mijn Heer en mijn God" (Joh 20:28) is qua taalvorm de persoonlijke psalmische gebedsaanspraak (de doublure kyrios+theos met possessief "mijn"), niet Domitianus' onpersoonlijke ambtelijke titel "dominus et deus noster"; herkomst is joods-liturgisch, de keizerlijke parallel hooguit contrastklank.
  - **Bron:** Sefaria, Psalms 35:23 (primaire toets); ondersteunende lezing nlm "John - exegesis" (Psalm 35 LXX als wortel, reeds in ronde 1 door Grieks-Romeins erkend)
  - **Specifiek:** Psalm 35:23 woordelijk אֱלֹהַ֖י וַאדֹנָ֣י ("mijn God en mijn Heer", JPS: "O my God and my Sovereign"); vergelijk Ps 5:3 en 84:4 ("mijn Koning en mijn God"). Contrast: Suetonius *Divus Domitianus* 13.2 "dominus et deus noster" als derde-persoons rescript-aanhef (reeds in ronde 1 gelogd).
  - **Raakt as:** karakter · **Aard:** primair (Psalter) · **Primair nagezien:** ja (de dubbelaanspraak staat letterlijk in de opgehaalde tekst)
  - **Commando:** `./.agents/tools/brontekst sefaria "Psalms 35:23"`
  - **Opgehaald:** ja · **Type:** liturgisch/exegetisch

### 🏛️ Grieks-Romeins
- **Claim:** De herkenningsscène (ἀναγνώρισις) is een dragende verhaalvorm van Johannes (Maria/tuinman Joh 20:14-16; handen en zijde als γνώρισμα 20:20,27; Natanaël 1:47-50; de blindgeborene hfst. 9), die de conventies van Aristoteles' Poetica, Homerus' Odyssee, de Griekse tragedie en de hellenistische roman volgt.
  - **Bron:** nlm "John - exegesis", query: `Does the Gospel of John use the Greek literary type-scene of ANAGNORISIS (recognition scene), as analyzed by Kasper Bro Larsen in 'Recognizing the Stranger'? Discuss recognition scenes such as Mary Magdalene at the tomb (John 20:11-18), the Emmaus-like non-recognition, Nathanael (1:47-50), the man born blind (ch.9), and how these follow the conventions of recognition (anagnorisis) from Aristotle's Poetics, Homer's Odyssey, Greek drama and the Greek novel. Which commentators connect John's recognition scenes to Greco-Roman literary convention rather than Jewish models?`
  - **Specifiek:** Jo-Ann A. Brant [10,20] (Jezus' getoonde handen en zijde als "tokens" vergeleken met Eurycleia die Odysseus aan zijn litteken herkent, Odyssee; en de stem die Maria's misvatting corrigeert vergeleken met Elektra/Orestes in Sophokles' Electra); Johannes Beutler [21] ("Rabboeni" mimt de anagnorisis-toon van de antieke Griekse roman, gescheiden geliefden die elkaar herkennen); George Parsenios [2,22] en Kasper Bro Larsen [2,22,23] (Johannes neemt de vormen van Griekse tragedie/drama over voor het epistemologische herkenningsdrama). Verzen Joh 1:47-50; 9; 20:14-18,20,27.
  - **Raakt as:** karakter · **Aard:** secundair · **Primair nagezien:** ja (Aristoteles-definitie zelf opgehaald, zie volgende entry)
  - **Commando:** n.v.t. (notebook)
  - **Opgehaald:** ja · **Type:** literair/narratologisch
- **Claim:** Aristoteles definieert ἀναγνώρισις in de Poetica hfst. 11 als "ἐξ ἀγνοίας εἰς γνῶσιν μεταβολή, ἢ εἰς φιλίαν ἢ εἰς ἔχθραν" (omslag van onwetendheid naar kennis, tot vriendschap of vijandschap), met de mooiste herkenning samenvallend met de peripeteia (Oedipus); deze dubbele uitkomst en epistemologische omslag structureren Johannes' krisis.
  - **Bron:** Perseus/Scaife, Aristoteles *Poetica* hfst. 11
  - **Specifiek:** Letterlijk: "ἀναγνώρισις δέ, ὥσπερ καὶ τοὔνομα σημαίνει, ἐξ ἀγνοίας εἰς γνῶσιν μεταβολή, ἢ εἰς φιλίαν ἢ εἰς ἔχθραν, τῶν πρὸς εὐτυχίαν ἢ δυστυχίαν ὡρισμένων· καλλίστη δὲ ἀναγνώρισις, ὅταν ἅμα περιπετείᾳ γένηται, οἷον ἔχει ἡ ἐν τῷ Οἰδίποδι." Staat woordelijk in de opgehaalde Griekse tekst (passage 11).
  - **Raakt as:** karakter · **Aard:** primair · **Primair nagezien:** ja (Perseus grc2, de definitie staat er letterlijk; ref "1452a" faalde in het schema, passage-ref "11" gaf de juiste tekst)
  - **Commando:** `/Users/ckleier/Desktop/projects/studiedag_ad_fontes/.agents/tools/brontekst perseus "urn:cts:greekLit:tlg0086.tlg034.perseus-grc2:11"`
  - **Opgehaald:** ja · **Type:** literair
- **Claim (corroboratie Larsen):** Larsens *Recognizing the Stranger: Recognition Scenes in the Gospel of John* (Brill, Biblical Interpretation Series 93, 2008) is de eerste monografie die anagnorisis-typescènes in Johannes systematisch analyseert; herkenning was een conventie van antiek drama en verhaal, door Aristoteles hooggewaardeerd (Oedipus, Odysseus' thuiskomst).
  - **Bron:** https://brill.com/display/title/14193
  - **Specifiek:** Brill-uitgeverspagina, Kasper Bro Larsen, "Recognizing the Stranger"; bevestigt titel, jaar (2008) en strekking (Johannes gebruikt en transformeert de structuren van het herkenningstype).
  - **Raakt as:** karakter · **Aard:** secundair · **Primair nagezien:** n.v.t.
  - **Commando:** n.v.t.
  - **Opgehaald:** ja (via WebSearch-resultaat; uitgeverspagina) · **Type:** literair
- **Claim (weerlegging Thomas):** Domitianus' "dominus et deus" was een directe aanspreekvorm, niet enkel een onpersoonlijk rescript: Suetonius zegt dat hij voortaan "ne scripto quidem ac sermone cuiusquam appellaretur aliter" werd, waarbij appellare directe aanspraak betekent; daarmee vervalt Joods' registeronderscheid tussen psalmische vocatief en keizerlijke derde persoon.
  - **Bron:** Perseus/Scaife, Suetonius *Divus Domitianus* 13.2 (reeds opgehaald en gelogd in ronde 1)
  - **Specifiek:** "...unde institutum posthac, ut ne scripto quidem ac sermone cuiusquam appellaretur aliter." Het werkwoord appellare (aanspreken) ziet op directe aanspraak.
  - **Raakt as:** karakter · **Aard:** primair · **Primair nagezien:** ja (ronde 1, Perseus lat2)
  - **Commando:** `./.agents/tools/brontekst perseus "urn:cts:latinLit:phi1348.abo022.perseus-lat2:13.2"`
  - **Opgehaald:** ja · **Type:** literair/historisch

### ⚖️ Moderator (verificatie, ronde 2)
- **Lezing klopt tegen primaire tekst?** Vroegs scharnierclaim dat formele uitsluiting uit een joodse gemeenschap vóór 70 bestond (Ezra 10:8) → bevestigd. De tekst bevat woordelijk וְה֥וּא יִבָּדֵ֖ל מִקְּהַ֥ל הַגּוֹלָֽה ("themselves excluded from the congregation of the returning exiles"). De claim houdt tekstueel stand; zij is dateringsneutraal (verwijdert een laat anker, bewijst geen vroege datum), zoals Vroeg zelf concedeerde.
  - **Commando:** `/Users/ckleier/Desktop/projects/studiedag_ad_fontes/.agents/tools/brontekst sefaria "Ezra 10:8"`
- **Lezing klopt tegen primaire tekst?** Grieks-Romeins' scharnierclaim dat Aristoteles' Poetica 11 de anagnorisis-definitie en de tweesprong "tot vriendschap of vijandschap" geeft → bevestigd. Woordelijk: "ἀναγνώρισις δέ, ὥσπερ καὶ τοὔνομα σημαίνει, ἐξ ἀγνοίας εἰς γνῶσιν μεταβολή, ἢ εἰς φιλίαν ἢ εἰς ἔχθραν ... καλλίστη δὲ ἀναγνώρισις, ὅταν ἅμα περιπετείᾳ γένηται, οἷον ἔχει ἡ ἐν τῷ Οἰδίποδι." De klassieke parallel zegt precies wat de opponent beweert.
  - **Commando:** `/Users/ckleier/Desktop/projects/studiedag_ad_fontes/.agents/tools/brontekst perseus "urn:cts:greekLit:tlg0086.tlg034.perseus-grc2:11"`
- **Lezing klopt tegen primaire tekst?** Joods' claim dat 1 Makkabeeën 4:54-59 de Chanoeka-consecratie van het altaar op 25 Kislev attesteert → bevestigd. Woordelijk חנוכת המזבח ("inwijding van het altaar"), gevierd "acht dagen, vanaf de vijfentwintigste dag van de maand Kislev, jaar op jaar". De consecratiematrix achter ἡγίασεν (Joh 10:36) staat.
  - **Commando:** `/Users/ckleier/Desktop/projects/studiedag_ad_fontes/.agents/tools/brontekst sefaria "The Book of Maccabees I 4:54-59"`
- **Overig:** Geen citaat oogde verzonnen; notebook-toeschrijvingen waren concreet (auteur plus vers). De 1QS-strafcode is via het Dode Zeerollen-notebook (Engelse vertaling) aangevoerd, niet apart door mij hertoetst; de Ezra-parallel draagt de pre-70-claim zelfstandig.

## Ronde 3

### ⏳ Vroeg
- **Claim:** Johannes is het breedst geattesteerde NT-boek in de vroege Egyptische papyri (26+ Griekse handschriften, vrijwel het hele evangelie dekkend); Llewelyn toont geen periode-skew in de verhouding Johannes-papyri, waarmee de Bauer/Aland-constructie van "Johannophobie"/vertraagde receptie instort, juist het receptiebeeld waarop Laats argument tegen Van Kootens "oudste evangelie"-pijler leunde.
  - **Bron:** nlm "John - exegesis", query: `What do the earliest papyri of the Gospel of John (P52 / Rylands Gk 457; P66; P90; P75) establish as a terminus ante quem for the Fourth Gospel? How is P52 dated palaeographically (Roberts c.125; Nongbri's wider range), where was it found (provincial Egypt), and what does its provenance imply about the time needed for composition, circulation and copying (diffusion lag)? Did the discovery of P52 refute the old Tübingen ultra-late dating of John (Baur c.160-170)? Is John in fact relatively WELL attested papyrologically in second-century Egypt compared with other gospels, contradicting a 'delayed reception/Johannophobia' picture?`
  - **Specifiek:** S.R. Llewelyn [18] (geen significant verschil in de proporties Johannes-papyri tussen vroege en latere periodes; "simple but persistent preference for the Gospel of John"; Johannophobie-these een "irrelevant and unnecessary complication"); "John is the most widely attested New Testament book in the early papyri" [19]; tegenover Walter Bauer en Kurt Aland [17,18].
  - **Raakt as:** datering · **Aard:** secundair · **Primair nagezien:** n.v.t. (papyri staan niet in Perseus/Sefaria)
  - **Commando:** n.v.t. (notebook)
  - **Opgehaald:** ja · **Type:** papyrologisch
- **Claim:** Verspreidingsvertraging: P52 (Joh 18:31-33 recto / 18:37-38 verso), een codexblad van de Egyptische markt, door Roberts in de eerste helft 2e eeuw (~125) en door Orsini-Clarysse op 125-175 gedateerd; een provinciaal-Egyptisch afschrift veronderstelt compositie + mediterrane circulatie + overschrijven (~2-3 decennia), wat de compositie uiterlijk naar ~90-100 duwt; P52 + Egerton maakten Baurs ultralate datering (160-170) definitief af. Palaeografische datering betwist (Nongbri; Rylands nu ~200), daarom geen dragend gewicht op het fragment zelf.
  - **Bron:** nlm "John - exegesis" (zelfde query als hierboven) + https://en.wikipedia.org/wiki/Rylands_Library_Papyrus_P52
  - **Specifiek:** nlm: Roberts (1935) ~125-130, vergeleken met P. Fayum 110 (94 CE) [2,3,4]; diffusie-lag-schatting 2-3 decennia → compositie ~90-100 [11,12,13]; P52 + Egerton "coup de grâce" aan Baur 160-170 [12,14,15,16]; Brent Nongbri bredere range tot late 2e/vroege 3e eeuw [5,6,7]. Wikipedia/Rylands: inhoud Joh 18:31-33 (recto) en 18:37-38 (verso); "acquired on the Egyptian market in 1920 by Bernard Grenfell"; dateringen Roberts 100-150, Orsini-Clarysse 125-175, Nongbri later, Rylands "nearer to 200 AD".
  - **Raakt as:** datering · **Aard:** secundair (met manuscriptcatalogus) · **Primair nagezien:** n.v.t. (papyrus niet in Perseus/Sefaria; gegevens wel geverifieerd tegen de Rylands/Wikipedia-beschrijving)
  - **Commando:** n.v.t.
  - **Opgehaald:** ja · **Type:** papyrologisch/codicologisch

### 🕰️ Laat
- **Claim:** Johannes veronderstelt dat zijn lezers de synoptische traditie al kennen (harmoniserende glosse Joh 3:24; abrupte "de Twaalf" 6:67-71; proleptische zalvende Maria 11:2; zonen van Zebedeüs alleen 21:2), wat hem in de relatieve chronologie ná de synoptici plaatst en Van Kootens "oudste evangelie"-/Lukaanse-posterioriteitspijler ondergraaft; eindvorm op die grond gedateerd in de jaren 90.
  - **Bron:** nlm "John - exegesis", query: `Does the Gospel of John presuppose that its readers ALREADY KNOW the Synoptic tradition / written gospels, implying John is LATER in the relative chronology (against the view that John is the oldest gospel)? Discuss the editorial cross-reference glosses and unexplained allusions: John 3:24 'for John had not yet been thrown into prison' as a harmonizing aside presupposing the Synoptic framework (Mark 1:14); the abrupt introduction of 'the Twelve' in 6:67-71 without narrating their call; John 11:2 introducing Mary as 'the one who anointed the Lord' before the anointing is narrated (a back/forward reference presupposing a known story); the sons of Zebedee mentioned only at 21:2 though prominent in the Synoptics. Which scholars (Barrett, Bauer, Lindars, Frey, Thyen) argue John writes for an audience already familiar with the Synoptic story, hence dependence/posteriority rather than priority?`
  - **Specifiek:** C.K. Barrett, Jörg Frey, Hartwig Thyen [30-32] (literaire/theologische afhankelijkheid van de synoptici; eindvorm jaren 90, "spirituele" her-editie voor een synoptisch geïnformeerd publiek); F.C. Baur [33] (Johannes als late synthese van Marcus en Lucas); Barnabas Lindars [30,34,35] (gefaseerde redactie die op gevestigde traditie voortbouwt); Richard Bauckham en Urban C. von Wahlde [1-3,19] (Johannes schreef "voor lezers van Marcus" en voegde correlerende glossen in). Verzen Joh 3:24; 6:67-71; 11:2; 21:2.
  - **Raakt as:** datering · **Aard:** secundair · **Primair nagezien:** ja (Joh 3:24 grondtekst, zie volgende entry)
  - **Commando:** n.v.t. (notebook)
  - **Opgehaald:** ja · **Type:** literair/relatieve chronologie
- **Claim:** De glosse Joh 3:24 ("οὔπω γὰρ ἦν βεβλημένος εἰς τὴν φυλακὴν ὁ Ἰωάννης") gebruikt de periphrastische plusquamperfectum ἦν βεβλημένος en verwijst terug naar een gevangenneming die Johannes zelf nergens vertelt; dat veronderstelt lezerskennis van buiten de tekst.
  - **Bron:** https://biblehub.com/interlinear/john/3-24.htm
  - **Specifiek:** interlineaire grondtekst Joh 3:24; οὔπω (nog niet), γὰρ (want), ἦν βεβλημένος (was geworpen, perifrastisch plusquamperfectum), εἰς τὴν φυλακήν (in de gevangenis), ὁ Ἰωάννης (Johannes).
  - **Raakt as:** datering · **Aard:** primair · **Primair nagezien:** ja (biblehub interlinear; de Griekse vorm staat er letterlijk; NT zit niet in de brontekst-databases Sefaria/Perseus)
  - **Commando:** n.v.t. (NT via biblehub)
  - **Opgehaald:** ja · **Type:** grammaticaal/syntactisch

### 🏛️ Grieks-Romeins
- **Claim:** De afscheidsredes (Joh 13-17) zijn gevormd naar het Grieks-Romeinse symposion en de troostrede (consolatio): de geliefde leerling aan Jezus' boezem (13:23) als symposiastische ereplaats naast de gastheer; de φιλία/ἀγάπη-discours (15:13-15, sterven voor de vrienden, φίλοι niet δοῦλοι) als symposion-stof; "laat uw hart niet ontroerd worden" (14:1) als consolatio-topos.
  - **Bron:** nlm "John - exegesis", query: `Do commentators read the Johannine Farewell Discourses (John 13-17), set at a reclining supper, as shaped by Greco-Roman SYMPOSIUM literature and the genre of CONSOLATION (consolatio/Trostrede) and the philosopher's farewell to his friends before death (like Socrates in Plato's Phaedo and Symposium)? Discuss George Parsenios 'Departure and Consolation', the beloved disciple reclining in Jesus' bosom (en to kolpo, 13:23) as symposiastic reclining, the discourse on friendship/love (philia, 15:13-15 'lay down his life for his friends', calling them philoi not douloi), and 'let not your hearts be troubled' (14:1) as consolation topos. Which scholars connect John 13-17 to the symposium and consolatory literature rather than to a Jewish farewell/testament model?`
  - **Specifiek:** George L. Parsenios (*Departure and Consolation*) [3,5], Paul A. Holloway [3], Manfred Lang [3,5], Jo-Ann A. Brant [31], Dennis E. Smith [32,33], Harold W. Attridge [34], Charles B. Puskas [34], George Kennedy [1]; *triclinium*-aanligging en "en tō kolpō" (13:23) als ereplaats [4,14,16,17]; φιλία/parrēsia-discours en δοῦλοι→φίλοι (15:13-15) [21-30]; "naast joodse testament-tradities" als gemengd model [1,35-37]. Verzen Joh 13:23; 14:1; 15:13-15.
  - **Raakt as:** karakter · **Aard:** secundair · **Primair nagezien:** ja (Plato Symposion 175, zie volgende entry)
  - **Commando:** n.v.t. (notebook)
  - **Opgehaald:** ja · **Type:** literair
- **Claim:** Plato's Symposion verifieert de symposiastische bouwsteen primair: de gastheer nodigt de wijze uit om naast hem aan te liggen op de ereplaats, en het werk is in zijn openingszin "de redevoeringen over de liefde" gehouden "tijdens het gastmaal", precies het genre dat Joh 13-17 uitvoert.
  - **Bron:** Perseus/Scaife, Plato *Symposion* passage 175
  - **Specifiek:** "δεῦρ', ὦ Σώκρατες, παρ' ἐμὲ κατάκεισο, ἵνα καὶ τοῦ σοφοῦ ἁπτόμενός σου ἀπολαύσω" (Agathon nodigt Sokrates op de ereplaats naast zich); aanlig-werkwoorden κατακλίνου / κατάκεισο / κατάκλισις; openingsframe "τῶν ... ἐν τῷ συνδείπνῳ παραγενομένων, περὶ τῶν ἐρωτικῶν λόγων". Beide formuleringen staan woordelijk in de opgehaalde Griekse tekst.
  - **Raakt as:** karakter · **Aard:** primair · **Primair nagezien:** ja (Perseus grc2, passage 175; ref "175c" faalde in het schema, passage-ref "175" gaf de juiste tekst)
  - **Commando:** `./.agents/tools/brontekst perseus "urn:cts:greekLit:tlg0059.tlg011.perseus-grc2:175"`
  - **Opgehaald:** ja · **Type:** literair

### ✡️ Joods
- **Claim:** De johanneïsche "Geest der waarheid" (Joh 14:17; 15:26; 16:13) en de licht-duister-dualistiek (1:5; 3:19-21; 8:12; 12:35-36) met "kinderen van het licht" (12:36) hebben hun matrix in de Verhandeling over de Twee Geesten van 1QS (geest van waarheid tegenover geest van onrecht, Vorst van het Licht tegenover Engel van de Duisternis, zonen van het licht); Qumran is de enige voor-christelijke joodse vindplaats van de titel "Geest der waarheid". Dit sluit de oudere hellenistisch-filosofische/gnostische verklaring af. Tevens weerlegging van de symposion-lezing van Joh 13-17 (de leerstellige kern van die hoofdstukken is qumranisch, niet Platoons).
  - **Bron:** nlm "John - exegesis", query: `The Paraclete in John's Farewell Discourse is called 'the Spirit of truth' (to pneuma tes aletheias, John 14:17; 15:26; 16:13). Which commentators argue that John's 'spirit of truth' and his light/darkness, truth/falsehood, sons of light dualism (John 1:5; 3:19-21; 8:12; 12:35-36) closely parallel the Qumran Community Rule's Treatise of the Two Spirits (1QS 3-4), the spirit of truth versus the spirit of deceit, indicating a Palestinian-Jewish/sectarian matrix rather than a Hellenistic/Greek one? Discuss James Charlesworth, Raymond Brown, John Ashton on John and Qumran dualism, the 'sons of light' (huioi photos, John 12:36), and whether this dualism is Jewish-apocalyptic rather than Greek-philosophical.`
  - **Specifiek:** Raymond E. Brown (Qumran biedt de dichtste ideologische/terminologische parallellen; maakt hellenistisch-oosterse gnostische achtergrond overbodig) [3,8,19,20,21]; James H. Charlesworth (mapt 1QS 3:13-4:26 punt voor punt: "Spirit of Truth", "sons of light", "light of life", "walking in darkness"; mogelijk directe ontlening/voormalige Essenen in de johanneïsche school) [22-26]; John Ashton (de evangelist had qumranische dualistiek "in his bones"; mogelijk Esseense bekeerling) [2,4,27-29]; "dualism of decision" als johanneïsche transformatie [27,30-32]. Verzen Joh 14:17; 15:26; 16:13; 1:5; 3:19-21; 8:12; 12:35-36.
  - **Raakt as:** karakter · **Aard:** secundair (commentaar) + primair (1QS via DZR-notebook) · **Primair nagezien:** ja (via notebook "De Complete Dode Zeerollen (English)", Engelse vertaling: 1QS Verhandeling over de Twee Geesten bevat letterlijk "the spirits of truth and injustice", "those born of truth spring from a fountain of light, but those born of injustice spring from a source of darkness", "the Prince of Light"/"the Angel of Darkness", "children of light"; query: `Does the Community Rule (1QS), specifically the Treatise of the Two Spirits (columns 3-4), contain the exact phrase 'spirit of truth' versus 'spirit of deceit/falsehood/perversity', and a dualism of light and darkness, sons of light versus sons of darkness, and walking in the ways of truth versus falsehood? Quote the literal lines about the two spirits, the Prince of Light / Angel of Darkness, and the spirit of truth.`)
  - **Commando:** n.v.t. (1QS staat niet in Sefaria/Perseus; getoetst via DZR-notebook, Engelse vertaling)
  - **Opgehaald:** ja · **Type:** literair/exegetisch
- **Claim:** De aanligvorm "ἐν τῷ κόλπῳ" (Joh 13:23) is bij een Pesach-maal (13:1) de halachisch voorgeschreven seder-houding (heseb), niet specifiek de Griekse symposion-ereplaats; reclining is een gedeelde, geen Grieks-exclusieve aanwijzing.
  - **Bron:** Sefaria, Mishnah Pesachim 10:1
  - **Specifiek:** woordelijk וַאֲפִלּוּ עָנִי שֶׁבְּיִשְׂרָאֵל לֹא יֹאכַל עַד שֶׁיָּסֵב ("zelfs de armste in Israël eet niet voordat hij aanligt, zoals vrije en welgestelde mensen aanliggen wanneer zij eten").
  - **Raakt as:** karakter · **Aard:** primair · **Primair nagezien:** ja (de zin staat letterlijk in de opgehaalde Hebreeuwse en Engelse tekst)
  - **Commando:** `/Users/ckleier/Desktop/projects/studiedag_ad_fontes/.agents/tools/brontekst sefaria "Mishnah Pesachim 10:1"`
  - **Opgehaald:** ja · **Type:** halachisch/liturgisch

### ⚖️ Moderator (verificatie, ronde 3)
- **Lezing klopt tegen primaire tekst?** Grieks-Romeins' scharnierclaim dat Plato's Symposion 175 het aanliggen-naast-de-gastheer-om-zijn-wijsheid-te-delen attesteert → bevestigd. De tekst bevat woordelijk "δεῦρʼ ... Σώκρατες, παρʼ ἐμὲ κατάκεισο, ἵνα καὶ τοῦ σοφοῦ ἁπτόμενός σου ἀπολαύσω" plus de aanligwerkwoorden κατακλίνου/κατάκεισο/κατάκλισις.
  - **Commando:** `/Users/ckleier/Desktop/projects/studiedag_ad_fontes/.agents/tools/brontekst perseus "urn:cts:greekLit:tlg0059.tlg011.perseus-grc2:175"`
- **Lezing klopt tegen primaire tekst?** Joods' counter dat aanliggen bij Pesach de halachisch voorgeschreven seder-houding is → bevestigd. Mishnah Pesachim 10:1 bevat woordelijk וַאֲפִלּוּ עָנִי שֶׁבְּיִשְׂרָאֵל לֹא יֹאכַל עַד שֶׁיָּסֵב ("zelfs de armste in Israël eet niet voordat hij aanligt, zoals vrije en welgestelde mensen aanliggen wanneer zij eten"). Beide primaire teksten houden stand, waardoor het aanligdetail zichzelf opheft als karakter-aanwijzing: het is gedeeld mediterraan, niet onderscheidend.
  - **Commando:** `/Users/ckleier/Desktop/projects/studiedag_ad_fontes/.agents/tools/brontekst sefaria "Mishnah Pesachim 10:1"`
- **Lezing klopt tegen primaire tekst?** Laats datering-scharnier dat Joh 3:24 een periphrastische plusquamperfectum ἦν βεβλημένος bevat die terugverwijst naar een niet-verhaalde arrestatie → de vorm is bevestigd ("οὔπω γὰρ ἦν βεβλημένος εἰς τὴν φυλακὴν ὁ Ἰωάννης"), maar dat zij externe lezerskennis veronderstelt is een interpretatieve stap die de grondtekst zelf niet beslecht.
  - **Commando:** WebFetch https://biblehub.com/interlinear/john/3-24.htm (NT zit niet in de brontekst-databases)
- **Overig:** Geen citaat oogde verzonnen; notebook-toeschrijvingen waren concreet (auteur plus vers). Het 1QS-materiaal ("Geest der waarheid", Verhandeling over de Twee Geesten) is via het notebook "De Complete Dode Zeerollen (English)" aangevoerd, een Engelse vertaling, niet door mij tegen het Hebreeuwse/Aramese grondcorpus hertoetst; het weegt als sterk maar niet als volwaardige primaire toets. De papyrologische gegevens (P52, de zesentwintig handschriften, Llewelyn) staan niet in Perseus/Sefaria en zijn niet primair toetsbaar; ze zijn als secundair/catalogus gewogen.

## Ronde 4

### ⏳ Vroeg
- **Claim (weerlegging Laat):** ἄλλον παράκλητον (Joh 14:16) veronderstelt de eerste Paracleet INTERN, namelijk Jezus zelf ("een ander van dezelfde soort"); de verwijzing vergt 1 Joh 2:1 niet. Von Wahlde is hier de betwiste minderheid; bovendien botst Laats coalitie intern: Brown (door Laat ingeroepen voor het traject) houdt evangelie-vóór-brieven en Joh 14:16 volkomen intern, terwijl von Wahlde brief-vóór-evangelie claimt.
  - **Bron:** nlm "John - exegesis", query: `In John 14:16 Jesus promises 'another Paraclete' (allon parakleton). Do commentators argue that the word 'another' (allos, another of the same kind) implies that the FIRST Paraclete is JESUS HIMSELF, so that the reference is INTERNAL to the Gospel and does not require the reader to already know 1 John 2:1 (where Jesus is called our paraclete with the Father)? Which scholars (Carson, Morris, Brown, Keener) read 'another Paraclete' as 'another helper like me, Jesus'? Also: what is the majority scholarly view on the relative order of the Gospel and the Johannine Epistles - did the Gospel come BEFORE the letters (Brown) or do some (von Wahlde) argue the Gospel's final form presupposes the letters? Is this order genuinely contested?`
  - **Specifiek:** Leon Morris [6] (ἄλλος = "another of the same kind", de Geest als "a Counselor like Christ", Jezus de eerste Paracleet); D.A. Carson [2] (voorzichtig met de strikte ἄλλος/ἕτερος-distinctie, maar de context van Jezus' vertrek impliceert dat zij al een Paracleet in Jezus hebben, en Joh 14:16 is "completely internal to the Gospel"); Raymond E. Brown [7,8] ("the one whom John calls 'another Paraclete' is another Jesus"; evangelie-vóór-brieven, 1 Joh als orthodoxe correctie); von Wahlde, Hengel, Schnelle [9,13,14,15] (minderheid: brieven vóór de eindeditie). Verzen Joh 14:16; 1 Joh 2:1.
  - **Raakt as:** datering · **Aard:** secundair · **Primair nagezien:** n.v.t. (notebook; Griekse vormen reeds in Laats ronde-4 log via biblehub bevestigd)
  - **Commando:** n.v.t. (notebook)
  - **Opgehaald:** ja · **Type:** grammaticaal/literair
- **Claim:** Argument uit stilzwijgen op de redactielaag: Joh 11:48 ("οἱ Ῥωμαῖοι ... ἀροῦσιν ἡμῶν καὶ τὸν τόπον καὶ τὸ ἔθνος") is een onverzilverde voorzegging van de val van tempel en volk; Johannes voegt overal elders vervullingsglossen toe (2:21-22; 12:33; 18:32; 21:23) maar hier juist niet. Robinson en Morris gebruiken dit voor een datum vóór 70; het zwijgen zit op Johannes' eigen redactiestem en is daarmee niet dateringsneutraal zoals bewaarde accuratesse.
  - **Bron:** nlm "John - exegesis", query: `Does the Gospel of John ever mention or allude to the actual destruction of Jerusalem and the Temple in AD 70? In John 11:48 the chief priests fear 'the Romans will come and take away both our place (the temple) and our nation' - do commentators note that John, unlike Luke, never adds a fulfillment note that this in fact happened in the war, even though John habitually adds fulfillment/explanatory glosses elsewhere (e.g. 2:22; 12:33; 18:32 'signifying what death he would die'; 21:19)? Is the argument from silence regarding the Temple's destruction used by any scholars (e.g. John A.T. Robinson) to argue for a date before 70? How do commentators read John 11:48 and the irony around the temple's fate?` + https://biblehub.com/interlinear/john/11-48.htm
  - **Specifiek:** John A.T. Robinson [1-4] en Leon Morris [1-4] (argument uit stilzwijgen vóór 70: Johannes' glos-gewoonte 2:21-22, 12:33, 18:32, 21:23 doet bij 11:48 een vervullingsnotitie verwachten; haar ontbreken wijst op vóór de verwoesting); contra D.A. Carson, Andreas Köstenberger, Gail O'Day [9-13] (post-70 dramatische/tragische ironie voor een publiek dat de verwoesting meemaakte). Vers Joh 11:48; 2:21-22; 12:33; 18:32; 21:23.
  - **Raakt as:** datering · **Aard:** secundair + primair · **Primair nagezien:** ja (Joh 11:48 Grieks "καὶ ἐλεύσονται οἱ Ῥωμαῖοι καὶ ἀροῦσιν ἡμῶν καὶ τὸν τόπον καὶ τὸ ἔθνος" staat letterlijk op biblehub; NT zit niet in de brontekst-databases)
  - **Commando:** n.v.t. (NT via biblehub; WebFetch https://biblehub.com/interlinear/john/11-48.htm)
  - **Opgehaald:** ja · **Type:** literair/historisch (argument uit stilzwijgen)
- **Claim:** Symmetrietoets via Lucas: het late kamp dateert Lucas ná 70 omdat Lucas Marcus' "gruwel der verwoesting" (Mc 13:14) redactioneel omzet in expliciete belegeringstaal (Lc 21:20 "Ἰερουσαλὴμ κυκλουμένην ὑπὸ στρατοπέδων"; Lc 19:43 "παρεμβαλοῦσιν χάρακά σοι ... περικυκλώσουσίν σε"); past men datzelfde criterium toe op Johannes, dan ontbreekt elke gebeurtenis-gevormde redactie en wijst de balans naar vóór 70.
  - **Bron:** nlm "Luke - exegesis", query: `Do commentators argue that Luke 21:20-24 ('Jerusalem surrounded by armies', 'trodden down by the Gentiles') and Luke 19:43-44 ('your enemies will set up a palisade/rampart against you and dash you to the ground') are redactionally shaped by the ACTUAL events of the AD 70 Roman siege of Jerusalem, compared with Mark 13:14, and that this vaticinium ex eventu is a major reason for dating Luke AFTER 70? Which scholars make this argument?` + https://biblehub.com/interlinear/luke/21-20.htm + https://biblehub.com/interlinear/luke/19-43.htm
  - **Specifiek:** W.G. Kümmel [4,7] ("certain"/"decisive" dat Lucas terugblikt op de val); Philip F. Esler [8], James R. Edwards [9,10] (circumvallatio en omsingeling verraden de Joodse Oorlog 66-70, datering late jaren 70); Robert C. Tannehill [11,12]; Hans Conzelmann, Rudolf Bultmann [13-15] (Lucaanse redactie in het licht van 70); contra C.H. Dodd [16-20], Leon Morris, David E. Garland [18,21-23], T.W. Manson [19,24,25] (Lucas' belegeringstaal is LXX-ontleend, Jes 29:3, Jer 6:6, Ezech 4, niet specifiek 70). Verzen Lc 21:20-24; 19:43-44; Mc 13:14.
  - **Raakt as:** datering · **Aard:** secundair + primair · **Primair nagezien:** ja (Lc 21:20 "Ἰερουσαλὴμ κυκλουμένην ὑπὸ στρατοπέδων" en Lc 19:43 "παρεμβαλοῦσιν χάρακά σοι ... περικυκλώσουσίν σε" staan letterlijk op biblehub; NT niet in brontekst-databases)
  - **Commando:** n.v.t. (NT via biblehub; WebFetch luke/21-20 en luke/19-43)
  - **Opgehaald:** ja · **Type:** literair/relatieve chronologie

### ✡️ Joods
- **Claim:** Joh 1:51 (engelen "op de Mensenzoon") is een midrasj op Genesis 28:12 die de Hebreeuwse antecedent-ambiguïteit van בּוֹ ("op haar"/de ladder versus "op hem"/Jakob) uitbuit; dezelfde crux is het uitdrukkelijke twistpunt in Genesis Rabbah 68:12. Johannes leest "op hem" en maakt de Mensenzoon tot de nieuwe Betel/hemelpoort. Een Griekse lezer (κλίμαξ vrouwelijk) kan de crux niet zien; het vers veronderstelt Hebreeuwse tekst en Hebreeuwse exegese.
  - **Bron:** nlm "John - exegesis", query: `In John 1:51 Jesus says 'you will see heaven opened and the angels of God ascending and descending upon the Son of Man'. Which commentators argue this is a midrash on Jacob's ladder (Genesis 28:12), and specifically on the rabbinic/targumic reading in Genesis Rabbah 68:12 where the angels ascend and descend 'on him' (bo), i.e. on Jacob/Israel, exploiting the Hebrew ambiguity of the antecedent (the ladder vs Jacob)? Discuss C.F. Burney, Hugo Odeberg, Raymond Brown, J.H. Neyrey, Wayne Meeks on John 1:51, the Son of Man as the locus/gate of heaven replacing Bethel, and Jewish exegetical technique behind this verse.`
  - **Specifiek:** C.F. Burney en Hugo Odeberg [4,7] (directe afhankelijkheid van de "op hem"-lezing; Odeberg: evangelist substitueert Jezus voor Jakob, Mensenzoon gelijktijdig in hemel en op aarde); Raymond E. Brown [5,8,9] (mechanische substitutie "dubious" want Natanaël is de "ware Israëliet"/Jakob, maar Mensenzoon als nieuwe locus van goddelijke heerlijkheid); Jerome H. Neyrey [10,11] (Mensenzoon = JHWH boven de ladder; Bauckham kritiseert: engelen "op" de Mensenzoon = Jezus neemt plaats van de ladder); Wayne Meeks [12-15] (afdaal/opstijg-schema als exclusieve openbaarder, polemiek tegen Mozes/Henoch); Francis Moloney, D.A. Carson, Dwight Moody Smith [1,16,17] (verschuiving van geografische plaats naar persoon, Jezus als nieuwe Betel/heiligdom). Vers Joh 1:51; Gen 28:12,17.
  - **Raakt as:** karakter · **Aard:** secundair · **Primair nagezien:** ja (Genesis 28:12 bevat letterlijk het ambigue בּוֹ met mannelijk סֻלָּם; Bereshit Rabbah 68:12 bevat woordelijk de machloket "רַבִּי חִיָּא וְרַבִּי יַנַּאי, חַד אָמַר עֹלִים וְיֹרְדִים בַּסֻּלָּם, וְחַד אָמַר עֹלִים וְיֹרְדִים בְּיַעֲקֹב" en de troon-icoon-traditie "אִיקוֹנִין שֶׁלְּךָ חֲקוּקָה לְמַעְלָה")
  - **Commando:** `/Users/ckleier/Desktop/projects/studiedag_ad_fontes/.agents/tools/brontekst sefaria "Genesis 28:12"` en `/Users/ckleier/Desktop/projects/studiedag_ad_fontes/.agents/tools/brontekst sefaria "Bereshit Rabbah 68:12"`
  - **Opgehaald:** ja · **Type:** exegetisch/literair
- **Claim (weerlegging symposion):** Het johanneïsche vriendschapsbegrip (Joh 15:15, de vriend versus de slaaf die "niet weet wat zijn heer doet") volgt het bijbelse patroon van Abraham als vriend van God (אֹהֵב, 2 Kron 20:7; Jes 41:8), wiens vriendschap erin bestaat dat God zijn plan niet voor hem verbergt (Gen 18:17), niet de Grieks-Romeinse symposion-φιλία.
  - **Bron:** brontekst sefaria (eigen primaire toets; geen specifieke auteur uit notebook toegeschreven, eigen exegetische observatie)
  - **Specifiek:** Genesis 18:17 "הַמְכַסֶּה אֲנִי מֵאַבְרָהָם אֲשֶׁר אֲנִי עֹשֶׂה" ("Zal Ik voor Abraham verbergen wat Ik ga doen?"); 2 Kronieken 20:7 "זֶרַע אַבְרָהָם אֹהַבְךָ" ("zaad van Abraham, uw vriend"); Jesaja 41:8 "זֶרַע אַבְרָהָם אֹהֲבִי" ("zaad van Abraham, mijn vriend"). De drieslag vriend-versus-slaaf-plus-onthulling van het geheim van de heer komt overeen met Joh 15:15.
  - **Raakt as:** karakter · **Aard:** primair · **Primair nagezien:** ja (alle drie verzen opgehaald; de term אֹהֵב en de wending in Gen 18:17 staan er letterlijk)
  - **Commando:** `/Users/ckleier/Desktop/projects/studiedag_ad_fontes/.agents/tools/brontekst sefaria "Genesis 18:17"`, `... "II Chronicles 20:7"`, `... "Isaiah 41:8"`
  - **Opgehaald:** ja · **Type:** exegetisch/literair

### 🕰️ Laat
- **Claim:** Het johanneïsche corpus toont een gemeenschapstraject van externe synagoge-crisis (evangelie) naar interne doketische scheuring (1 Joh 2:19; 4:2-3; 2 Joh 7), wat een tientallen jaren oude gemeenschap veronderstelt; commentatoren verwerpen daarom een datum vóór 70 en plaatsen evangelie en brieven samen rond 85-100.
  - **Bron:** nlm "John - exegesis", query: `What is the relative chronological relationship between the Gospel of John and the Johannine Epistles (1-3 John)? Do commentators argue the Gospel was composed BEFORE the Epistles, and that 1 John presupposes the Gospel's theology? What does the schism in 1 John 2:19 ('they went out from us but were not of us') and the anti-docetic polemic (1 John 4:2-3; 2 John 7) imply about the maturity and elapsed lifespan of the Johannine community, and therefore about DATING the Gospel to the late first century rather than before 70? Which scholars (Brown, Schnackenburg, Strecker, von Wahlde, Lieu) discuss the dating sequence Gospel-then-Epistles and the community trajectory?`
  - **Specifiek:** Raymond E. Brown [8,11-15] (Gospel-then-Epistles; evangelie eerst, 1 Joh later als "orthodox commentary" nadat de afgescheidenen het evangelie zelf doketisch lazen); trajectorie extern (synagoge, Joh 9:22; 12:42; 16:2) naar intern (scheuring) [2,3]; "pushes the final composition ... to the late first century (roughly 85-100 CE)", "a pre-70 CE date is widely rejected" [7-10]; Rudolf Schnackenburg [1] (volgorde onzeker, brieven mogelijk tussen mondelinge verspreiding en schriftelijke voltooiing); Georg Strecker [19,20] (2-3 Joh vóór 1 Joh); Judith M. Lieu [21,22] (waarschuwt tegen automatische literaire afhankelijkheid en tegen gedetailleerde gemeenschapsreconstructie). Verzen 1 Joh 2:19; 4:2-3; 2 Joh 7; Joh 9:22.
  - **Raakt as:** datering · **Aard:** secundair · **Primair nagezien:** ja (NT-grondtekst, zie de twee volgende entries)
  - **Commando:** n.v.t. (notebook)
  - **Opgehaald:** ja · **Type:** historisch/sociaal-historisch
- **Claim:** 1 Joh 2:19 (scheuring) en 1 Joh 4:2 (doketische inzet) staan letterlijk in de grondtekst.
  - **Bron:** https://biblehub.com/interlinear/1_john/2-19.htm en https://biblehub.com/interlinear/1_john/4-2.htm
  - **Specifiek:** 1 Joh 2:19 "ἐξ ἡμῶν ἐξῆλθαν, ἀλλ' οὐκ ἦσαν ἐξ ἡμῶν" ("zij zijn uit ons voortgekomen maar waren niet uit ons"); 1 Joh 4:2 "ὁμολογεῖ Ἰησοῦν Χριστὸν ἐν σαρκὶ ἐληλυθότα" ("belijdt dat Jezus Christus in het vlees gekomen is", perfectum participium ἐληλυθότα).
  - **Raakt as:** datering · **Aard:** primair · **Primair nagezien:** ja (beide Griekse clausules staan letterlijk in de opgehaalde interlineair; NT zit niet in de brontekst-databases Sefaria/Perseus)
  - **Commando:** n.v.t. (NT via biblehub)
  - **Opgehaald:** ja · **Type:** grammaticaal/tekstkritisch
- **Claim:** Volgorde-argument von Wahlde: Joh 14:16 "ἄλλον παράκλητον" (een ándere Paracleet) veronderstelt lexicaal een eerste Paracleet, die alleen in 1 Joh 2:1 wordt benoemd (Jezus); de eindvorm van het evangelie veronderstelt dus de theologie van de brief en staat er downstream van.
  - **Bron:** nlm "John - exegesis" (zelfde query als hierboven, Urban C. von Wahlde [16-18]) + https://biblehub.com/interlinear/john/14-16.htm en https://biblehub.com/interlinear/1_john/2-1.htm
  - **Specifiek:** von Wahlde [16,17,18] (interwoven composition; de eindeditie van het evangelie presupponeert de theologie van 1 Joh: "another Paraclete" in Joh 14:16 werkt alleen als het publiek uit 1 Joh 2:1 weet dat Jezus de eerste Paracleet is). Primair: Joh 14:16 "καὶ ἄλλον Παράκλητον δώσει ὑμῖν"; 1 Joh 2:1 "Παράκλητον ἔχομεν πρὸς τὸν Πατέρα, Ἰησοῦν Χριστὸν δίκαιον". Verzen Joh 14:16; 1 Joh 2:1.
  - **Raakt as:** datering · **Aard:** secundair (von Wahlde) + primair (NT-grondtekst) · **Primair nagezien:** ja (ἄλλον Παράκλητον resp. Παράκλητον ... Ἰησοῦν Χριστὸν δίκαιον staan letterlijk in de opgehaalde interlineair)
  - **Commando:** n.v.t. (NT via biblehub)
  - **Opgehaald:** ja · **Type:** grammaticaal/literair

### 🏛️ Grieks-Romeins
- **Claim:** Joh 9:6 (Jezus geneest de blindgeborene met speeksel-slijk op de ogen) staat in het Grieks-Romeinse topos van de goddelijke genezer die met speeksel de ogen van een blinde herstelt; bekendste parallel is Vespasianus' genezing van een blinde te Alexandrië op aanwijzing van Serapis. Johannes presenteert Jezus als de genezer die keizer en heilgod evenaart en overtreft (theios anēr).
  - **Bron:** nlm "John - exegesis", query: `Does the healing of the man born blind in John 9 (Jesus spits on the ground, makes clay/mud from saliva, and anoints the blind man's eyes, John 9:6) parallel the Greco-Roman miracle tradition of healing with spittle? Specifically the famous healing by the emperor Vespasian of a blind man in Alexandria using saliva, reported by Tacitus (Histories 4.81) and Suetonius (Vespasian 7), associated with the god Serapis. Also discuss the pool of Bethesda/Bethzatha (John 5) with its porticoes where the sick lay waiting for the water to be stirred, in relation to Greco-Roman healing sanctuaries (Asclepieia, incubation, the cult of Asclepius/Serapis). Which commentators connect John's healing signs to the Greco-Roman divine healer (theios aner) and healing-cult topos?`
  - **Specifiek:** Vespasianus-parallel via Tacitus *Hist.* 4.81, Suetonius *Vesp.* 7, Cassius Dio, verbonden aan Serapis [2-7]; Asclepius-genezing met oogzalf [7]; speeksel als geneeskrachtig (Plinius) [2,8]; "presents and supersedes" [4]. Theios-anēr-paradigma: Rudolf Bultmann (semeia-bron als theios-anēr-christologie) [22-24]; David L. Tiede, Carl R. Holladay, Eugene Gallagher (waarschuwen tegen te strakke toepassing) [28,29]; D. Moody Smith, Willem Nicol, Heinz-Wolfgang Kuhn, Anthony Giambrone [21,29-31]; vergelijking Apollonius van Tyana [20,21]. Verzen Joh 9:6; 5:2-9.
  - **Raakt as:** karakter · **Aard:** secundair · **Primair nagezien:** ja (Suetonius, zie volgende entry)
  - **Commando:** n.v.t. (notebook)
  - **Opgehaald:** ja · **Type:** historisch/literair
- **Claim:** Suetonius attesteert de speekselgenezing van een blinde door Vespasianus op aanwijzing van Serapis primair; staat woordelijk in de opgehaalde Latijnse tekst.
  - **Bron:** Perseus/Scaife, Suetonius *Divus Vespasianus* 7
  - **Specifiek:** "e plebe quidam luminibus orbatus, item alius debili crure sedentem pro tribunali pariter adierunt orantes opem valitudini demonstratam a Serapide per quietem: restituturum oculos, si inspuisset ... extremo hortantibus amicis palam pro contione utrumque temptavit, nec eventus defuit." De blinde (luminibus orbatus), de Serapis-droom en het bespuwen (inspuisset) van de ogen staan woordelijk.
  - **Raakt as:** karakter · **Aard:** primair · **Primair nagezien:** ja (Perseus lat2, de passage staat er letterlijk)
  - **Commando:** `/Users/ckleier/Desktop/projects/studiedag_ad_fontes/.agents/tools/brontekst perseus "urn:cts:latinLit:phi1348.abo020.perseus-lat2:7"`
  - **Opgehaald:** ja · **Type:** literair/historisch
- **Claim:** Joh 5 (Bethesda/Bethzatha, vijf zuilengangen, zieken die wachten tot het water beweegt) volgt het incubatiepatroon van de Asclepius-/Serapis-heilsanctuaria; bij de St.-Annakerk te Jeruzalem zijn grotten, Serapis-votieven en resten van een tweede-eeuws asklepion gevonden.
  - **Bron:** nlm "John - exegesis" (zelfde query als hierboven)
  - **Specifiek:** Antoine Duprez (Bethesda als asklepion-serapeum; Johannes ensceneert Jezus' suprematie) [25-27]; Anthony Giambrone (Bethesda als gememorialiseerd asklepion) [21,29-31]; archeologen Jodi Magness, Jean-Baptiste Humbert, Rousée [21,29-31]; incubatie aan Asclepieia/Serapeia [9,13,14]. Vers Joh 5:2-9.
  - **Raakt as:** karakter · **Aard:** secundair · **Primair nagezien:** n.v.t. (archeologie/site staat niet in Perseus/Sefaria)
  - **Commando:** n.v.t. (notebook)
  - **Opgehaald:** ja · **Type:** archeologisch/historisch
- **Claim (weerlegging Joods, Joh 1:51):** Johannes bewaart de Hebreeuwse בּוֹ-ambiguïteit niet maar lost haar op tot ἐπὶ τὸν υἱὸν τοῦ ἀνθρώπου, een afgeronde christologische middelaarsuitspraak die zonder Hebreeuws te begrijpen is; de op- en neerdalende engelen op één middelaarsfiguur is de hellenistisch-joodse/middenplatoonse as-mundi-kosmologie (Philo, De Somniis 1). Substraat Hebreeuws toegegeven; eindkarakter Grieks.
  - **Bron:** eigen tekstargument op basis van het werkdossier; Philo-verwijzing niet primair geverifieerd deze ronde.
  - **Specifiek:** Joh 1:51 grondtekst ἐπὶ τὸν υἱὸν τοῦ ἀνθρώπου (geen open antecedent); κλίμαξ vrouwelijk (Joods' eigen punt); Philo *De Somniis* 1 (ladder als met zielen/daimones gevulde lucht) genoemd maar niet opgehaald.
  - **Raakt as:** karakter · **Aard:** secundair (eigen exegese) · **Primair nagezien:** nee (Philo De Somniis 1 niet via Perseus opgehaald: tlg0018-URN's gaven 404)
  - **Commando:** poging mislukt: `brontekst perseus "urn:cts:greekLit:tlg0018.tlg028.perseus-grc2:1.133"` (404)
  - **Opgehaald:** nee · **Type:** exegetisch/literair

### ⚖️ Moderator (verificatie, ronde 4)
- **Lezing klopt tegen primaire tekst?** Joods' karakter-spil dat Joh 1:51 de Hebreeuwse בּוֹ-ambiguïteit van Genesis 28:12 uitbuit, het twistpunt van R. Chiyya en R. Yannai in Genesis Rabbah 68:12 → bevestigd. De machloket staat woordelijk: רַבִּי חִיָּא וְרַבִּי יַנַּאי, חַד אָמַר עֹלִים וְיֹרְדִים בַּסֻּלָּם וְחַד אָמַר עֹלִים וְיֹרְדִים בְּיַעֲקֹב ("de een zei: opstijgend en neerdalend op de ladder, de ander: op Jakob"), met de icoon-traditie אִיקוֹנִין שֶׁלְּךָ חֲקוּקָה לְמַעְלָה. Genesis 28:12 bevat het ambigue בּֽוֹ letterlijk. Joods' midrasj-claim houdt volledig stand.
  - **Commando:** `/Users/ckleier/Desktop/projects/studiedag_ad_fontes/.agents/tools/brontekst sefaria "Bereshit Rabbah 68:12"` en `... sefaria "Genesis 28:12"`
- **Lezing klopt tegen primaire tekst?** Premisse van Vroegs datering-symmetrie, dat Lc 21:20 expliciete belegeringstaal bevat → bevestigd. Het Grieks luidt "Ὅταν δὲ ἴδητε κυκλουμένην ὑπὸ στρατοπέδων Ἰερουσαλήμ ..." ("wanneer u Jeruzalem door legerkampen omsingeld ziet"). De Lucas-helft van de symmetrie rust dus op een echte tekst (al kan de taal Septuagintaal van oorsprong zijn, zoals Vroeg zelf concedeert).
  - **Commando:** https://biblehub.com/interlinear/luke/21-20.htm (NT zit niet in de brontekst-databases)
- **Lezing klopt tegen primaire tekst?** Grieks-Romeins' nieuwe primaire claim, dat Suetonius *Divus Vespasianus* 7 de speekselgenezing van een blinde via Serapis attesteert → bevestigd. Woordelijk: "e plebe quidam luminibus orbatus ... orantes opem valitudini demonstratam a Serapide per quietem: restituturum oculos, si inspuisset ... palam pro contione utrumque temptavit, nec eventus defuit." De Vespasianus-parallel bij Joh 9:6 staat.
  - **Commando:** `/Users/ckleier/Desktop/projects/studiedag_ad_fontes/.agents/tools/brontekst perseus "urn:cts:latinLit:phi1348.abo020.perseus-lat2:7"` (de in ronde 4 door de opponent gebruikte abo010-URN gaf 404; de juiste levensnummering is abo020)
- **Overig:** Geen citaat oogde verzonnen; notebook-toeschrijvingen waren concreet. Grieks-Romeins markeerde zijn Philo *De Somniis* 1-steun zelf eerlijk als niet-opgehaald (Perseus-URN's 404), zodat de middelaarsduiding op bewering rust en lichter weegt; de asklepion-archeologie bij Bethesda is tweede-eeuws en blijft een gevolgtrekking.

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
