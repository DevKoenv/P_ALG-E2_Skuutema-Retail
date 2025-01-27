```mermaid
erDiagram
    Winkels {
        int Winkel_ID PK
        string Winkelnaam
        string Locatie
        string Adres
        string Postcode
        string Regio
    }

    Producten {
        int Product_ID PK
        string Productnaam
        string Productcode
        string Categorie
        int Minimale_voorraad
        int Maximale_voorraad
        float Prijs_per_eenheid
        string Barcode
    }

    Voorraad {
        int Voorraad_ID PK
        int Winkel_ID FK
        int Product_ID FK
        int Huidige_voorraad
    }

    Bestellingen {
        int Bestel_ID PK
        int Winkel_ID FK
        date Datum
        time Tijd
        string Status
        date Leverdatum
        string Bezorgschema
    }

    Bestellingproducten {
        int Bestel_ID FK
        int Product_ID FK
        int Hoeveelheid
        float Totale_prijs
    }

    Gebruikers {
        int Gebruiker_ID PK
        string Gebruikersnaam
        string Naam
        string Email
        string Telefoonnummer
        string Wachtwoord
        string Rol
        int Winkel_ID FK
    }

    Klachten {
        int Klacht_ID PK
        int Winkel_ID FK
        string Categorie
        string Beschrijving
        date Datum
        time Tijd
        string Status
        date Oplossingsdatum
    }

    KPI {
        int KPI_ID PK
        int Winkel_ID FK
        string KPI
        string Waarde
        string Periode
    }

    Winkels ||--o{ Voorraad : heeft
    Producten ||--o{ Voorraad : omvat
    Voorraad ||--o{ Bestellingproducten : bevat
    Bestellingen ||--o{ Bestellingproducten : bevat
    Gebruikers ||--o{ Winkels : beheert
    Winkels ||--o{ Klachten : ontvangt
    Winkels ||--o{ KPI : heeft
