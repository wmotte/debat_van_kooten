# Primaire teksten ophalen met de `brontekst`-CLI

Dit is het concrete gereedschap om Sams tweede kritiek te beantwoorden: toets een secundaire claim
over een primaire tekst aan de **echte primaire tekst** voordat je erop leunt. De CLI haalt teksten
deterministisch op uit twee databases en is, net als `nlm`, bedoeld om via Bash aangeroepen te
worden.

Pad naar de tool (gebruik het absolute pad; je werkmap kan afwijken):
`<repo>/.agents/tools/brontekst` (ook bereikbaar als `.claude/tools/brontekst`, een symlink).
Alleen `python3` nodig, geen installatie.

## Welke database waarvoor
- **Sefaria** = joodse bronnen: Tanakh, targumim (Onkelos, Pseudo-Jonatan, Neofiti waar aanwezig),
  Mishna, Talmoed, midrasj, Ben Sira (Hebreeuwse fragmenten). Voor de Joods-opponent de eerste keus.
- **Perseus/Scaife** = klassiek Grieks en Latijn (Herodotus, Plato, de tragici, Tacitus, Suetonius,
  enzovoort). Voor de Grieks-Romeins-opponent en voor klassieke dateringscomparanda van Vroeg/Laat.
- **Niet** in deze twee: de NT-Griekse grondtekst van Johannes zelf. Blijf daarvoor biblehub
  interlinear / NA28 gebruiken (zie `bronnen.md`). Ook Qumran, Philo en Josephus zitten niet in
  Sefaria; Josephus/Philo staan deels in de Perseus-repos (probeer via Scaife de URN te vinden).
- **Qumran/Dode Zeerollen** (1QS, 4QMMT, Hodayot enz.) staan in geen van beide databases. Toets die
  via het NotebookLM-corpus `De Complete Dode Zeerollen (English)` met
  `nlm cross query "..." -n "De Complete Dode Zeerollen (English)"` en vraag om de letterlijke regels.
  Dit is de brontekst zelf, maar in **Engelse vertaling** en via een notebook (geen Hebreeuwse/Aramese
  grondtekst), dus tag een geslaagde toets als `primair nagezien: ja (via notebook, Engelse vertaling)`
  met de exacte query, niet als een gewone `brontekst`-toets.

## Sefaria
```
brontekst sefaria "Targum Onkelos, Genesis 1:1"        # Hebreeuws + Engels (default)
brontekst sefaria "Mishnah Sukkah 5:1" --lang he       # alleen Hebreeuws
brontekst sefaria "Ben Sira 24:8"                       # faalt netjes als de tekst ontbreekt
brontekst resolve "Sukkah"                              # vind de juiste ref bij twijfel
```
Refs in gewone vorm mogen ("Targum Onkelos, Genesis 1:1"); de tool normaliseert ze. Lukt een ref
niet, gebruik dan eerst `resolve`. Voorbeelden die nuttig zijn voor het karakterdebat: `Targum
Onkelos, Genesis 1:1` (Memra), `Mishnah Sukkah 4:9` / `5:1` (waterlibatie, Soekot), `Genesis 28:12`
(Jakobsladder, vgl. Joh 1:51), `Exodus 33:20` (niemand ziet God, vgl. Joh 1:18).

## Perseus/Scaife
```
brontekst perseus "urn:cts:greekLit:tlg0016.tlg001.perseus-grc2:1.1"     # Herodotus, boek.hoofdstuk
brontekst perseus "urn:cts:latinLit:phi1351.phi005.perseus-lat1:1.1"     # Tacitus, Annales 1.1
brontekst scaife-url "urn:cts:greekLit:tlg0016.tlg001.perseus-grc2:1.1"  # alleen de leeslink
```
De tool haalt de ruwe TEI op (canonical-greekLit / canonical-latinLit, met First1KGreek als
terugval voor Grieks) en snijdt de passage eruit. Werkt voor zowel EpiDoc-opmaak (geneste
`textpart`-divs) als de oudere `div1`/`milestone`-opmaak.

**De URN vind je via de Scaife-bibliotheek:** https://scaife.perseus.org/library/ . Zoek de auteur,
open een editie, en lees de CTS-URN (vorm `urn:cts:greekLit:<textgroup>.<work>.<editie>:<passage>`)
en het citatieschema (bv. boek.hoofdstuk.sectie) af. Exitcode 2 met een oriëntatie-fragment betekent
dat de passage-ref niet in het schema paste: controleer dan de ref via de getoonde Scaife-link.

## Tagging en citeren (verplicht)
Wanneer je een tekst via `brontekst` zelf hebt nagezien, log dan in `sources.md`:
- `aard: primair`
- `primair nagezien: ja`
- `commando:` het exacte `brontekst`-commando dat je draaide (reproduceerbaarheid)

Lukt de toets niet (tekst niet in de database, exitcode 1/2), noteer dan eerlijk `primair nagezien:
nee` en leun niet zwaarder op de claim dan de secundaire bron rechtvaardigt.

## Eerlijke grenzen
- De NT-Griekse grondtekst komt niet uit deze twee diensten (biblehub/NA28 blijft).
- Qumran/Dode Zeerollen lopen via het NotebookLM-corpus `De Complete Dode Zeerollen (English)`, dat een
  Engelse vertaling biedt (niet de grondtekst) en via een notebook gaat, geen deterministische
  tekstophaling zoals `brontekst`; weeg een notebook-toets dus iets lichter dan een directe Sefaria-
  of Perseus-toets.
- Ben Sira op Sefaria is fragmentarisch (Hebreeuwse Genizah-fragmenten); hele hoofdstukken kunnen
  ontbreken. De Griekse Sirach (LXX, relevant voor de skēnoō-parallel met Joh 1:14) staat niet op
  Sefaria; zoek die zo nodig als Septuaginta-tekst via Perseus (`tlg0527`) of een LXX-uitgave.
- Scaifes eigen passage-API is ongelijk gevuld; daarom leunt de tool op de ruwe TEI en blijft Scaife
  vooral de browsebare metgezel en citatielink.
- Een volledige Loeb Classical Library is hier niet beschikbaar; de open corpora zijn een
  gedeeltelijke vervanging.
