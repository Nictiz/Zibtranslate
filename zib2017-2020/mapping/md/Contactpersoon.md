# Contactpersoon
## File formats

The translation specs are available as: 
[CSV](../csv/Contactpersoon.csv) [JSON](../json/Contactpersoon.json) [XML](../xml/Contactpersoon.xml)



[Contactpersoon-v3.1(2017NL)](https://zibs.nl/wiki/Contactpersoon-v3.1(2017NL))

[Contactpersoon-v3.4(2020NL)](https://zibs.nl/wiki/Contactpersoon-v3.4(2020NL))







## Zib-level changes

| ConceptID_2017   | ConceptName_2017   | Change                | TypeChange          | Omschrijving                      |
|:-----------------|:-------------------|:----------------------|:--------------------|:----------------------------------|
| DCM::Purpose     | Purpose            | geel: patch wijziging | SIMPLE PATCH CHANGE | Purpose Tekst definitie aangepast |

## Changes

| ConceptID_2017   | ConceptName_2017   | Change               | TypeChange                         | Impact_heen   | TRANSLATIE_spec_heen                                              | Impact_terug   | TRANSLATIE_spec_terug                                            | Omschrijving                                                                                                                                 |
|:-----------------|:-------------------|:---------------------|:-----------------------------------|:--------------|:------------------------------------------------------------------|:---------------|:-----------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------------|
| NL-CM:3.1.1      | Contactpersoon     | oranje: minor change | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefintionCode  [blank] -> [70862002 contactpersoon (persoon)] | Medium         | SCT DefintionCode [70862002 contactpersoon (persoon)] -> [blank] | SNOMED CT DefintionCode concept aangepast                                                                                                    |
| NL-CM:3.1.2      | Rol                | oranje: minor change | VALUESET CHANGES                   | Low           | valuesets 2017 -> valueset 2020 regel                             | Medium         | valuesets 2017 <- valueset 2020 regel                            | Diverse toevoegingen aan codelijst en erratum waarbij de codes onder de 10 een leading zero hebben gekregen zoals bij dit codesysteem hoort. |
| NL-CM:3.1.5      | Adresgegevens      | rood: major change   | CARDINALITY CHANGE                 | Low           | ZERO-TO-ONE TO ZERO-TO-MANY                                       | High           | ZERO-TO-MANY TO  ZERO-TO-ONE                                     | Cardinaliteit adresgegevens in de zib Contactpersoon verruimt van 0..1 naar 0..*                                                             |

## Mapping

| ZibName        | ConceptID_2017   | ConceptName_2017   | Codelists_2017   | Change                  | ConceptID_2020   | ConceptName_2020   | Codelists_2020   | Bits                                    | Omschrijving                                                                                                                                 | TypeChange                         | Impact_heen   | TRANSLATIE_spec_heen                                              | Impact_terug   | TRANSLATIE_spec_terug                                            |
|:---------------|:-----------------|:-------------------|:-----------------|:------------------------|:-----------------|:-------------------|:-----------------|:----------------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------------|:-----------------------------------|:--------------|:------------------------------------------------------------------|:---------------|:-----------------------------------------------------------------|
| Contactpersoon | NL-CM:3.1.1      | Contactpersoon     |                  | oranje: minor change    | NL-CM:3.1.1      | Contactpersoon     |                  | ZIB-1189                                | SNOMED CT DefintionCode concept aangepast                                                                                                    | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefintionCode  [blank] -> [70862002 contactpersoon (persoon)] | Medium         | SCT DefintionCode [70862002 contactpersoon (persoon)] -> [blank] |
| Contactpersoon | NL-CM:3.1.2      | Rol                | RolCodelijst     | oranje: minor change    | NL-CM:3.1.2      | Rol                | RolCodelijst     | ZIB-698 ; ZIB-1094 ; ZIB-629 ; ZIB-1378 | Diverse toevoegingen aan codelijst en erratum waarbij de codes onder de 10 een leading zero hebben gekregen zoals bij dit codesysteem hoort. | VALUESET CHANGES                   | Low           | valuesets 2017 -> valueset 2020 regel                             | Medium         | valuesets 2017 <- valueset 2020 regel                            |
| Contactpersoon | NL-CM:3.1.3      | Relatie            | RelatieCodelijst | groen: geen wijzigingen | NL-CM:3.1.3      | Relatie            | RelatieCodelijst |                                         |                                                                                                                                              |                                    |               |                                                                   |                |                                                                  |
| Contactpersoon | NL-CM:3.1.4      | Naamgegevens       |                  | groen: geen wijzigingen | NL-CM:3.1.4      | Naamgegevens       |                  |                                         |                                                                                                                                              |                                    |               |                                                                   |                |                                                                  |
| Contactpersoon | NL-CM:3.1.5      | Adresgegevens      |                  | rood: major change      | NL-CM:3.1.5      | Adresgegevens      |                  | ZIB-960                                 | Cardinaliteit adresgegevens in de zib Contactpersoon verruimt van 0..1 naar 0..*                                                             | CARDINALITY CHANGE                 | Low           | ZERO-TO-ONE TO ZERO-TO-MANY                                       | High           | ZERO-TO-MANY TO  ZERO-TO-ONE                                     |
| Contactpersoon | NL-CM:3.1.6      | Contactgegevens    |                  | groen: geen wijzigingen | NL-CM:3.1.6      | Contactgegevens    |                  |                                         |                                                                                                                                              |                                    |               |                                                                   |                |                                                                  |

