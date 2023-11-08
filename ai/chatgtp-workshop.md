# Opzet ChatGTP workshop

:::{admonition} Over de workshop

Het doel van de workshop is om (PO/VO) docenten kennis te laten maken met ChatGPT, 
op zo'n manier dat ze er zelf mee aan de slag kunnen gaan in hun onderwijs-praktijk.

Docenten die deze workshop gedaan hebben, het achtergrondmateriaal bestudeerd hebben,
en een redelijk aantal uren (tenminste 10) zelf geëxperimenteerd hebben, kunnen deze
workshop ook geven voor hun collega-docenten. Bij de voorbereiding kan het i&i-team
ondersteuning bieden. Vragen en opmerkingen bij dit materiaal zijn welkom:
we proberen deze workshop steeds te verbeteren en bij-de-tijd te houden.
:::

Indeling:

| *duur (min)* | *onderdeel* | *wie* |
| :---   | :---        | :---- |
| 10     | Presentatie: ChatGPT: wat, waarom, hoe?   | |
| 20     | Zelf (experimenteel) aan de slag (1)      | deelnemers |
| 10     | Presentatie: Beperkingen, ethisch gebruik | |
| 10     | vragen, gesprek hierover                  | |
| 10     | Presentatie: ChatGPT voor onderwijs       | |
| 20     | Zelf (gestructureerd) aan de slag (2)     | deelnemers |
| 10     | Afronding, volgende stappen               | |


De onderdelen "Zelf aan de slag" bestaan uit een korte instructie, 
waarna de deelnemers ca. 15 minuten aan de slag gaan.
Aan het eind van zo'n onderdeel kun je 5 minuten vragen naar de ervaringen,
zowel positieve als negatieve.

## Zelf aan de slag (1)

Bij dit onderdeel ga je zelf experimenteren met ChatGPT.
Stel vragen die je kunnen helpen bij je dagelijkse praktijk, voor school of voor thuis.
Of ga op de creatieve toer, bijvoorbeeld met gedichten of met fantasie-verhalen.
Als het eerste antwoord je niet helemaal bevalt, vraag dan om het aan te passen:
je voert een gesprek om tot het gewenste resultaat te komen.

Dit soort experimenten is belangrijk om een gevoel te krijgen voor de manier
waarop ChatGPT werkt: wat werkt wel, wat werkt niet.

Houd er rekening mee dat ChatGPT soms "hallucineert", en misschien wel een plausibel,
maar niet een "waar" antwoord geeft. En denk eraan dat ChatGPT niet deterministisch
is: eenzelfde vraag kan verschillende antwoorden geven.

## Beperkingen en ethisch gebruik

### ChatGPT heeft een grillige grens

:::{figure} ../assets/chatgpt-grillige-grens.drawio.png
:width: 400
:align: center

ChatGPT: grillige grens
:::

ChatGPT geeft, net als andere LLMs, een plausibel antwoord - maar dat is niet altijd *waar*.
Soms is het compleet bedacht: CHatGPT "hallucineert".

Zo kan ChatGPT refereren aan een boek of artikel van een bepaalde auteur.
De titel in combinatie met de auteur is plausibel: 
zij zou dat artikel geschreven kunnen hebben.
Ook de referentie voldoet aan alle regels voor referenties.
Maar het gaat om een niet-bestaand artikel.

Je kunt niet van te voren zeggen of ChatGPT een bepaalde taak naar behoren zal uitvoeren.
Door te experimenteren kun je een zekere intuïtie daarvoor opbouwen, maar ChatGPT heeft
een *grillige grens* tussen wat wel en wat niet werkt. 
Je moet altijd controleren of het resultaat klopt, 
soms word je aangenaam verrast, en soms zul je je "snijden aan de rafelrand".

* 


## Zelf aan de slag (2)

In plaats van een "vrije prompt" kun je ook gebruik maken van een *gestructureerde prompt*.
Deze bevat een aantal elementen waarmee je de interactie tussen ChatGPT en de gebruiker stuurt.
Typische elememten zijn: de persona (rol) voor ChatGPT, de taak in detail beschreven,
de context (extra invoer e.d.), de regels waaraan de uitvoer moet voldoen.

In het boek staan veel gestructureerde prompts beschreven, voor allerlei soorten taken,
vooral gericht op onderwijs.
In het document {doc}`./prompts.md` vind je een aantal 
voorbeelden van Mollick & Mollick, gericht op onderwijs, 
voor zowel docent als leerling (student). 


## Achtergrondmateriaal

Er zijn zeer veel video's en blogs, goede en minder goede, waar je informatie over
het gebruik van ChatGPT voor het onderwijs kunt vinden.

De belangrijkste bronnen die wij gebruikt hebben (en nog steeds gebruiken):

### Boek

Het boek "Chatten met Napoleon" geeft een goede start voor het gebruik van ChatGPT
in het onderwijs. De verschillende aspecten van dit gebruik, inclusief ethiek
en beleid, komen hierin aan de orde. Lezen! (...dat is nog steeds niet ouderwets...)

* https://www.boomhogeronderwijs.nl/product/100-14318_Chatten-met-Napoleon

### Video's

Ethan Mollick en Lilach Mollick hebben een reeks korte video's (samen ca. 1 uur) over
*Practical AI for Teachers and Students*, gericht op LLMs in het algemeen
en ChatGPT in het bijzonder.

* https://www.youtube.com/playlist?list=PL0EdWFC9ZZrUAirFa2amE4Hg05KqCWhoq

`code.org` heeft een vergelijkbare reeks video's: AI 101 voor docenten.
Je vindt daar ook meer inhoudelijke video's over LLMs en AI in het algemeen.

* https://code.org/ai/pl/101

De onderstaande video geeft een goed inzicht in de plannen van de Khan Academy voor de inzet
van ChatGPT als *tutor* (Khan Migo).

* Harnessing AI for education: https://www.youtube.com/watch?v=sOWHNKHAMkQ

### Blogs

De blog van Ethan Mollick, https://oneusefulthing.com, is zeer informatief en
geeft veel inzicht in ChatGPT en het gebruik daarvan, in het bijzonder voor het onderwijs.

Voor een technische verdieping, met het nieuwste onderzoek op het gebied van LLMs,
kun je de blog [Ahead of AI](https://magazine.sebastianraschka.com) 
van Sebastian Raschka volgen.
