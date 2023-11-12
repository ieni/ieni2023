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
| 10     | Presentatie: ChatGPT: wat, waarom, hoe?   | inleider(s)|
| 20     | Zelf (experimenteel) aan de slag (1)      | deelnemers |
| 10     | Presentatie: Beperkingen, ethisch gebruik | inleider(s)|
| 10     | vragen, gesprek hierover                  | inleider(s)|
| 10     | Presentatie: ChatGPT voor onderwijs       | inleider(s)|
| 20     | Zelf (gestructureerd) aan de slag (2)     | deelnemers |
| 10     | Afronding, volgende stappen               | inleider(s)|


De onderdelen "Zelf aan de slag" bestaan uit een korte instructie, 
waarna de deelnemers ca. 15 minuten aan de slag gaan.
Aan het eind van zo'n onderdeel kun je 5 minuten vragen naar de ervaringen,
zowel positieve als negatieve.

## ChatGPT: wat, waarom, hoe?

### ChatGPT is een LLM

ChatGPT is een zogenaamd *Large Language Model* (LLM): 
een zeer groot speciaal neuraal netwerk
dat getraind wordt met een enorme hoeveelheid data.
ChatGPT3.5 bevat 175 miljard parameters, onder meer in de vorm van de gewichten in
het neurale netwerk.
ChatGPT3.5 is getraind op zeer veel data: 300 miljard woorden.
Een normaal leesboek bevat zo'n 250-300 woorden per pagina: dat komt dus neer op
zo'n miljard pagina's, ofwel enkele miljoenen boeken.
Veel van deze tekst is afkomstig van het web: denk aan Wikipedia, 
en heel veel andere websites.
ChatGPT4 (en later) is ongeveer een orde (factor 10) groter, maar daarvan zijn veel
minder gegevens bekend.

Al deze data wordt gebruikt voor met maken van een groot *statistisch taalmodel*, 
dat steeds een plausibel volgend woord kiest bij de tekst die tot nu toe ingevoerd en
gegenereerd is. Je kunt dit zien als "autocompletion on steroids"

De ChatGPT-aanpak kun je zien als een *brute force* aanpak: het probleem wordt
met zeer veel rekengeweld en zeer veel data aangepakt.
Dit blijkt wel goed te werken - maar misschien kan het ook slimmer?
De komende jaren zullen we het zien: er wordt ook zeer veel onderzoek naar gedaan.

### ...en wat is het niet?

ChatGPT is een *taalmodel*, geen *kennismodel*.
Heel veel kennis is op een impliciete manier in de vorm van taal opgeslagen,
en die kennis wordt door ChatGPT gebruikt om steeds een plausibel antwoord 
te geven.
Maar ChatGPT kan zelf niet nagaan of het antwoord "waar" is of niet;
of wat de feiten zijn waar het antwoord op gebaseerd is, en de redenering.

ChatGPT geeft bovendien niet steeds hetzelde antwoord bij dezelfde invoer:
het is geen deterministisch systeem.

ChatGPT is *getraind*, niet geprogrammeerd.
Het neurale netwerk van ChatGPT is wel geprogrammeerd, 
maar daarna is dit netwerk getraind met zeer veel data.
Het resultaat is een statistisch model, niet een regel-gebaseerd model.
Dit betekent bijvoorbeeld dat ChatGPT geen uitleg kan geven welke regels
gevolgd zijn om tot een bepaald resultaat te komen.

Vergelijking:

* als je leert fietsen, train je je hersenen om op de fiets in evenwicht te blijven,
met vallen en opstaan. 
Je kunt niet uitleggen welke regels je gebruikt om overeind te blijven.
* de verkeersregels leer je op een andere manier, en gebruik je op een andere manier.
Je kunt steeds in een situatie uitleggen wie voorrang heeft, en op grond van 
welke regels dat zo is.

### Waarom ChatGPT?

...het blijkt verbazend goed te werken...

:::{figure} ../assets/chatgpt-examen-resultaten.png
:width: 400

Examenresultaten van ChatGPT
:::

Bill Gates gaf OpenAI de uitdaging om ChatGPT een Biologie-AP examen te laten maken, 
ongeveer vergelijkbaar met onze eindexamens VWO.
Hij koos Biologie omdat het daar niet gaaat om het puur reproduceren van feiten,
maar je moet ook kunnen nadenken en redeneren over Biologie.
Hij dacht dat die uitdaging ze nog wel twee of drie jaar bezig zou houden.
Het werden een paar maanden: zie de groene resultaten van ChatGPT3.5
Dat was voor Gates het teken dat hier van een echte doorbraak sprake was.

Zoals je ziet presteert ChatGPT3.5 al heel behoorlijk voor veel vakken.
ChatGPT4 komt nog flink verder (een half jaar later).

:::{admonition} Achtergrond 
:class: dropdown

Voor inzichten van Bill Gates over OpenAI en ChatGPT, 
zie https://www.gatesnotes.com/The-Age-of-AI-Has-Begun.
Daar vind je ook het volgende:

> The second big surprise came just last year. I’d been meeting with the team
> from OpenAI since 2016 and was impressed by their steady progress. In
> mid-2022, I was so excited about their work that I gave them a challenge:
> train an artificial intelligence to pass an Advanced Placement biology exam.
> Make it capable of answering questions that it hasn’t been specifically
> trained for. (I picked AP Bio because the test is more than a simple
> regurgitation of scientific facts—it asks you to think critically about
> biology.) If you can do that, I said, then you’ll have made a true
> breakthrough.
>
> I thought the challenge would keep them busy for two or three years. They
> finished it in just a few months.

(lees ook vooral de rest).

:::

### Ondersteuning van professionals

:::{figure} ../assets/oneusefulthing-cyborgs.png
:width: 500

Resultaten van consultants zonder en met gebruik van ChatGPT4
:::

De Boston Consultancy Group heeft een wetenschappelijk experiment gedaan:
een groep consultants werd in tweeën gesplitst, 
waarbij de ene groep wel gebruik maakte van ChatGPT4,
en de andere groep niet.
Daarna moesten ze 18 taken uitvoeren die representatief zijn 
voor hun dagelijkse consultancy-werk.

Het resultaat zie je in de grafiek:

* de groep die ChatGPT4 gebruikte had maar 75% van de tijd nodig 
vergeleken met de andere groep;
* de resultaten van deze AI-ondersteunde groep waren ca. 40% beter dan die van de
andere groep.

De resultaten van de AI-ondersteunde consultants waren allemaal beter dan hun
normale niveau, maar dat gold het sterkst voor de gewoonlijk minder presterende
professionals: deze gingen er zeer sterk op vooruit.

Een dergelijke verbetering geen professional en geen bedrijf laten liggen.

:::{admonition} Achtergrond
:class: dropdown

Het experiment met de consultants van de Boston Consultancy Group 
wordt besproken in de blog oneusefulthing: 
[Centaurs and Cyborgs on the jagged frontier](https://www.oneusefulthing.org/p/centaurs-and-cyborgs-on-the-jagged)

> There is a ton of important and useful nuance in the paper but let me tell
> you the headline first: for 18 different tasks selected to be realistic
> samples of the kinds of work done at an elite consulting company,
> consultants using ChatGPT-4 outperformed those who did not, by a lot. On
> every dimension. Every way we measured performance.

Nog enkele opvallende punten:

* zowel menselijke experts als ChatGPT gaven een beoordeling van de resultaten.
Beide waren het vrijwel altijd eens;
* de AI-ondersteunde groep is niet speciaal getraind voor het gebruik van ChatGPT.

:::

### ...soms gaat het mis...

:::{figure} ../assets/chatgpt-grillige-grens.drawio.png
:width: 400

De grillige grens tussen succes en falen van ChatGPT

:::

Het resultaat van ChatGPT is vaak goed, maar soms gaat het subtiel of spectaculair mis.
ChatGPT verzint dan een *plausibel* antwoord dat feitelijk onjuist is.

ChatGPT kan een referentie naar een artikel geven van een bestaande auteur.
De referentie voldoet aan alle eisen van een wetenschappelijke referentie,
en ziet er *plausibel* uit - maar de betreffende auteur heeft het artikel niet geschreven. 
Op grond van haar expertise had ze dat artikel kunnen schrijven - 
maar dat is nooit gebeurd.

Een jurist in de USA is hiermee bij de rechtbank onderuit gegaan: 
de jurisprudentie die hij aanhaalde (via ChatGPT verzameld) was bedacht.

In zo'n geval spreken we wel over het "hallucineren van generatieve AI".

Er is een *grillige grens* tussen wat wel en wat niet goed gaat.
Soms gaat een geval waarvan je denkt dat het relatief eenvoudig is, faliekant mis.
En soms gaat een moeilijk geval verrassend goed.

**Conclusie**: je moet altijd het resultaat van ChatGPT controleren.
Hiervoor heb je goede informatievaardigheden nodig, geholpen door relevante kennis.

:::{admonition} Achtergrond
:class: dropdown

Zie: https://arstechnica.com/tech-policy/2023/06/lawyers-have-real-bad-day-in-court-after-citing-fake-cases-made-up-by-chatgpt/

Voor de "grillige grens" (jagged frontier), zie: 
[Centaurs and Cyborgs on the jagged frontier](https://www.oneusefulthing.org/p/centaurs-and-cyborgs-on-the-jagged)

:::

### Hoe gebruik je ChatGPT?

ChatGPT heeft geen handleiding.

Voor een deel is deze misschien niet nodig, omdat het interface heel eenvoudig is:
je geeft opdrachten in natuurlijke taal, en krijgt antwoord in natuurlijke taal.
(Of, in de vorm van een plaatje, als je daarom vraagt.)

Maar: de makers van ChatGPT weten zelf ook eigenlijk niet hoe het werkt,
en aan welke "knoppen" je kunt draaien om een goed resultaat te krijgen.
Bovendien weten ze helemaal niet hoe ze ChatGPT het best kunnen aanpassen aan
jouw specifieke situatie.

De beste manier is daarom om zelf aan de slag te gaan met ChatGPT,
en te experimenteren met verschillende mogelijkheden.
Na een aantal uren experimenteren krijg je een gevoel voor wat werkt en wat niet.
(Je *traint* op deze manier jezelf in het gebruik van ChatpGPT.)
Je kunt dit het beste doen met je dagelijkse taken, vooral als die wat lastiger
zijn of veel tijd kosten.

Als je een eerste reactie krijgt die je niet bevalt, vraag ChatpGPT dan om een
aanvulling of een verbetering: vraag door en stuur bij totdat je een bevredigend
resultaat krijgt. Je voert een gesprek met ChatpGPT totdat het resultaat goed is
(*conversational prompting*).

(Later in deze workshop ga je aan de slag met *gestructureerde prompts*,
maar probeer eerst zelf uit wat voor jou werkt en wat niet.)

:::{admonition} Achtergrond
:class: dropdown 

In zijn blog [two paths to prompting](https://www.oneusefulthing.org/p/working-with-ai-two-paths-to-prompting)
maakt Ethan Mollick onderscheid tussen *conversational prompting*, 
zoals hier bedoeld, en *structured prompting*.

:::

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
(Je kunt om een ander antwoord vragen door de "regenerate" knop.)

## ChatGTP in het onderwijs

**Kansen, beperkingen en ethisch gebruik**

Drie belangrijke punten bij het gebruik van ChatGPT in het onderwijs:

* ChatGPT is overal (en laagdrempelig) beschikbaar
* ChatGTPT is transformatief - *disruptive innovation*
* het gebruik van ChatGPT is *niet detecteerbaar*

**Overal beschikbaar.** Er zijn allerlei manieren om toegang te krijgen tot 
ChatGPT en andere LLMs, van gratis versies tot betaalde versies.
De gratis versies lopen wat achter in de technologie, maar zijn voor veel doeleinden
ook goed te gebruiken. Zowel OpenAI als Microsoft (Bing) en Google (Bard) 
bieden gratis versies aan.  
Ook de betaalde versies, van bijvoorbeeld OpenAI (ChatGPT 4 Plus) maar ook van
Khan Academy (Khanmigo) zijn voor veel mensen te betalen.
(Die kosten zijn veel lager dan bijlessen of examentraining.)

**ChatGPT is transformatief.** ChatGPT heeft alle kenmerken van een 
*disruptive innovation*: deze zet de bestaande verhoudingen op de kop.
Dit betekent dat je over veel zaken, bijvoorbeeld in het onderwijs, 
op een fundamentele manier moet nadenken wat de betekenis ervan is in een
wereld met AI. (Dit denken is in veel domeinen, bijvoorbeeld in het onderwijs,
nog maar net begonnen.)

**ChatGPT is niet detecteerbaar.** Je kunt niet detecteren dat het resultaat
gemaakt is met behulp van AI. Ook al vallen veel leerlingen nu nog door de mand,
bijvoorbeeld door een taalgebruik dat niet bij hen past, 
dat zal in de nabije toekomst al "gerepareerd" zijn.
(Een voorbeeld is een leerling die aan ChatGPT aangaf dat het resultaat eruit 
moest zien als gemaakt door een dyslectische leerling. 
Het resultaat bevatte precies de fouten die je van zo'n leerling verwacht.)

De figuur hierboven geeft het resultaat van een taal-analyse van afstudeerscripties
van studenten uit Delft. Na de introductie van ChatGPT in november 2022 komen ineens
veel meer minder gangbare Engelse woorden in deze scripties voor.
Dit doet vermoeden dan deze studenten AI gebruikt hebben voor het schrijven van hun
scriptie. 
(Voor zover bekend is heeft deze lichting niet een extra cursus Engels gekregen.)
Een student die zijn taalgebruik wil aanpassen kan ChatGPT gewoon een aantal
voorbeeld-documenten geven, bijvoorbeeld oudere afstudeeerscripties, om dit effect
te vermijden.

Deze punten worden o.a. in de presentaties van Mollick & Mollick genoemd.

Het detecteren van 

## Beperkingen en ethisch gebruik

### 

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

`code.org` heeft een vergelijkbare reeks video's: *AI 101 voor docenten*.
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
