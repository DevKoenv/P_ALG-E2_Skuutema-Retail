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

    Leveringen {
        int Levering_ID PK
        int Distributeur_ID FK
        int Winkel_ID FK
        date Leverdatum
        string Tracking_Number
        string Leveringsstatus
    }

    Leveringproducten {
        int Levering_ID FK
        int Product_ID FK
        int Aantal_geleverd
    }

    Distributeurs {
        int Distributeur_ID PK
        string Naam
        string Adres
        string Telefoonnummer
        string Email
    }

    DistributeurBestellingen {
        int Distributeur_ID FK
        int Bestel_ID FK
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

    Personeels_planning {
        int Gebruiker_ID FK
        date Datum
        string Tijdslot
        string Shift_Type
        boolean Is_Holiday
    }

    Winkels ||--o{ Voorraad : heeft
    Winkels ||--o{ Bestellingen : plaatst
    Winkels ||--o{ Klachten : ontvangt
    Winkels ||--o{ KPI_Metingen : heeft
    Winkels ||--o{ Gebruikers : beheert
    Winkels ||--o{ Leveringen : ontvangt

    Gebruikers ||--o{ Klachten : lost_op
    Gebruikers ||--o{ Meldingen : ontvangt
    Gebruikers ||--o{ Personeels_planning : heeft

    Producten ||--o{ Voorraad : omvat
    Producten ||--o{ Bestellingproducten : bevat
    Producten ||--o{ Leveringproducten : bevat

    Bestellingen ||--o{ Bestellingproducten : bevat
    Leveringen ||--o{ Leveringproducten : bevat
    Leveringen ||--o{ Distributeurs : verwerkt
    Bestellingen ||--o{ DistributeurBestellingen : verwerkt

    KPI_Types ||--o{ KPI_Metingen : definieert

    Meldingen ||--o{ Rapporten : bevat
