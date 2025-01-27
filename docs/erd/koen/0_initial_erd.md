# 0NF : Ongeorganiseerde data

##  **Winkellocaties**
- Winkelnaam
- Locatie (stad)
- Adres (straat, huisnummer, postcode)
- Regio

---

##  **Producten**
- Productnaam
- Productcode
- Categorie (groente, zuivel, dranken, etc.)
- Minimale voorraad
- Maximale voorraad
- Huidige voorraad
- Prijs per eenheid
- Barcode

---

##  **Bestellingen**
- Bestelnummer
- Datum en tijd van bestelling
- Winkel
- Producten in de bestelling
- Hoeveelheid van elk product
- Totale bestelbedrag
- Status (bijvoorbeeld: in behandeling, verzonden, geleverd)
- Leverdatum

---

##  **Gebruikers**
- Gebruikersnaam
- Rol (bijvoorbeeld: winkelbeheerder, klantenservice, management)
- Naam
- E-mailadres
- Telefoonnummer
- Wachtwoord (versleuteld)
- Toegewezen winkel (indien van toepassing)

---

##  **Klachten**
- Klachtnummer (uniek ID)
- Klantnaam (optioneel)
- Winkel
- Categorie (bijvoorbeeld: product, service)
- Product gerelateerd aan de klacht (optioneel)
- Beschrijving van de klacht
- Datum en tijd van klacht
- Oplossingsstatus (bijvoorbeeld: open, opgelost, in behandeling)
- Oplossingsdatum

---

##  **KPI’s en Managementdata**
- Omzet per winkel
- Omzet per vierkante meter
- Winstmarge per product/winkel
- Voorraadnauwkeurigheid
- Winkeldiefstalpercentage
- Producten met lage voorraad (lijst)
- Topomzet-producten
- Groene/rrode trendpijlen (omzet stijging/daling)

---

##  **Voorraadbeheer**
- Producten per winkel
- Huidige voorraad per product
- Magazijnvoorraad per winkel
- Aantal te bestellen producten
- Historie van voorraadbewegingen (bijv. ontvangen, verkocht, retour)

---

##  **Distributie**
- Distributeurnaam
- Distributeuradres
- Bestellingen gekoppeld aan distributeur
- Bezorgschema’s (bijvoorbeeld: voor 12:00 besteld, volgende dag geleverd)
- Contactinformatie distributeur

---

##  **Klantenservicefunctionaliteiten**
- Veelgestelde vragen (FAQ)
- Beschikbare antwoorden/templates
- Soorten klachten (bijvoorbeeld: beschadigd product, ontbrekend item, verlopen product)
- Formulierinhoud (velden zoals klantnaam, klachtomschrijving, categorie, etc.)

---

##  **Dashboardfunctionaliteiten**
- Filteropties (bijv. per winkel, productcategorie)
- Overzichten van winkels (bijvoorbeeld: tegelweergave)
- Grafieken en tabellen met KPI’s
- Meldingen over lage voorraad, te late leveringen, enz.
- Historische gegevens en trends

---

##  **Privacy en Beveiliging**
- AVG-conforme opslag van klantengegevens
- Versleuteling van gevoelige data
- Gebruikersactiviteit-logs (wie heeft wat gedaan)
- Toegangscontrole (op basis van rol)

---

##  **Overige data**
- Tijdstempels (voor alle acties, zoals meldingen, bestellingen, voorraadupdates)
- Zoektermen gebruikt in de zoekfunctie
- Statistieken over gebruik (bijv. hoe vaak een melding wordt bekeken, aantal ingediende klachten)
