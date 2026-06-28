# Seed-bronnen

Startpunten uit de "Geciteerd werk"-lijst van het achtergrondmateriaal, grof gecategoriseerd.
**Dit is een vertrekpunt, geen volledige lijst.** Opponenten moeten met WebSearch verder zoeken
(o.a. naar peer-reviewed artikelen en primaire teksten) en elke geciteerde bron echt ophalen
(WebFetch) voordat ze hem in het whiteboard zetten. Vermeld bij elke gebruikte bron of je hem
daadwerkelijk hebt geopend.

## Commentaar-notebooks (NotebookLM via de `nlm` CLI), gebruik deze actief
Er staat een set ingelezen bijbelcommentaren klaar als NotebookLM-notebooks, te bevragen met de
`nlm` command-line tool via Bash. Per bijbelboek zitten er tientallen commentaren in. De voor dit
debat relevante notebooks:
- `John - exegesis` (95 bronnen)
- `Luke - exegesis` (99 bronnen)
- `Matthew - exegesis` (63 bronnen)
- `Mark - exegesis` (78 bronnen)
- `Acts - exegesis` (77 bronnen; tweede boek van Lucas, relevant voor de Lucas-datering)

Daarnaast staat er één **primaire-tekstcorpus** klaar (geen commentaar maar de brontekst zelf, in
Engelse vertaling), te bevragen op dezelfde manier:
- `De Complete Dode Zeerollen (English)`, voor Qumran-/Dode Zeerollen-claims (de Gemeenschapsregel 1QS
  en de Verhandeling over de Twee Geesten, 4QMMT, de Hodayot, enzovoort) die niet in Sefaria of de
  Perseus-repos staan, en dus niet via `brontekst` te halen zijn. Dit vult precies het gat dat de
  joods-Palestijnse achtergrond (licht/duister-dualisme, geest van waarheid) anders ongetoetst laat.
  Behandel een treffer als primaire tekst maar markeer dat het een Engelse vertaling via notebook is.

Bevragen (let op de aanhalingstekens rond namen met spaties):
```
nlm cross query "Je concrete vraag" -n "John - exegesis"
nlm cross query "Je vraag" -n "John - exegesis,Luke - exegesis"
nlm notebook list            # overzicht van alle beschikbare notebooks
```
Het antwoord is een gesynthetiseerd commentaar-overzicht met namen van commentatoren (bv. Leon
Morris, D.A. Carson, Stanley Porter, Raymond Brown, Urban von Wahlde). Gebruik dit voor exegetische,
grammaticale en tekstkritische diepgang. Citeer met notebooktitel plus, waar mogelijk, commentaar/
auteur en vers. Deze notebooks zijn doorgaans rijker en betrouwbaarder dan losse webpagina's;
verkies ze boven populaire blogs of Wikipedia. Lukt een query niet, gebruik dan het open web en
vermeld dat.

## Pro vroege datering (datering-as, nuttig voor Opponent Vroeg)
- New theory on the earliest Gospel, University of Cambridge (CSAH): https://www.csah.cam.ac.uk/news/new-theory-earliest-gospel
- Prof. George van Kooten publishes new book on the origins of the Gospels, Clare Hall: https://www.clarehall.cam.ac.uk/news/professor-george-van-kooten-publishes-new-book-on-the-origins-of-the-gospels/
- An Archimedean Point for Dating the Gospels, Brill, *Novum Testamentum*: https://brill.com/view/journals/nt/67/3/article-p310_2.xml
- Evangelie van Johannes – Eerste Evangelie?, Ecclesia: https://www.ecclesianet.nl/publicaties/evangelie-johannes-eerste-evangelie
- Hoe vroeg is het Johannes-evangelie?, Mainzer Beobachter: https://mainzerbeobachter.com/2024/04/09/hoe-vroeg-is-het-johannes-evangelie/
- Reconsidering the Date of John's Gospel, Tom Stegall, CTS Journal: https://www.chafer.edu/CTS-Journal-Reconsidering-the-Date-of-Gospel-of-John
- Evidence for an Early Dating of the Four Gospels: https://evidenceunseen.com/theology/scripture/historicity-of-the-new-testament/evidence-for-an-early-dating-of-the-four-gospels
- Redating the New Testament (John A.T. Robinson), overzicht: https://www.ministrymagazine.org/archive/1978/06/redating-the-new-testament

## Late datering en aposynagōgos (datering-as, nuttig voor Opponent Laat)
- Was John the first gospel?, Psephizo (Ian Paul, kritische bespreking): https://www.psephizo.com/biblical-studies/was-john-the-first-gospel/
- Is the Gospel of John Historical? Dating Evidence and Objections, Cold and Lonely Truth: https://www.cltruth.com/2026/is-gospel-of-john-historical-dating-evidence-objections/
- Dating of John, IssuesWithJohn.com: https://issueswithjohn.com/dating-of-john/
- The Date and Purpose of the Gospel by John, ETS/JETS (Turner): https://etsjets.org/wp-content/uploads/2013/05/files_JETS-PDFs_6_6-3_BETS_6-3_82-85_Turner.pdf
- Strong's Greek 656, ἀποσυνάγωγος (aposynagōgos): https://biblehub.com/greek/656.htm
- Disaffiliation in associations and the ἀποσυναγωγός of John, Kloppenborg (HTS): https://hts.org.za/index.php/hts/article/view/962/1640
- Aposynagōgos and the Historical Jesus in John, Bernier (DTS Voice): https://voice.dts.edu/review/aposynagogos-and-the-historical-jesus-in-john-rethinking-the-historicity-of-the-johannine-expulsion/
- Rethinking the Historicity of the Johannine Expulsion Passages, Bible Interpretation: https://bibleinterp.arizona.edu/articles/2014/06/ber388011
- Birkat ha-minim, The Dustin Martyr Blog: https://dustinmartyr.wordpress.com/tag/birkat-ha-minim/
- Paradigms, Terminology, and Exegesis: Toward a Nonsupersessionist Reading, MDPI *Religions*: https://www.mdpi.com/2077-1444/16/7/868

## Karakter-as (Grieks-Romeins versus joods)
Deze seed-lijst is dateringsgericht. De karakter-opponenten moeten vooral zelf zoeken; enkele
trefwoorden om mee te beginnen:
- **Grieks-Romeins (Opponent Grieks-Romeins):** Richard Burridge, *What Are the Gospels?* (evangelie
  als antieke *bios*); Logos in de Stoa en het middenplatonisme; Philo van Alexandrië; johanneïsche
  ironie en *anagnorisis* (Grieks drama); Justinus de Martelaar en de Logos-christologie.
- **Joods (Opponent Joods):** Logos en *Memra* in de targumim (Alan Segal, *Two Powers in Heaven*);
  feestcyclus en tempeltheologie; Qumran-dualisme (1QS); de onomastiek van Bauckham en Tal Ilan;
  semitismen in het johanneïsche Grieks.

## Recensies van Van Kooten (beide kanten, vaak met tegenargumenten)
- RECENSIE, Nico Riemersma (PDF): https://www.nicoriemersma.nl/storage/blog/Geurt_Henk_van_Kooten_Echos_van_het_goede_nieuws.pdf
- Recensie Echo's van het goede nieuws, Theologie.nl: https://www.theologie.nl/recensie-echos-van-het-goede-nieuws-van-geurt-henk-van-kooten/
- Geurt Henk van Kooten, Echo's van het goede nieuws, Bert Altena: https://www.bertaltena.com/geurt-henk-van-kooten-echos-van-het-goede-nieuws/
- NPO Radio 1, interview/ontdekking: https://www.nporadio1.nl/nieuws/geschiedenis/54b71127-1bf9-4f48-b131-4319fe590762/

## Methodologie / consensus / paradigma (nuttig voor de Moderator-context en meta-argumenten)
- On Scholarly Consensus, Bart Ehrman Blog: https://ehrmanblog.org/on-scholarly-consensus/
- Critical Consensus and Believing Scholarship, Krisis & Praxis: https://krisispraxis.com/archives/2016/03/critical-consensus-and-believing-scholarship/
- Paradigm shift, Wikipedia: https://en.wikipedia.org/wiki/Paradigm_shift
- Thomas Kuhn, paradigm and theology (PDF): https://www.atsjats.org/thomas-kuhn-paradigm-and-theology.pdf

## Primaire teksten, toets secundaire claims hieraan (gebruik dit actief)
Een commentaar (secundaire bron) kan een primaire tekst verkeerd weergeven. Doet een geleerde een
**toetsbare** bewering over een primaire tekst (bv. "Herodotus gebruikt het praesens voor plaats X",
"het Grieks van Joh 5:2 heeft *estin*", "Josephus dateert gebeurtenis Y"), controleer die dan zelf
tegen de primaire tekst voordat je erop leunt, en noteer `aard: primair` en `primair nagezien: ja`.
Dit is het concrete antwoord op de kritiek dat het debat anders blind op secundaire bronnen vaart.

**Voorkeursroute: de `brontekst`-CLI.** Het project heeft een eigen command-line tool die primaire
teksten deterministisch ophaalt uit Sefaria (joodse bronnen) en de Perseus-corpora (klassiek Grieks
en Latijn). Gebruik die boven losse webpagina's. Volledige uitleg, voorbeelden en grenzen staan in
`primaire-bronnen.md`. Kort:
```
brontekst sefaria "Targum Onkelos, Genesis 1:1"                       # joodse tekst (Hebr. + Eng.)
brontekst perseus "urn:cts:greekLit:tlg0016.tlg001.perseus-grc2:1.1"  # klassieke tekst via CTS-URN
brontekst resolve "Sukkah"                                             # juiste Sefaria-ref zoeken
```
De onderstaande webbronnen blijven de terugval als de CLI een tekst niet dekt (bv. de NT-grondtekst,
die je via biblehub/NA28 raadpleegt).

Grieks Nieuwe Testament en kritische tekst:
- Johannes 5:2 (Grieks + interlinear): https://biblehub.com/interlinear/john/5-2.htm
- Johannes 9:22 (aposynagōgos in context): https://biblehub.com/interlinear/john/9-22.htm
- Lucas-parallellen (Lc 7:38; 22:50; 23:4, 14, 22; 23:53; 24:12) via biblehub interlinear of een
  digitale kritische tekst (NA28 waar beschikbaar). Algemeen: https://biblehub.com/interlinear/

Klassieke en antieke teksten (Grieks/Latijn, deels Loeb-afgeleid):
- **Perseus Digital Library** (Grieks/Latijn met woordanalyse): https://www.perseus.tufts.edu/hopper/
- **LacusCurtius** (klassieke teksten, veel Loeb-vertalingen, o.a. de Romeinse auteurs):
  https://penelope.uchicago.edu/Thayer/E/Roman/home.html
- **Lexundria** (doorzoekbare antieke teksten): https://lexundria.com/
- **Herodotus, Historiën** (Perseus, Grieks + Engels): https://www.perseus.tufts.edu/hopper/text?doc=Perseus:text:1999.01.0125
- **Flavius Josephus** (PACE / Perseus): https://pace.webhosting.rug.nl/ en
  https://www.perseus.tufts.edu/hopper/searchresults?q=Josephus
- **Justinus de Martelaar en vroegchristelijke teksten** (relevant voor de Parting of the Ways en
  het Grikser worden van de latere kerk): https://www.earlychristianwritings.com/ en
  https://ccel.org/

Eerlijke grens: een volledige Loeb Classical Library is hier niet beschikbaar. De bovenstaande open
bronnen zijn een gedeeltelijke vervanging. Lukt een primaire toets niet, noteer dan `primair
nagezien: nee` en leun niet zwaarder op de claim dan de secundaire bron rechtvaardigt.
