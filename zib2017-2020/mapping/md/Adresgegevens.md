# Adresgegevens
## File formats

The translation specs are available as: 
[CSV](../csv/Adresgegevens.csv) [JSON](../json/Adresgegevens.json) [XML](../xml/Adresgegevens.xml) [Excel](../excel/Adresgegevens.xlsx)



## Zib Adresgegevens

[Adresgegevens-v1.0(2017NL)](https://zibs.nl/wiki/Adresgegevens-v1.0(2017NL))

[Adresgegevens-v1.1(2020NL)](https://zibs.nl/wiki/Adresgegevens-v1.1(2020NL))









## Changes

| ConceptID_2017   | ConceptName_2017   | Change               | TypeChange         | Impact_heen   | TRANSLATIE_spec_heen   | Impact_terug   | TRANSLATIE_spec_terug   | Omschrijving                                                                                                         |
|:-----------------|:-------------------|:---------------------|:-------------------|:--------------|:-----------------------|:---------------|:------------------------|:---------------------------------------------------------------------------------------------------------------------|
| NL-CM:20.5.8     | AdresSoort         | oranje: minor change | CARDINALITY CHANGE | Low           | ONE TO ZERO-TO-ONE     | Medium         | ZERO-TO-ONE TO ONE      | kardinatliteit van 1 naar 0..1                                                                                       |
| NL-CM:20.5.8     | AdresSoort         | oranje: minor change | VALUESET CHANGES   | Low           |                        | Low            |                         | Typo in engelse tekst in waarde binnen AdresTypeCodelijst aangepast. "Tempory address" moet zijn "Temporary address" |

## Mapping

| ConceptID_2017   | ConceptName_2017      | Codelists_2017               | Change                  | ConceptID_2020   | ConceptName_2020      | Codelists_2020               | Bits    | Omschrijving                                                                                                         | TypeChange         | Impact_heen   | TRANSLATIE_spec_heen   | Impact_terug   | TRANSLATIE_spec_terug   |
|:-----------------|:----------------------|:-----------------------------|:------------------------|:-----------------|:----------------------|:-----------------------------|:--------|:---------------------------------------------------------------------------------------------------------------------|:-------------------|:--------------|:-----------------------|:---------------|:------------------------|
| NL-CM:20.5.1     | Adresgegevens         |                              | groen: geen wijzigingen | NL-CM:20.5.1     | Adresgegevens         |                              |         |                                                                                                                      | NO CHANGE          |               |                        |                |                         |
| NL-CM:20.5.2     | Straat                |                              | groen: geen wijzigingen | NL-CM:20.5.2     | Straat                |                              |         |                                                                                                                      | NO CHANGE          |               |                        |                |                         |
| NL-CM:20.5.3     | Woonplaats            |                              | groen: geen wijzigingen | NL-CM:20.5.3     | Woonplaats            |                              |         |                                                                                                                      | NO CHANGE          |               |                        |                |                         |
| NL-CM:20.5.4     | Gemeente              |                              | groen: geen wijzigingen | NL-CM:20.5.4     | Gemeente              |                              |         |                                                                                                                      | NO CHANGE          |               |                        |                |                         |
| NL-CM:20.5.5     | Land                  | LandGBACodelijst             | groen: geen wijzigingen | NL-CM:20.5.5     | Land                  | LandGBACodelijst             |         |                                                                                                                      | NO CHANGE          |               |                        |                |                         |
|                  |                       | LandISOCodelijst             |                         |                  |                       | LandISOCodelijst             |         |                                                                                                                      |                    |               |                        |                |                         |
| NL-CM:20.5.6     | Postcode              |                              | groen: geen wijzigingen | NL-CM:20.5.6     | Postcode              |                              |         |                                                                                                                      | NO CHANGE          |               |                        |                |                         |
| NL-CM:20.5.7     | AdditioneleInformatie |                              | groen: geen wijzigingen | NL-CM:20.5.7     | AdditioneleInformatie |                              |         |                                                                                                                      | NO CHANGE          |               |                        |                |                         |
| NL-CM:20.5.8     | AdresSoort            | AdresSoortCodelijst          | oranje: minor change    | NL-CM:20.5.8     | AdresSoort            | AdresSoortCodelijst          | ZIB-959 | kardinatliteit van 1 naar 0..1                                                                                       | CARDINALITY CHANGE | Low           | ONE TO ZERO-TO-ONE     | Medium         | ZERO-TO-ONE TO ONE      |
| NL-CM:20.5.8     | AdresSoort            | AdresSoortCodelijst          | oranje: minor change    | NL-CM:20.5.8     | AdresSoort            | AdresSoortCodelijst          | ZIB-900 | Typo in engelse tekst in waarde binnen AdresTypeCodelijst aangepast. "Tempory address" moet zijn "Temporary address" | VALUESET CHANGES   | Low           |                        | Low            |                         |
| NL-CM:20.5.9     | AanduidingBijNummer   |                              | groen: geen wijzigingen | NL-CM:20.5.9     | AanduidingBijNummer   |                              |         |                                                                                                                      | NO CHANGE          |               |                        |                |                         |
| NL-CM:20.5.10    | Huisnummertoevoeging  | AanduidingBijNummerCodelijst | groen: geen wijzigingen | NL-CM:20.5.10    | Huisnummertoevoeging  | AanduidingBijNummerCodelijst |         |                                                                                                                      | NO CHANGE          |               |                        |                |                         |
| NL-CM:20.5.11    | Huisnummerletter      |                              | groen: geen wijzigingen | NL-CM:20.5.11    | Huisnummerletter      |                              |         |                                                                                                                      | NO CHANGE          |               |                        |                |                         |
| NL-CM:20.5.12    | Huisnummer            |                              | groen: geen wijzigingen | NL-CM:20.5.12    | Huisnummer            |                              |         |                                                                                                                      | NO CHANGE          |               |                        |                |                         |

