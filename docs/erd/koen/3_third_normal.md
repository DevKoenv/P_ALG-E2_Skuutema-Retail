# 3NF: Derde Normaalvorm

## **Winkellocaties**

| **Winkel_ID** | **Winkelnaam**               | **Locatie**   | **Adres**                 | **Postcode** |
|---------------|------------------------------|---------------|---------------------------|---------------|
| 1             | Skuutema Retail Hoofdkantoor | Amsterdam     | Keizersgracht 123         | 1015 CJ       |

---

## **Producten**

| **Product_ID** | **Productnaam** | **Productcode** | **Categorie** | **Minimale voorraad** | **Maximale voorraad** | **Prijs per eenheid** | **Barcode**       |
|----------------|-----------------|-----------------|---------------|-----------------------|-----------------------|-----------------------|-------------------|
| 1              | Appel           | 1001            | Groente       | 20                    | 100                   | €0.50                 | 8711234567890     |

---

## **Voorraad**

| **Voorraad_ID** | **Winkel_ID** | **Product_ID** | **Huidige voorraad** |
|------------------|---------------|----------------|-----------------------|
| 1               | 1             | 1              | 15                    |

---

## **Bestellingen**

**Hoofdbestellingen:**
| **Bestel_ID** | **Winkel_ID** | **Datum**   | **Tijd** | **Status**       | **Leverdatum** |
|---------------|---------------|-------------|----------|------------------|----------------|
| 1             | 1             | 2025-01-27  | 12:00    | In behandeling   | 2025-01-28     |

**Bestellingproducten**
| **Bestel_ID** | **Product_ID** | **Hoeveelheid** | **Totale prijs** |
|---------------|----------------|-----------------|------------------|
| 1             | 1              | 10              | €5.00            |

---

## **Gebruikers**

| **Gebruiker_ID** | **Gebruikersnaam** | **Naam**      | **E-mailadres**       | **Telefoonnummer** | **Wachtwoord**     | **Rol**          | **Winkel_ID** |
|-------------------|--------------------|---------------|-----------------------|--------------------|--------------------|------------------|---------------|
| 1                | jansmit           | Jan Smit      | jan.smit@example.com  | 0612345678         | HASHED_PASSWORD    | Winkelbeheerder  | 1             |

---

## **Klachten**

**Klachten:**
| **Klacht_ID** | **Winkel_ID** | **Categorie** | **Beschrijving**        | **Datum**   | **Tijd** | **Status**    | **Oplossingsdatum** | **Opgelost_door** | **Oplossing_beschrijving** |
|---------------|---------------|---------------|-------------------------|-------------|----------|---------------|---------------------|-------------------|----------------------------|
| 1             | 1             | Product       | Beschadigde verpakking  | 2025-01-26  | 15:00    | Opgelost      | 2025-01-27          | 1                 | Product vervangen          |

**Klachtproducten**
| **Klacht_ID** | **Product_ID** |
|---------------|----------------|
| 1             | 1              |

---

## **KPI Definities**

| **KPI_Type_ID** | **Naam**                    | **Eenheid** | **Beschrijving**                    |
|-----------------|----------------------------|-------------|-------------------------------------|
| 1               | Omzet per vierkante meter  | EUR/m²      | Totale omzet gedeeld door opp      |
| 2               | Voorraadnauwkeurigheid     | %           | Percentage correcte voorraadtelling |
| 3               | Winstmarge                 | %           | Percentage winst op verkoop         |

## **KPI Metingen**

| **Meting_ID** | **Winkel_ID** | **KPI_Type_ID** | **Waarde** | **Periode**    |
|---------------|---------------|-----------------|------------|----------------|
| 1             | 1             | 1               | 500        | Januari 2025   |
| 2             | 1             | 2               | 98.5       | Januari 2025   |
