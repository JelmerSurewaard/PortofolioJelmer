# PortofolioJelmer

## Stelling

Mijn stelling die ik ga beschrijven is: In het bedrijfsleven wordt steeds meer in software gesimuleerd.

Simulaties worden gebruikt om grafisch weer te geven wat er zou gaan gebeuren in een situatie. Zo kan je beter voorbereiden op bepaalde events. Het is wel lastig om een goede simulatie te maken. Er zijn namelijk veel dingen waar er rekening mee moet worden gehouden. Denk maar aan alle verschillende factoren die er kunnen spelen. Deze factoren hoeven niet alleen maar te limiteren tot het weer, zoals regen, wind, zon of onweer. Dit kan ook bijvoorbeeld het gedrag van bepaalde personen zijn. Zo kunnen mensen in een groepsverband anders reageren dan mensen die alleen lopen. Om een perfecte simulatie te maken, is onmogelijk. Er zijn namelijk te veel variabelen waar rekening mee gehouden moet worden. Daarom moeten er beslissingen worden gemaakt over wat wel en niet wordt gesimuleerd. Zo an er worden gezegd dat mensen maar 2 soorten gedachtes hebben: Ik ben tevreden en Ik ben ontevreden. Zo is het gemakkelijker om het gedrag van deze mensen te simuleren. Tevreden mensen zullen namelijker sneller dingen kopen bijvoorbeeld dan mensen die niet tevreden zijn.  
Er zijn al veel bedrijven die gebruik maken van simulaties om situaties to voorspellen. En met goede redenen natuurlijk. Zo kunnen ze zien wat er anders moet om een positiever resultaat te berijken.

bronnen:

https://blog.designsolutions.nl/hoe-kan-simulatie-software-bijdragen-aan-betere-innovaties
https://www.scientias.nl/mensenmassas-simuleren-voorbereid-op-de-ergste-rampen/
https://en.wikipedia.org/wiki/Business_simulation

## Applicaties die gebruik maken van Json

1. Minecraft.

Json wordt hierbij gebruikt om de informatie van de speler door te sturen naar de server waar deze speler op speelt.

2. Chrome

Json wordt hierbij wederom gebruikt om informatie te sturen naar de server.

3. Steam

Steam gebruikt Json om informatie van de gebruiker door te sturen naar de steam server.


## Wekelijke reflecties

## Week 2

In week 2 hebben we gekeken naar wat we moesten doen. Eerst hebben we een plan gemaakt over wat voor ontwerp we wilden maken voor ons rooster. Dit rooster ontwerp zag er als volgt uit:

![](http://shitposts.nl/img/d6opm.png "Rooster ontwerp")

Hierbij hadden we ook een klassendiagram gemaakt. Hierbij moesten we nadenken over de verschillende eisen die we zelf moesten stellen. Dit hebben we gedaan in een groepsverband. Hieruit kwam de volgende klassendiagram:

![](http://shitposts.nl/img/dvqk7.png "Klassendiagram roostermodule")

In week 2 ben ik begonnen aan een pop-up venster. Dit pop-up venster heeft als functionaliteit om een les in te voeren in het rooster. Voor nu gebruikten we TextIO. Dit hadden we gedaan omdat het makkelijk was om toe te passen en te veranderen.

## Week 3

In week 3 hebben we niet heel veel gedaan.

## Week 4

Na onze demonstratie bleek onze manier van data opslaan niet helemaal goed. We maaktte namelijk gebruik van TextIO ipv. ObjectIO. In deze week ben ik samen met Stijn begonnen om onze datastructuur om te zetten naar ObjectIO. 

Onze situatie was als volgt: We hebben nu een RosterInput die gebruik maakt van TextIO. Dit werkt in principe prima, alleen kan je hierdoor je ingevoerde waardes niet bewerken en verwijderen. Ook kan je zo dubbele objecten maken, wat niet optimaal is. Om dit te fixen, heb ik eerst onze eerste Rosterinput helemaal ge-reworked. In het eerste design was het namelijk onmogelijk om makkelijk veranderingen aan te passen. In het nieuwe model heb ik nu ook ListViews gezet, zodat de objecten die al bestaat duidelijk zijn weergegeven. (hoewel dit nog niet werkt atm.) 

![](http://shitposts.nl/img/4e60t.png "Nieuwe model")

Ook kwam ik tegen het probleem dat mijn paths niet klopte met de paths die mijn groepsgenoten gebruiktte. Na een aantal uur te hebben gewerkt met persoonlijke paths, kwam ik uiteindelijk achter het probleem. Ik had namelijk mijn project een laag te diep gezet in de directory. 

## Week 5

In deze week ben ik verder gegaan aan het verbeteren van onze Roostermodule. Hier kwam ik erachter dat het toch wat meer werk was dan ik eerst dacht. Het idee was om een textfile aan te maken met pathnames naar de object bestanden. Nadat ik zelf een methode had gemaakt om text toe te voegen aan een file, kwam ik erachter dat we al een werkende methode hiervoor hadden. Na een kleine dosis frustatie ging ik dus weer verder met het project. Eerst ging ik aan de slag voor de functionaliteit van de "ADD" button. Elke keer dat er een nieuwe waarde werd toegevoegd, moesten er 3 dingen veranderen: 

* Er moet een objectfile worden aangemaakt die de data van het ingevoegde object opslaat.
* De textfile met pathnames naar deze objectfiles moet worden geupdate.
* Het object moet aan de listview worden toegevoegd, zodat de waarde zichtbaar is voor de gebruiker.

Om dit laatste punt werkend te krijgen heb ik gebruik gemaakt van ObservableLists. Nadat de functinaliteit van de "ADD" button werkte (dit koste echter meer tijd dan ik had gehoopt) ging ik verder met de volgende button: de "Delete" button. Deze button was in principe vrij simpel. Het maakte namelijk gebruik van de vorige logica die ik al had geschreven voor de  "ADD" button. Nu zijn de punten dan iets anders:

* Het objectfile moet worden verwijderd.
* De textfile met pathnames moet worden geupdate.
* Het opject moet van de listview worden verwijderd.

Nadat ik deze button werkend had gekregen, ging ik door naar de laatse button: de "CHANGE" button. Eerst dacht ik dat deze button het moeilijkst zou zijn. Dit bleek echter niet het geval. In principe doet de "CHANGE" button precies hetzelfde als de  "ADD" button. Het enige verschil is dat hij eerst het oude object verwijderd als zowel het bestand als in de observablelist, en gelijk weer toevoegd, maar met de nieuwe waardes.

## Week 6

In deze week heb ik als eerst nog de verandering gedaan dat de lessen ook daadwerkelijk de goede informatie bevatten. Deze informatie bestond voorheen nog uit textfiles bestanen. Nu heb ik het omgezet naar de Object bestanden die we met onze roostermodule aanmaken.

Nadat we weer onze demonstratie hebben gehad, kwam er naar voren dat we nog best wel achter liepen. Ik was tot deze tijd vooral bezig geweest met de roostermodule, maar er moest nog veel gebeuren aan de simulatiemodule. Daarom heb ik hierna ook niks meer aan de roostermodule gedaan, buiten objecten toevoegen, veranderen en verwijderen.

Verder heb ik deze week nog kleine bugs verbeterd, zoals het correct weergeven van de klassen op onze roostermodule, maar daarnaast heb ik niet veel meer gedaan.

## Week 7

In week 7 kwamen we er echt achter dat we nog best ver achter liepen. We hadden een lijst gemaakt met dingen die nog moesten gebeuren. 1 hiervan was de nieuwe map maken. Samen met Pascal ben ik hier mee bezig geweest. Om deze map goed te maken moesten we rekening houden met verschillende dingen:

- Er moeten niet te veel lokalen zijn
- Er moet een aula, docentenruimte, wc en ingang zijn.
- De map moet niet te groot zijn
- Er moet een objectlaag komen waarin alle lokalen een eigen positie hebben
- Er moet een collisionlaag komen waar te zien is waar de collision is. bv. in muren.

Het maken van de map zelf kostte nog best wat tijd. Eerst moesten we namelijk zoeken naar de goede tilesheats. Daarna moesten we de map zelf tekenen en rekening houden met de boven gestelde punten. Uiteindelijk waren we redelijk tevreden met het resultaat:

![](http://shitposts.nl/img/h8t6a.png "Tiled map")

Hierin is te zien hoe we alles hebben opverdeeld. Alles dat een rode tint heeft hoort tot de collision laag. Ook hebben we alle stoelen een groene kleur gegeven. We hebben echter in het plaatje de opacity op 0 gezet van deze groene kleur, want anders zag je de stoelen niet meer. We hadden dit gedaan om zo gemakkelijk de positites van de stoelen te achterhalen.

Nadat we de map hadden gemaakt, kwamen we er achter dat we nog helemaal geen goede maploader hadden. Onze maploader hoefte eerst namelijk maar 1 laag te tekenen. Hier heb ik best veel uur aan moeten besteden om erachter te komen dat het uiteindelijk niet zo heel moeilijk was. Je moest namelijk in plaats van de hele laag doorsturen, een Array van lagen doorsturen. Zo kan hij laag voor laag alles berekenen. Ook heb ik eerst een grote array moeten maken van onze tilesheets. Omdat we er eerst 1 gebruikte, en nu meer, kwamen we erachter dat dit nog voor iets meer moeilijkheden meebracht. Nu het 1 array is met waardes, was het veel makkelijker om uit te lezen. 

Nadat ik de maploader werkend heb gekregen, heb ik ook de Camera aangepast zodat deze ook goed werkt. Dit was in principe niet heel lastig, aangezien we al een goede camera klasse hadden meegekregen in onze eindopdracht voor 2DGraphics. Daarna heb ik heel het simulation project dat we eerst appart hadden onder de simulation tab gezet. Zo kon de simulatie tegelijk met de rootstermodule starten.

## Week 8

In week 8 moesten we echt gaan opschieten. Nu moest er namelijk nog veel functionaliteit komen voor de NPC's. Eerst ben ik samen gaan werken met Lars. We gingen eerst werken aan hoe we verder objecten uit de Jsonfile van de map konden uitlezen. Na heel veel proberen kwamen we eindelijk op een goed resultaat. Omdat het langer duurde echter, was het toen al aan het eind van de dag en hadden we besloten om de volgende dag via discord verder te gaan. 

De volgende dag zijn we verder gegaan en hadden we het voor elkaar gekregen om alle objecten uit te lezen. Hierna zijn we de anderen gaan helpen met hun stukjes. 

Om de studenten naar hun klassen te laten lopen, bleek echter nog best moeilijk te zijn. We hebben met al onze groepsleden er een hele middag aan besteed om hier een oplossing voor te verzinnen. Uiteindelijk was dit een grote methode waarin er heel veel for-loopjes en if-statements worden aangemaakt. Nu liepen de studenten wel naar de goede lokalen, maar liepen ze nog niet naar de goede stoelplekken. 

![](http://shitposts.nl/img/58bcr.png "Big method")

Arno ging hiermee aan de slag, en ik heb hem daar een beetje mee geholpen. Nadat hij dat af had gekregen, ben ik begonnen om de Teachers naar hun lokalen te laten lopen en op hun plekken te laten zitten. Omdat de Teachers ook NPC's zijn net zoals de studenten, was dit minder moeilijk om zelf te bedenken, aangezien er al een groot stuk van de code was gemaakt. Echter bleek het nog wel een uitdaging te zijn om het ook te laten werken voor de Teachers. Na een tijd coderen was het toch in mijn eentje gelukt om de Teachers naar hun eigen plek te laten lopen wanneer ze les hadden.