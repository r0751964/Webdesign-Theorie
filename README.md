# Webdesign-Theorie
Theorie die in de cursus staat

Inhoudstabel  
- [Les 3, Fonts](#les-3-fonts)
- [Les 4, .htaccess](#les-4-htaccess)


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
