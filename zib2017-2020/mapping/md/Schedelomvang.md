# Schedelomvang
## File formats

The translation specs are available as: 
[CSV](../csv/Schedelomvang.csv) [JSON](../json/Schedelomvang.json) [XML](../xml/Schedelomvang.xml)



[Schedelomvang-v1.1(2017NL)](https://zibs.nl/wiki/Schedelomvang-v1.1(2017NL))

[Schedelomvang-v1.3(2020NL)](https://zibs.nl/wiki/Schedelomvang-v1.3(2020NL))









## Changes

| ConceptID_2017   | ConceptName_2017    | Change                | TypeChange                         | Impact_heen   | TRANSLATIE_spec_heen                                                          | Impact_terug   | TRANSLATIE_spec_terug                                                          | Omschrijving                                                                                                                                |
|:-----------------|:--------------------|:----------------------|:-----------------------------------|:--------------|:------------------------------------------------------------------------------|:---------------|:-------------------------------------------------------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------|
| NL-CM:12.14.1    | Schedelomvang       | oranje: minor change  | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | LOINC DefinitionCode [blank] -> [9843-4 Head Occipital-frontal circumference] | Medium         | LOINC DefinitionCode [9843-4 Head Occipital-frontal circumference] ->  [blank] | LOINC DefintionCodes concept aangepast                                                                                                      |
| NL-CM:12.14.3    | SchedelomvangWaarde | geel: patch wijziging | SIMPLE PATCH CHANGE                | Low           |                                                                               | Low            |                                                                                | Bij de definitie van  concept Schedelomvangwaarde is toegevoegd dat het resultaat ook in mm kan worden vastgelegd. Dit was eerst alleen cm. |

## Mapping

| ZibName       | ConceptID_2017   | ConceptName_2017         | Codelists_2017                    | Change                  | ConceptID_2020   | ConceptName_2020         | Codelists_2020                    | Bits    | Omschrijving                                                                                                                                | TypeChange                         | Impact_heen   | TRANSLATIE_spec_heen                                                          | Impact_terug   | TRANSLATIE_spec_terug                                                          |
|:--------------|:-----------------|:-------------------------|:----------------------------------|:------------------------|:-----------------|:-------------------------|:----------------------------------|:--------|:--------------------------------------------------------------------------------------------------------------------------------------------|:-----------------------------------|:--------------|:------------------------------------------------------------------------------|:---------------|:-------------------------------------------------------------------------------|
| Schedelomvang | NL-CM:12.14.1    | Schedelomvang            |                                   | oranje: minor change    | NL-CM:12.14.1    | Schedelomvang            |                                   | ZIB-928 | LOINC DefintionCodes concept aangepast                                                                                                      | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | LOINC DefinitionCode [blank] -> [9843-4 Head Occipital-frontal circumference] | Medium         | LOINC DefinitionCode [9843-4 Head Occipital-frontal circumference] ->  [blank] |
| Schedelomvang | NL-CM:12.14.2    | SchedelomvangDatumTijd   |                                   | groen: geen wijzigingen | NL-CM:12.14.2    | SchedelomvangDatumTijd   |                                   |         |                                                                                                                                             |                                    |               |                                                                               |                |                                                                                |
| Schedelomvang | NL-CM:12.14.3    | SchedelomvangWaarde      |                                   | geel: patch wijziging   | NL-CM:12.14.3    | SchedelomvangWaarde      |                                   | ZIB-858 | Bij de definitie van  concept Schedelomvangwaarde is toegevoegd dat het resultaat ook in mm kan worden vastgelegd. Dit was eerst alleen cm. | SIMPLE PATCH CHANGE                | Low           |                                                                               | Low            |                                                                                |
| Schedelomvang | NL-CM:12.14.4    | Toelichting              |                                   | groen: geen wijzigingen | NL-CM:12.14.4    | Toelichting              |                                   |         |                                                                                                                                             |                                    |               |                                                                               |                |                                                                                |
| Schedelomvang | NL-CM:12.14.5    | SchedelomvangMeetmethode | SchedelomvangMeetmethodeCodelijst | groen: geen wijzigingen | NL-CM:12.14.5    | SchedelomvangMeetmethode | SchedelomvangMeetmethodeCodelijst |         |                                                                                                                                             |                                    |               |                                                                               |                |                                                                                |

