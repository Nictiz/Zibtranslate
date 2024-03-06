# Contactgegevens
## File formats

The translation specs are available as: 
[CSV](../csv/Contactgegevens.csv) [JSON](../json/Contactgegevens.json) [XML](../xml/Contactgegevens.xml) [Excel](../excel/Contactgegevens.xlsx)



## Zib Contactgegevens

[Contactgegevens-v1.0(2017NL)](https://zibs.nl/wiki/Contactgegevens-v1.0(2017NL))

[Contactgegevens-v1.2(2020NL)](https://zibs.nl/wiki/Contactgegevens-v1.2(2020NL))









## Changes

| ConceptID_2017   | ConceptName_2017               | Change               | TypeChange         | Impact_heen   | TRANSLATIE_spec_heen                  | Impact_terug   | TRANSLATIE_spec_terug                                                                                             | Omschrijving                                                                                                                          |
|:-----------------|:-------------------------------|:---------------------|:-------------------|:--------------|:--------------------------------------|:---------------|:------------------------------------------------------------------------------------------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------|
| NL-CM:20.6.8     | EmailSoort                     | oranje: minor change | CARDINALITY CHANGE | Low           | ONE TO ZERO-TO-ONE                    | Medium         | ZERO-TO-ONE TO ONE                                                                                                | Kardinaliteit TelecomType aangepast van 1 naar 0..1.                                                                                  |
| NL-CM:20.6.8     | EmailSoort                     | oranje: minor change | VALUESET CHANGES   | Low           | valuesets 2017 -> valueset 2020 regel | Medium         | valuesets 2017 <- valueset 2020 regel                                                                             | Typo in engelse tekst in waarde binnen AdresTypeCodelijst aangepast. "Tempory address" moet zijn "Temporary address"                  |
| NL-CM:20.6.9     | **concept toegevoegd in 2020** | rood: major change   | CONCEPT ADDITION   | Low           |                                       | High           | IF [blank]source->target ELSE [toon en stuur de inhoud van dit data item als vrije tekst naar een 2017 ontvanger] | Aan een telefoonnummers is nu een toelichtingsveld toegevoegd, waarin nadere bijzonderheden over het nummer kunnen worden vastgelegd. |

## Mapping

| ConceptID_2017   | ConceptName_2017               | Codelists_2017       | Change                  | ConceptID_2020   | ConceptName_2020   | Codelists_2020       | Bits    | Omschrijving                                                                                                                          | TypeChange         | Impact_heen   | TRANSLATIE_spec_heen                  | Impact_terug   | TRANSLATIE_spec_terug                                                                                             |
|:-----------------|:-------------------------------|:---------------------|:------------------------|:-----------------|:-------------------|:---------------------|:--------|:--------------------------------------------------------------------------------------------------------------------------------------|:-------------------|:--------------|:--------------------------------------|:---------------|:------------------------------------------------------------------------------------------------------------------|
| NL-CM:20.6.1     | Contactgegevens                |                      | groen: geen wijzigingen | NL-CM:20.6.1     | Contactgegevens    |                      |         |                                                                                                                                       | NO CHANGE          |               |                                       |                |                                                                                                                   |
| NL-CM:20.6.2     | Telefoonnummers                |                      | groen: geen wijzigingen | NL-CM:20.6.2     | Telefoonnummers    |                      |         |                                                                                                                                       | NO CHANGE          |               |                                       |                |                                                                                                                   |
| NL-CM:20.6.3     | EmailAdressen                  |                      | groen: geen wijzigingen | NL-CM:20.6.3     | EmailAdressen      |                      |         |                                                                                                                                       | NO CHANGE          |               |                                       |                |                                                                                                                   |
| NL-CM:20.6.4     | Telefoonnummer                 |                      | groen: geen wijzigingen | NL-CM:20.6.4     | Telefoonnummer     |                      |         |                                                                                                                                       | NO CHANGE          |               |                                       |                |                                                                                                                   |
| NL-CM:20.6.5     | TelecomType                    | TelecomTypeCodelijst | groen: geen wijzigingen | NL-CM:20.6.5     | TelecomType        | TelecomTypeCodelijst |         |                                                                                                                                       | NO CHANGE          |               |                                       |                |                                                                                                                   |
| NL-CM:20.6.6     | NummerSoort                    | NummerSoortCodelijst | groen: geen wijzigingen | NL-CM:20.6.6     | NummerSoort        | NummerSoortCodelijst |         |                                                                                                                                       | NO CHANGE          |               |                                       |                |                                                                                                                   |
| NL-CM:20.6.7     | EmailAdres                     |                      | groen: geen wijzigingen | NL-CM:20.6.7     | EmailAdres         |                      |         |                                                                                                                                       | NO CHANGE          |               |                                       |                |                                                                                                                   |
| NL-CM:20.6.8     | EmailSoort                     | EmailSoortCodelijst  | oranje: minor change    | NL-CM:20.6.8     | EmailSoort         | EmailSoortCodelijst  | ZIB-958 | Kardinaliteit TelecomType aangepast van 1 naar 0..1.                                                                                  | CARDINALITY CHANGE | Low           | ONE TO ZERO-TO-ONE                    | Medium         | ZERO-TO-ONE TO ONE                                                                                                |
| NL-CM:20.6.8     | EmailSoort                     | EmailSoortCodelijst  | oranje: minor change    | NL-CM:20.6.8     | EmailSoort         | EmailSoortCodelijst  | ZIB-900 | Typo in engelse tekst in waarde binnen AdresTypeCodelijst aangepast. "Tempory address" moet zijn "Temporary address"                  | VALUESET CHANGES   | Low           | valuesets 2017 -> valueset 2020 regel | Medium         | valuesets 2017 <- valueset 2020 regel                                                                             |
| NL-CM:20.6.9     | **concept toegevoegd in 2020** |                      | rood: major change      | NL-CM:20.6.9     | Toelichting        |                      | ZIB-760 | Aan een telefoonnummers is nu een toelichtingsveld toegevoegd, waarin nadere bijzonderheden over het nummer kunnen worden vastgelegd. | CONCEPT ADDITION   | Low           |                                       | High           | IF [blank]source->target ELSE [toon en stuur de inhoud van dit data item als vrije tekst naar een 2017 ontvanger] |

