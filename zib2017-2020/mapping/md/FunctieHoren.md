# FunctieHoren
## File formats

The translation specs are available as: 
[CSV](../csv/FunctieHoren.csv) [JSON](../json/FunctieHoren.json) [XML](../xml/FunctieHoren.xml)



[FunctieHoren-v3.1(2017NL)](https://zibs.nl/wiki/FunctieHoren-v3.1(2017NL))

[FunctieHoren-v3.2(2020NL)](https://zibs.nl/wiki/FunctieHoren-v3.2(2020NL))









## Changes

| ConceptID_2017   | ConceptName_2017                   | Change               | TypeChange                         | Impact_heen   | TRANSLATIE_spec_heen                                                   | Impact_terug   | TRANSLATIE_spec_terug                                                  | Omschrijving                                |
|:-----------------|:-----------------------------------|:---------------------|:-----------------------------------|:--------------|:-----------------------------------------------------------------------|:---------------|:-----------------------------------------------------------------------|:--------------------------------------------|
| NL-CM:4.17.4     | HorenHulpmiddel::MedischHulpmiddel | oranje: minor change | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefinitionCode [272182005 Aid to hearing] -> [6012004 Hoortoestel] | Medium         | SCT DefinitionCode [6012004 Hoortoestel] -> [272182005 Aid to hearing] | DefinitionCode aangepast                    |
| NL-CM:10.1.3     | ProductType                        | oranje: minor change | VALUESET CHANGES                   | Low           | existing valueset [valuesetname] changed in [baseline 2020]            | Medium         | existing valueset [valuesetname] changed in [baseline 2020]            | Foutieve Snomed code aangepast in codelijst |

## Mapping

| ZibName      | ConceptID_2017   | ConceptName_2017                   | Codelists_2017               | Change                  | ConceptID_2020   | ConceptName_2020                   | Codelists_2020               | Bits    | Omschrijving                                | TypeChange                         | Impact_heen   | TRANSLATIE_spec_heen                                                   | Impact_terug   | TRANSLATIE_spec_terug                                                  |
|:-------------|:-----------------|:-----------------------------------|:-----------------------------|:------------------------|:-----------------|:-----------------------------------|:-----------------------------|:--------|:--------------------------------------------|:-----------------------------------|:--------------|:-----------------------------------------------------------------------|:---------------|:-----------------------------------------------------------------------|
| FunctieHoren | NL-CM:4.17.1     | FunctieHoren                       |                              | groen: geen wijzigingen | NL-CM:4.17.1     | FunctieHoren                       |                              |         |                                             |                                    |               |                                                                        |                |                                                                        |
| FunctieHoren | NL-CM:4.17.2     | Toelichting                        |                              | groen: geen wijzigingen | NL-CM:4.17.2     | Toelichting                        |                              |         |                                             |                                    |               |                                                                        |                |                                                                        |
| FunctieHoren | NL-CM:4.17.3     | HoorFunctie                        | HoorFunctieCodelijst         | groen: geen wijzigingen | NL-CM:4.17.3     | HoorFunctie                        | HoorFunctieCodelijst         |         |                                             |                                    |               |                                                                        |                |                                                                        |
| FunctieHoren | NL-CM:4.17.4     | HorenHulpmiddel::MedischHulpmiddel |                              | oranje: minor change    | NL-CM:4.17.4     | HorenHulpmiddel::MedischHulpmiddel |                              | ZIB-732 | DefinitionCode aangepast                    | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefinitionCode [272182005 Aid to hearing] -> [6012004 Hoortoestel] | Medium         | SCT DefinitionCode [6012004 Hoortoestel] -> [272182005 Aid to hearing] |
| FunctieHoren | NL-CM:10.1.3     | ProductType                        | HorenHulpmiddelTypeCodelijst | oranje: minor change    | NL-CM:10.1.3     | ProductType                        | HorenHulpmiddelTypeCodelijst | ZIB-732 | Foutieve Snomed code aangepast in codelijst | VALUESET CHANGES                   | Low           | existing valueset [valuesetname] changed in [baseline 2020]            | Medium         | existing valueset [valuesetname] changed in [baseline 2020]            |
| FunctieHoren | NL-CM:10.1.6     | HulpmiddelAnatomischeLocatie       |                              | groen: geen wijzigingen | NL-CM:10.1.6     | HulpmiddelAnatomischeLocatie       |                              |         |                                             |                                    |               |                                                                        |                |                                                                        |

