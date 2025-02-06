```mermaid
erDiagram
    Winkels {
        int Winkel_ID PK
        string Winkelnaam
        string Adres
        string Postcode
        float Oppervlakte
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
        int Distributeur_ID FK
        date Besteldatum
        time Besteltijd
        date Leverdatum
        string Status
        string Tracking_Number
        string Leveringsstatus
        string Bezorgschema
    }

    Bestellingproducten {
        int Bestel_ID FK
        int Product_ID FK
        int Hoeveelheid
        float Totale_prijs
        int Aantal_geleverd
    }

    Gebruikers {
        int Gebruiker_ID PK
        string Naam
        string Email
        string Telefoonnummer
        string Wachtwoord
        string Rol
        date Datum_in_dienst
        int Winkel_ID FK
    }

    Klachten {
        int Klacht_ID PK
        int Winkel_ID FK
        int Opgelost_door FK
        string Categorie
        string Beschrijving
        date Datum
        time Tijd
        string Status
        date Oplossingsdatum
        string Oplossing_beschrijving
    }

    KPI_Types {
        int KPI_Type_ID PK
        string Naam
        string Eenheid
        string Beschrijving
    }

    KPI_Metingen {
        int Meting_ID PK
        int Winkel_ID FK
        int KPI_Type_ID FK
        float Waarde
        string Periode
    }

    Distributeurs {
        int Distributeur_ID PK
        string Naam
        string Adres
        string Telefoonnummer
        string Email
    }

    Meldingen {
        int Melding_ID PK
        string Beschrijving
        datetime Datum_tijd
        string Status
    }

    Rapporten {
        int Rapport_ID PK
        string Titel
        string Beschrijving
        date Datum
        string Type
        int Gerelateerd_ID FK
    }

    Winkels ||--o{ Voorraad : heeft
    Winkels ||--o{ Bestellingen : plaatst
    Winkels ||--o{ Klachten : ontvangt
    Winkels ||--o{ KPI_Metingen : heeft
    Winkels ||--o{ Gebruikers : beheert

    Gebruikers ||--o{ Klachten : lost_op
    Gebruikers ||--o{ Meldingen : ontvangt

    Producten ||--o{ Voorraad : omvat
    Producten ||--o{ Bestellingproducten : bevat

    Bestellingen ||--o{ Bestellingproducten : bevat
    Distributeurs ||--o{ Bestellingen : verwerkt

    KPI_Types ||--o{ KPI_Metingen : definieert

    Meldingen ||--o{ Rapporten : bevat
