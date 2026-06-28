# 📚 Bronnenlog, run {{RUN_NAAM}}

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
