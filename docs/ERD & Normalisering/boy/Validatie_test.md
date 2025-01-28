# Faker Data voor Database Validatie

## Winkels
| id | Naam        | Locatie     | Adres                |
|----|------------|------------|----------------------|
| 1  | SuperMart  | Amsterdam  | Damstraat 10        |
| 2  | FoodLand   | Rotterdam  | Coolsingel 20       |

## Producten
| id | Naam     | Streepjescode | Minimale hoeveelheid |
|----|---------|--------------|---------------------|
| 1  | Appel   | 8712345678901 | 10                  |
| 2  | Melk    | 8712345678902 | 5                   |

## Bestellingen
| id | winkel_id | Hoeveelheid | Leverdatum  |
|----|----------|------------|------------|
| 1  | 1        | 20         | 2025-02-01 |
| 2  | 2        | 15         | 2025-02-03 |

## Leveringen
| id | Distributeur_id | winkel_id | Aantal geleverd | Leverdatum  |
|----|----------------|-----------|----------------|------------|
| 1  | 1              | 1         | 50             | 2025-01-30 |
| 2  | 2              | 2         | 30             | 2025-01-31 |

## Klachten
| id | winkel_id | Klantnaam      | Categorie  | Beschrijving          |
|----|----------|---------------|------------|----------------------|
| 1  | 1        | Jan Jansen     | Product    | Beschadigde verpakking |
| 2  | 2        | Maria Verbeek  | Service    | Te late levering      |

## KPI's
| id | winkel_id | KPI             | Waarde | Periode     |
|----|----------|----------------|--------|------------|
| 1  | 1        | Omzet per maand | €5000  | Januari 2025 |
| 2  | 2        | Klanttevredenheid | 85%   | Januari 2025 |

## Personeel
| id | Naam        | Wachtwoord | winkel_id | Rol       |
|----|------------|------------|----------|----------|
| 1  | jdoe       | pass123    | 1        | Admin    |
| 2  | mjansen    | safePass   | 2        | Kassa |

## Distributeurs
| id | naam         | adres           | telefoonnummer | email               |
|----|-------------|-----------------|----------------|----------------------|
| 1  | FreshFruits | Havenstraat 1   | 0612345678     | contact@fresh.nl    |
| 2  | DairyBest   | Melkweg 5       | 0623456789     | info@dairybest.nl   |

## Meldingen
| id | Beschrijving      | Datum en tijd     | Afgehandeld |
|----|------------------|------------------|------------|
| 1  | Voorraad bijna op | 2025-01-29 14:00 | Ja         |
| 2  | Nieuwe klacht    | 2025-01-30 09:30 | Nee        |

## Rapporten
| id | Titel         | Beschrijving               | Datum      | Type | Gerelateerd_id |
|----|-------------|---------------------------|-----------|------|---------------|
| 1  | Verkooprapport | Analyse van januari sales | 2025-02-01 | KPI  | 1             |
| 2  | Klachtenrapport | Overzicht van klachten  | 2025-02-02 | Klachten | 2       |

## Bestellingproducten
| bestellingen_id | Product_id | Hoeveelheid |
|----------------|------------|------------|
| 1              | 1          | 5          |
| 2              | 2          | 10         |

## Leveringproducten
| leveringen_id | product_id | aantal geleverd |
|--------------|-----------|----------------|
| 1            | 1         | 25             |
| 2            | 2         | 20             |

## DistributeurProducten
| Distributeur_id | product_id |
|----------------|-----------|
| 1              | 1         |
| 2              | 2         |

## Personeels_planning
| personeel_id | datum      | tijdslot |
|-------------|-----------|---------|
| 1           | 2025-02-01 | 09:00-17:00 |
| 2           | 2025-02-02 | 10:00-18:00 |

## DistributeurBestelling
| distributeur_id | bestelling_id |
|----------------|--------------|
| 1              | 1            |
| 2              | 2            |