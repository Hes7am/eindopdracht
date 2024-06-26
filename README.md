# Eindopdracht - inloggen met PHP en MySQL 
Template voor eindopdracht level 4
# Opdracht:
Maak een Inlogsysteem met PHP en MySQL
# Beschrijving:
Het doel van deze opdracht is om een eenvoudig inlogsysteem te bouwen met behulp van PHP en MySQL. Het inlogsysteem moet gebruikersregistratie, inlogfunctionaliteit en een beveiligde pagina bieden waar alleen ingelogde gebruikers toegang toe hebben. 

Gebruik de uitnodigingslink van GitHub classroom om je aan te melden voor de persoonlijke repository van dit project. 

Clone deze repository naar je eigen systeem om met de bestanden in dit project de opdracht af te maken. De repository bestaat uit de volgende onderdelen:

- edit.php
- index.php
- login.php
- logout.php
- register.php
- css/style.css
- classes/database.php
- README.md
- login_pvb_2024.sql

Het laatste SQL-bestand gebruik je als database voor je inlogsysteem. Deze database bestaat uit een enkele tabel (user) met een username, password, postcode, huisnummer en woonplaats kolom.

# Functionele vereisten:

## Registratiepagina:
- Een gebruiker moet zich kunnen registreren door een gebruikersnaam en wachtwoord in te voeren 
- Zorg bij registreren voor een controle op het wachtwoord door deze 2 x in te voeren, deze beide **hetzelfde** moeten zijn. Laat deze controle plaats vinden in de front- en backend.
- De gebruikersnaam moet **uniek** zijn in de database.
- Het wachtwoord moet worden **gehasht** voordat het in de database wordt opgeslagen.
## Inlogpagina:
- Een geregistreerde gebruiker moet kunnen inloggen met zijn/haar gebruikersnaam en wachtwoord.
- Onjuiste inloggegevens moeten een foutmelding geven en de gebruiker moet op de inlogpagina blijven.
## Uitlog pagina:
- Een ingelogde gebruiker moet kunnen uitloggen.
- Verplaats de gebruiker naar de inlogpagina nadat het uitloggen heeft plaatsgevonden.
## Beveiligde pagina's:
- Nadat een gebruiker is ingelogd, moeten bepaalde pagina's alleen toegankelijk zijn voor ingelogde gebruikers.
- Als een niet-ingelogde gebruiker probeert toegang te krijgen tot een beveiligde pagina, moet hij/zij worden omgeleid naar de inlogpagina.
  - Beveiligde pagina zijn: index.php en edit.php
## Inhoud van de beveiligde pagina's:
- De index.php pagina toont een lijst van alle gebruikers uit de database in een tabel, deze gebruikers moeten worden opgehaald uit de database.
- Zodra een gebruiker op een gebruiker klikt (met het _edit_ icon), wordt de edit.php pagina geopend.
- De edit.php pagina toont een formulier met de geselecteerde gebruiker waarvan de postcode, huisnummer en woonplaats kan worden aangepast. 
- Nadat de gegevens zijn aangepast, moet de gebruiker op de _submit_ knop drukken om de gegevens op te slaan in de database en daarna weer terug keren naar de index.php pagina.
## Technische vereisten:
- Gebruik PHP om de backend-functionaliteit te implementeren.
- Gebruik Javascript om de frontend-functionaliteit te implementeren.
- Maak gebruik van MySQL om de gebruikersgegevens op te slaan.
- - Het is alleen toegestaan om gebruik te maken van de object georiënteerde interface API: MySQLi of PDO om je database te raadplegen
- - Gebruik prepared statements om SQL-injectie te voorkomen.
- Maak gebruik van HTML, CSS en eventueel JavaScript voor de frontend.
- Maak gebruik sessies om de ingelogde status van een gebruiker bij te houden.
- Benader de database met een aparte klasse (class: database.php).
- Gebruik een ander account dan **root** om de database te benaderen.
# Inleveren:
- Ben je klaar? **Commit** en **Push** het resultaat voor deze opdracht naar de Github classroom repository zoals boven de opdracht is beschreven. 
# Beoordeling:
- De opdracht wordt beoordeeld op basis van de functionele en technische vereisten zoals in de rubric is beschreven.
