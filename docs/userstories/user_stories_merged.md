## User stories

### Summary

**Als winkelbeheerder** wil ik in real-time waarschuwingen ontvangen over lage voorraadniveaus, zodat ik snel producten kan bijbestellen.

**Als winkelbeheerder** wil ik een zoekfunctie hebben om snel producten te vinden en hun voorraadstatus te bekijken, zodat ik efficiënter kan werken.

**Als klantenservicemedewerker** wil ik een formulier op de website kunnen invullen voor veelvoorkomende klachten, zodat klachten systematisch geregistreerd worden.

**Als manager** wil ik dashboards zien met KPI’s zoals omzet per vierkante meter en voorraadnauwkeurigheid, zodat ik beter kan sturen op prestaties.

**Als manager** wil ik dat het systeem meldingen verstuurt wanneer bestellingen later geleverd worden dan gepland, zodat klanten hiervan tijdig op de hoogte zijn.

**Als manager** wil ik een tegelweergave zien van alle winkels met statussen zoals omzet en trends, zodat ik in één oogopslag de prestaties kan beoordelen.

**Als IT-beheerder** wil ik ervoor zorgen dat klantengegevens voldoen aan de AVG-normen, zodat de organisatie geen juridische risico's loopt.

**Als klant** wil ik winkelinformatie kunnen opzoeken, zodat ik gemakkelijk een winkel in mijn buurt kan vinden.

**Als projectgroep** wil ik dagelijks een stand-up houden, zodat we elkaars voortgang kunnen bespreken en problemen tijdig signaleren.

---

### User story 1: Gebruikersauthenticatie en Autorisatie

**Als een** winkelbeheerder  
**wil ik** kunnen inloggen op het platform  
**zodat** ik toegang heb tot mijn winkelgegevens.

#### Acceptatiecriteria:

1. Gebruikers kunnen inloggen met een gebruikersnaam en wachtwoord.
2. Toegang wordt beperkt op basis van rollen.

**Als een** klantenservicemedewerker  
**wil ik** alleen toegang hebben tot functies die relevant zijn voor mijn rol  
**zodat** ik efficiënt kan werken.

#### Acceptatiecriteria:

1. Autorisatieschema's beperken de toegang tot specifieke functies.

---

### User story 2: Voorraadbeheer

**Als een** winkelbeheerder  
**wil ik** real-time voorraadniveaus kunnen bekijken  
**zodat** ik inzicht heb in welke producten bijna op zijn.

#### Acceptatiecriteria:

1. Een overzicht van actuele voorraadniveaus wordt weergegeven.

**Als een** winkelbeheerder  
**wil ik** een product kunnen scannen om direct de voorraad te zien  
**zodat** ik efficiënter kan werken.

#### Acceptatiecriteria:

1. Het scannen van een product toont direct de beschikbare voorraad.

**Als een** winkelbeheerder  
**wil ik** eenvoudig bestellingen kunnen plaatsen voor producten die bijna op zijn  
**zodat** de winkel altijd goed bevoorraad is.

#### Acceptatiecriteria:

1. Een bestelknop toont een eenvoudig formulier om de benodigde hoeveelheid aan te geven.

**Als een** winkelbeheerder  
**wil ik** in real-time waarschuwingen ontvangen wanneer de voorraad van een product onder een bepaald niveau komt  
**zodat** ik op tijd nieuwe bestellingen kan plaatsen.

#### Acceptatiecriteria:

1. Wanneer een product onder de minimale voorraad (20 stuks) komt, ontvang ik een melding.
2. De melding bevat het product, de huidige voorraad, en de aanbevolen bestelhoeveelheid.
3. De meldingen zijn zichtbaar op mijn dashboard en worden verzonden via pushnotificaties.

**Als een** winkelbeheerder  
**wil ik** producten snel kunnen opzoeken in het systeem  
**zodat** ik direct de voorraadstatus kan zien.

#### Acceptatiecriteria:

1. De zoekfunctie ondersteunt het zoeken op productnaam en barcode.
2. De resultaten bevatten het huidige voorraadniveau, locatie in de winkel, en aanbevolen bestelstatus.
3. Het systeem laat producten met lage voorraad bovenaan de resultaten zien.

---

### User story 3: Dashboards en Analyse

**Als een** lid van het executief management  
**wil ik** toegang hebben tot dashboards met samenvattende gegevens over verkoop en winstgevendheid  
**zodat** ik strategische beslissingen kan nemen.

#### Acceptatiecriteria:

1. Het dashboard toont KPI's zoals omzet, winst en voorraadniveaus in grafieken en tabellen.

**Als een** winkelbeheerder  
**wil ik** inzicht hebben in personeelsplanning via een dashboard  
**zodat** ik mijn team effectief kan aansturen.

#### Acceptatiecriteria:

1. Het dashboard toont een kalenderweergave met geplande diensten.

**Als een** manager  
**wil ik** dashboards zien met KPI’s zoals omzet per vierkante meter en voorraadnauwkeurigheid  
**zodat** ik beter kan sturen op prestaties.

#### Acceptatiecriteria:

1. Het dashboard toont KPI’s zoals omzet per vierkante meter, voorraadnauwkeurigheid en winkeldiefstalpercentage.
2. Data in het dashboard wordt minimaal elke dag geüpdatet.
3. KPI’s worden visueel weergegeven via grafieken en tabellen.

**Als een** manager  
**wil ik** een tegelweergave zien van alle winkels met statussen zoals voorraad en omzet  
**zodat** ik in één oogopslag de prestaties kan beoordelen.

#### Acceptatiecriteria:

1. Iedere tegel toont de winkelnaam, voorraadstatus, en omzettrend (groen pijltje omhoog, rood pijltje omlaag).
2. Bij klikken op een tegel verschijnt een gedetailleerd overzicht met grafieken en statistieken.
3. De tegelweergave is filterbaar op regio of stad.

---

### User story 4: Klantenservice

**Als een** klantenservicemedewerker  
**wil ik** klachten en vragen kunnen registreren  
**zodat** ik deze efficiënt kan afhandelen.

#### Acceptatiecriteria:

1. Een formulier voor klachtregistratie met invoervelden voor klantnaam, klachtomschrijving en status.

**Als een** klantenservicemedewerker  
**wil ik** productinformatie snel kunnen opzoeken  
**zodat** ik klanten snel kan helpen.

#### Acceptatiecriteria:

1. Een zoekfunctie toont direct de relevante productinformatie.

**Als een** klantenservicemedewerker  
**wil ik** een formulier op de website kunnen invullen voor veelvoorkomende klachten  
**zodat** klachten systematisch geregistreerd worden.

#### Acceptatiecriteria:

1. Het formulier bevat presets zoals “aangebroken materiaal”, “cola zonder koolzuur”, en een optie “Anders”.
2. Ingevoerde klachten worden automatisch opgeslagen in het systeem.
3. Klantgegevens worden niet opgeslagen bij het invullen van een klacht.

---

### User story 5: Bestelproces

**Als een** winkelbeheerder  
**wil ik** dagelijks mijn bestellijsten automatisch kunnen versturen  
**zodat** de distributie soepel verloopt.

#### Acceptatiecriteria:

1. Bestellijsten worden om 12:00 en 18:00 automatisch naar de distributeur verzonden.

**Als een** distributeur  
**wil ik** de levertijd kunnen garanderen  
**zodat** winkels tijdig hun producten ontvangen.

#### Acceptatiecriteria:

1. Bestellingen vóór 12:00 worden de volgende dag voor 10:00 geleverd.

**Als een** manager  
**wil ik** meldingen ontvangen wanneer een bestelling niet op tijd geleverd wordt  
**zodat** ik klanten op de hoogte kan stellen van de vertraging.

#### Acceptatiecriteria:

1. Het systeem verstuurt automatisch een melding wanneer een bestelling te laat is.
2. De melding bevat de verwachte levertijd en de reden van de vertraging.
3. De melding wordt doorgestuurd naar de betrokken winkel.

---

### User story 6: Privacy en Beveiliging

**Als een** IT-beheerder  
**wil ik** ervoor zorgen dat klantengegevens voldoen aan de AVG-normen  
**zodat** de organisatie geen juridische risico's loopt.

#### Acceptatiecriteria:

1. Gegevens worden versleuteld opgeslagen.
2. Toegang is alleen mogelijk voor geautoriseerde gebruikers.

---

### User story 7: Winkellocaties

**Als een** klant  
**wil ik** winkelinformatie kunnen opzoeken  
**zodat** ik gemakkelijk een winkel in mijn buurt kan vinden.

#### Acceptatiecriteria:

1. Een kaart of lijst toont alle filialen met locatie, adres en contactinformatie.

---

### User story 8: Wireframes en Technische Ontwerpen

**Als een** ontwikkelaar  
**wil ik** duidelijke wireframes hebben  
**zodat** ik de functionaliteit en flow van de applicatie kan begrijpen.

#### Acceptatiecriteria:

1. Alle wireframes bevatten labels bij invoervelden en navigatiepaden tussen schermen.

**Als een** projectgroep  
**wil ik** een genormaliseerd ERD hebben  
**zodat** de database efficiënt kan worden opgezet.

#### Acceptatiecriteria:

1. Een ERD toont alle entiteiten, attributen en relaties, genormaliseerd tot minstens de 3e normaalvorm.

---

### User story 9: Samenwerking en Planning

**Als een** projectgroep  
**wil ik** dagelijks een stand-up houden  
**zodat** we elkaars voortgang kunnen bespreken en problemen tijdig signaleren.

#### Acceptatiecriteria:

1. De stand-up omvat een overzicht van wat er is gedaan, wat gepland is en waar hulp nodig is.

**Als een** groep  
**wil ik** een sprint retrospective houden  
**zodat** we kunnen leren van het proces en verbeteringen kunnen doorvoeren.

#### Acceptatiecriteria:

1. Feedback wordt genoteerd en verwerkt in actiepunten voor toekomstige projecten.

