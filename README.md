# Webdesign-Theorie
Theorie die in de cursus staat

Inhoudstabel  
- [Les 3, Fonts](#les-3-fonts)
- [Les 4, .htaccess](#les-4-htaccess)
- [Les 5, Update mediaqueries](#les-5-update-mediaqueries)


___


## Les 3, fonts:
- Font-stack: de font-families die je instelt op één element, specifiek bedoelt naar de back-up fonts indien eentje ontbreekt
  - Bijvoorbeeld:
  ```css
  p { font-family: 'cowboy_hippie_proregular', sans-serif, cursive; }
  ```
- CDN = Content Delivery Network, wereldwijd netwerk van servers om content (zoals CSS-bestanden) zo snel mogelijk aan eindgebruiker te bezorgen.
Voor developers betekent dit dat ze bv niet zelf de CSS bestanden moeten hosten, scoor
Voorbeelden:
  - Fontawesome (gebruikt \<i class=""\> element voor icons te laden)
  - Google Fonts (gebruikt \<link\> element voor css te laden)
  - Material.io (gebruikt een Google Fonts link voor icons te laden)

___

## Les 4, htaccess
- .htaccess = HyperText Access
- Ondersteund door aantal webservers
- Definieert wat er moet gebeuren bij errors (zoals 404 not found, of 403 forbidden)
- 403, 404 etc. zijn bekend als HTTP statuscodes
- Alhoewel meeste er chill mee zijn, blijkbaar laten sommige hostingproviders .htaccess maar in beperkte mate/helemaal niet toe

___

## Les 5, Update mediaqueries

- Evolutie:
  - Voor 2010: mobiele site = uitgeklede versie van gewone site, 2 versies moesten onderhouden worden
  - 2010 en na: Ethan Marcotte bedacht Responsive Webdesign
    1. Flexibele, op grid (raster) gebaseerde lay-out
    2. Flexibele afbeeldingen/andere media die meeschalen met breder/smaller worden van lay-out
    3. CSS3 media queries om te detecteren op welke breedte de site bekeken wordt (en vervolgens optimaal op te reageren)
- Content first: "alle inhoud moet correct getoond worden op alle apparaten!"
- Mobile first: vertrekken vanaf ontwerp voor een smal scherm (gsm), daarna breder (tablet), daarna breedst (computer)
- Breakpoints: de punten/breedtes wanneer de lay-out zich aanpast (baseer op inhoud, niet op schermgroottes)  
2 breekpunten = 3 lay-outs
- Media query = media attribuut in link tag in head van HTML, dat test op type scherm en (andere kenmerken/features)  
Tip: werk van klein naar groot (no media query, (min-width:500px), (min-width:700px) etc.)
  - Media queries met meerdere CSS bestanden: vele requests bij grote schermen
  - Media queries in CSS: maar één request, maar wel een heel grote (meestal gebruikt in voorbeelden vd cursus)
- Screen query dient ervoor dat de css niet toepast bij bv printen
  

