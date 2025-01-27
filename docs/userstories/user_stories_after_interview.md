## User stories

### Summary

**Als winkelbeheerder** wil ik in real-time waarschuwingen ontvangen over lage voorraadniveaus, zodat ik snel producten kan bijbestellen.

**Als winkelbeheerder** wil ik een zoekfunctie hebben om snel producten te vinden en hun voorraadstatus te bekijken, zodat ik efficiënter kan werken.

**Als klantenservicemedewerker** wil ik een formulier op de website kunnen invullen voor veelvoorkomende klachten, zodat klachten systematisch geregistreerd worden.

**Als manager** wil ik dashboards zien met KPI’s zoals omzet per vierkante meter en voorraadnauwkeurigheid, zodat ik beter kan sturen op prestaties.

**Als manager** wil ik dat het systeem meldingen verstuurt wanneer bestellingen later geleverd worden dan gepland, zodat klanten hiervan tijdig op de hoogte zijn.

**Als manager** wil ik een tegelweergave zien van alle winkels met statussen zoals omzet en trends, zodat ik in één oogopslag de prestaties kan beoordelen.

---

### User story 1: Real-time voorraadwaarschuwingen

**Als een** winkelbeheerder  
**wil ik** real-time waarschuwingen ontvangen wanneer de voorraad van een product onder een bepaald niveau komt  
**zodat** ik op tijd nieuwe bestellingen kan plaatsen.

#### Acceptance Criteria:

1. Wanneer een product onder de minimale voorraad (20 stuks) komt, ontvang ik een melding.
2. De melding bevat het product, de huidige voorraad, en de aanbevolen bestelhoeveelheid.
3. De meldingen zijn zichtbaar op mijn dashboard en worden verzonden via pushnotificaties.

---

### User story 2: Zoekfunctie voorraad

**Als een** winkelbeheerder  
**wil ik** producten snel kunnen opzoeken in het systeem  
**zodat** ik direct de voorraadstatus kan zien.

#### Acceptance Criteria:

1. De zoekfunctie ondersteunt het zoeken op productnaam en barcode.
2. De resultaten bevatten het huidige voorraadniveau, locatie in de winkel, en aanbevolen bestelstatus.
3. Het systeem laat producten met lage voorraad bovenaan de resultaten zien.

---

### User story 3: Klachtenformulier

**Als een** klantenservicemedewerker  
**wil ik** een formulier op de website kunnen invullen voor veelvoorkomende klachten  
**zodat** klachten systematisch geregistreerd worden.

#### Acceptance Criteria:

1. Het formulier bevat presets zoals “aangebroken materiaal”, “cola zonder koolzuur”, en een optie “Anders”.
2. Ingevoerde klachten worden automatisch opgeslagen in het systeem.
3. Klantgegevens worden niet opgeslagen bij het invullen van een klacht.

---

### User story 4: Managementdashboards

**Als een** manager  
**wil ik** toegang hebben tot dashboards met KPI’s zoals omzet per vierkante meter en voorraadnauwkeurigheid  
**zodat** ik inzicht krijg in de prestaties van de winkels.

#### Acceptance Criteria:

1. Het dashboard toont KPI’s zoals omzet per vierkante meter, voorraadnauwkeurigheid en winkeldiefstalpercentage.
2. Data in het dashboard wordt minimaal elke dag geüpdatet.
3. KPI’s worden visueel weergegeven via grafieken en tabellen.

---

### User story 5: Meldingen over late bestellingen

**Als een** manager  
**wil ik** meldingen ontvangen wanneer een bestelling niet op tijd geleverd wordt  
**zodat** ik klanten op de hoogte kan stellen van de vertraging.

#### Acceptance Criteria:

1. Het systeem verstuurt automatisch een melding wanneer een bestelling te laat is.
2. De melding bevat de verwachte levertijd en de reden van de vertraging.
3. De melding wordt doorgestuurd naar de betrokken winkel.

---

### User story 6: Tegelweergave winkels

**Als een** manager  
**wil ik** een tegelweergave zien van alle winkels met statussen zoals voorraad en omzet  
**zodat** ik in één oogopslag de prestaties kan beoordelen.

#### Acceptance Criteria:

1. Iedere tegel toont de winkelnaam, voorraadstatus, en omzettrend (groen pijltje omhoog, rood pijltje omlaag).
2. Bij klikken op een tegel verschijnt een gedetailleerd overzicht met grafieken en statistieken.
3. De tegelweergave is filterbaar op regio of stad.
