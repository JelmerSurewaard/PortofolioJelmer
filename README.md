# PortofolioJelmer

## Week 2

In week 2 ben ik begonnen aan een pop-up venster. Dit pop-up venster heeft als functionaliteit om een les in te voeren

## Week 3

## Week 4

Na onze demonstratie bleek onze manier van data opslaan niet helemaal goed. We maaktte namelijk gebruik van TextIO ipv. ObjectIO. In deze week ben ik samen met Stijn begonnen om onze datastructuur om te zetten naar ObjectIO. 

Onze situatie was als volgt: We hebben nu een RosterInput die gebruik maakt van TextIO. Dit werkt in principe prima, alleen kan je hierdoor je ingevoerde waardes niet bewerken en verwijderen. Ook kan je zo dubbele objecten maken, wat niet optimaal is. Om dit te fixen, heb ik eerst onze eerste Rosterinput helemaal ge-reworked. In het eerste design was het namelijk onmogelijk om makkelijk veranderingen aan te passen. In het nieuwe model heb ik nu ook ListViews gezet, zodat de objecten die al bestaat duidelijk zijn weergegeven. (hoewel dit nog niet werkt atm.) 

*insert plaatje van oude model en nieuwe model

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
