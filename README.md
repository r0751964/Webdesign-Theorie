# Webdesign Theorie
Theorie die in de cursus staat


[Link naar Theorie Website](https://r0751964.github.io/Webdesign-Theorie/)  
[Link naar Theorie pure tekst, als je dat liever hebt](https://github.com/r0751964/Webdesign-Theorie/blob/master/README.md)

[Link naar Voorbeelden Website](https://r0751964.github.io/Webdesign-Cursus-Voorbeelden/)  
[Link naar Voorbeelden pure tekst, als je dat liever hebt](https://github.com/r0751964/Webdesign-Cursus-Voorbeelden/blob/master/README.md)

[Link naar Handige Links Website](https://r0751964.github.io/Webdesign-Handige-Links/)  
[Link naar Handige Links pure tekst, als je dat liever hebt](https://github.com/r0751964/Webdesign-Handige-Links/blob/master/README.md)  


Inhoudstabel  
- [Les 3, Fonts](#les-3-fonts)
- [Les 4, .htaccess en errorpages](#les-4-htaccess-en-errorpages)
- [Les 5, Update mediaqueries](#les-5-update-mediaqueries)
- [Les 6, Responsieve afbeeldingen](#les-6-responsieve-afbeeldingen)
- [Les 7, Frameworks](#les-7-frameworks)
- [Les 8, Formulieren en formulierafhandeling](#les-8-formulieren-en-formulierafhandeling)
- [Les 9, Samenwerken via Github](#les-9-samenwerken-via-github)
- [Les 10, Bootstrap 4 voor beginners](#les-10-bootstrap-4-voor-beginners)
- [Les 11, Huisstijl en logo](#les-11-huisstijl-en-logo)
- [Les 12, Sass](#les-12-sass)
- [Les 13, CSS3](#les-13-css3)




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

## Les 4, .htaccess en errorpages
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
  
___

# Les 6, Responsieve afbeeldingen

- Welk bestandsformaat?
  - SVG: afbeelding is in paden op te bouwen
    - Is weinig kB (hogere ranking in Google)
    - Geen kwaliteitsverlies in vergoten (handig in responsieve sites)
  - JPG: fotorealistisch materiaal zonder transparantie
  - PNG: foto met transparantie
  GIF: afbeeldingen met weinig kleuren die niet vectorieel te beschrijven zijn (geen svg kunnen zijn)
- Zorg ervoor dat je de afbeelding mag hergebruiken (pexels.com) of (indien jouw eigen foto) dat enige herkenbare mensen erop toestemming geven)
- Hotlink niet (tenzij website het wilt)
- Gewone afbeeldingen: altijd kleiner dan 100kB  
Achtergrondafbeeldingen (schermvullend gebruikt): kleiner dan 200kB  
http://www.picresize.com
- Gebruik height/width niet voor te grote fotos kleiner te weergeven
- Zo weinig mogelijk photoshop, zoveel mogelijk css (bv foto cirkelvormig weergeven)

___

## Les 7, Frameworks

- Voorbeelden
  - Tent.CSS
  - Bootstrap
- Schrijf zo weinig mogelijk CSS (gebruik klassenamen van framework waar mogelijk)
- Wijzijg NOOIT iets in het CSS bestand vd framework (bij updates gaat dan alles verloren)
- Bij Googlen voor hulp met Framework, kijk versie na

___

## Les 8, Formulieren en formulierafhandeling

- Maken website interactiever
- Inhoud formulier: HTML5  
  Opmaak formulier: CSS3
- Formulieren = schakel tussen browser bezoeker & databank website
- Databankacties kunnen gemaakt worden in Java, PHP...
- Methods:
  - get --> gegevens toegevoegd aan URL (niet zo handig voor wachtwoorden)
  - post --> gegevens niet toegevoegd aan URL
- Id moet uniek zijn, begin naam met letter, alleen kleine letters, geen blanco's!
- rgba = rood groen blauw alfawaarde (alfawaarde = transparantie) --> rgba(255, 0, 0, 0.4) in CSS

___

## Les 9, Samenwerken via GitHub

- Git is een versiebeheersysteem waardoor developers tegelijk aanpassingen kunnen maken
- GitHub is een website/hosting service voor software, gebouwd rond Git (alternatieven zijn BitBucket, GitLab, Codebase, Assembla...)

___

## Les 10, Bootstrap 4 voor beginners

- Bootstrap bestaat uit:
  1. General default styles
    - De basispagina ziet er hetzelfde uit in elke browser
    - Er zijn standaard lettertypes en lettergroottes aanwezig
    - Rables, images en figures zijn standaard responsief
  2. Grid layout
    - Ingebouwde flexbox via klassenamen
  3. Predefiend CSS/classes/components
    - Enkel klassenamen moeten gebruiken voor alerts, buttons, cards, forms, navbars... te lay-outen

## Les 11, Huisstijl en logo

Merken: (foto uit cursus H11, slide 7)
![Voorbeelden merken: Woordmerk logo Coca-Cola, beeldmerk logo McDonalds, vormmerk Toblerone chocolade en Legoblok, kleurmerk onderkant schoenen louboutin](img/11.png)

Een goed logo is:
- Eenvoudig
- Herkenbaar
- Tijdloos
- Veelzijdig
- Geschikt voor doelpubliek
- Perfect te printen in grijswaarden
- Vectorieel ontworpen

___

## Les 12, Sass

- Sass = Syntactically Awesome StyleSheets
- Scripttaal, breidt CSS uit
  - Variabelen ($var = "waarde")
  - Functies (lighten())
  - Nesting (div{a{}})
  - Partials (\_variables.scss)
  - Mixins
- Je schrijft sass, sass compiled deze code naar css

___

## Les 13, CSS3

- Prefixes, fabrikanten geven voor sommige experimentele eigenschappen een prefix
  Alleen prefixen indien nodig! (Na te kijken op https://caniuse.com)
  Wordt soms ook afgehandeld door gulp-autoprefixer
  - WebKit (Chrome, Safari, recente Opera versies) -webkit-
  - Mozilla Firefox -moz-
  - Opera (oudere versies) -o-
  - Internet Explorer, Edge -ms-
- Media query voor pixel density (@media (min-resolution: 2dppx){})
- 
  
