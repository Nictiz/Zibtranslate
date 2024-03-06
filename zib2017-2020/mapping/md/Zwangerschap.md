# Zwangerschap
## File formats

The translation specs are available as: 
[CSV](../csv/Zwangerschap.csv) [JSON](../json/Zwangerschap.json) [XML](../xml/Zwangerschap.xml) [Excel](../excel/Zwangerschap.xlsx)



## Zib Zwangerschap

[Zwangerschap-v3.1(2017NL)](https://zibs.nl/wiki/Zwangerschap-v3.1(2017NL))

[Zwangerschap-v4.0(2020NL)](https://zibs.nl/wiki/Zwangerschap-v4.0(2020NL))









## Changes

| ConceptID_2017   | ConceptName_2017               | Change                | TypeChange                         | Impact_heen   | TRANSLATIE_spec_heen                                                                                                                | Impact_terug   | TRANSLATIE_spec_terug                                                                                                                  | Omschrijving                                                                  |
|:-----------------|:-------------------------------|:----------------------|:-----------------------------------|:--------------|:------------------------------------------------------------------------------------------------------------------------------------|:---------------|:---------------------------------------------------------------------------------------------------------------------------------------|:------------------------------------------------------------------------------|
| NL-CM:7.14.1     | Zwangerschap                   | oranje: minor change  | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefinitionCode [364320009 Pregnancy observable] -> [118185001 bevinding betreffende zwangerschap]                               | Medium         | SCT DefinitionCode [118185001 bevinding betreffende zwangerschap] -> [364320009 Pregnancy observable]                                  | SNOMED CT DefintionCode concept aangepast                                     |
| NL-CM:7.14.2     | Zwanger                        | rood: major change    | CONCEPT REMOVED                    | High          | IF [blank]source->target ELSE [toon en stuur de inhoud van dit data item als vrije tekst naar een 2020 ontvanger]                   | Low            |                                                                                                                                        | Boolean concept zwanger is verwijderd.                                        |
| NL-CM:7.14.3     | ATermeDatum                    | geel: patch wijziging | SIMPLE PATCH CHANGE (EN)           | Low           |                                                                                                                                     | Low            |                                                                                                                                        | Kleine tekstwijzing in engelse vertaling "term date" naar ''due date''.       |
| NL-CM:7.14.5     | Graviditeit                    | oranje: minor change  | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefintionCode [blank] -> [161732006 Gravida]; LOINC DefintionCode[11996-6 Pregnancies] ->[blank]                                | Medium         | SCT DefintionCode [161732006 Gravida] ->[blank] ; LOINC DefintionCode [blank] -> [11996-6 Pregnancies]                                 | SNOMED CT en LOINC DefintionCodes concept aangepast                           |
| NL-CM:7.14.6     | Pariteit                       | oranje: minor change  | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefintionCode [blank] -> [364325004 Pariteit]; LOINC DefintionCode[11977-6 Parity] ->[blank]                                    | Medium         | SCT DefintionCode [364325004 Pariteit] -> [blank] ; LOINC DefintionCode [blank] -> [11977-6 Parity]                                    | SNOMED CT en LOINC DefintionCodes concept aangepast                           |
| NL-CM:7.14.7     | Toelichting                    | oranje: minor change  | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefintionCode [blank] -> [161714006 Estimated date of delivery]; LOINC DefintionCode[11778-8 Delivery date Estimated] ->[blank] | Medium         | SCT DefintionCode [161714006 Estimated date of delivery] -> [blank] ; LOINC DefintionCode [blank] -> [11778-8 Delivery date Estimated] | SNOMED CT en LOINC DefintionCodes concept aangepast                           |
| NL-CM:7.14.8     | DatumLaatsteMenstruatie        | rood: major change    | CONCEPT ADDITION                   | Low           |                                                                                                                                     | High           | IF [blank]source->target ELSE [toon en stuur de inhoud van dit data item als vrije tekst naar een 2017 ontvanger]                      | AtermeDatum container met onderliggende elementen zijn toegevoegd aan de zib. |
| NL-CM:7.14.9     | **concept toegevoegd in 2020** | rood: major change    | CONCEPT ADDITION                   | Low           |                                                                                                                                     | High           | IF [blank]source->target ELSE [toon en stuur de inhoud van dit data item als vrije tekst naar een 2017 ontvanger]                      | AtermeDatum container met onderliggende elementen zijn toegevoegd aan de zib. |
| NL-CM:7.14.10    | **concept toegevoegd in 2020** | rood: major change    | CONCEPT ADDITION                   | Low           |                                                                                                                                     | High           | IF [blank]source->target ELSE [toon en stuur de inhoud van dit data item als vrije tekst naar een 2017 ontvanger]                      | AtermeDatum container met onderliggende elementen zijn toegevoegd aan de zib. |
| NL-CM:7.14.11    | **concept toegevoegd in 2020** | rood: major change    | CONCEPT ADDITION                   | Low           |                                                                                                                                     | High           | IF [blank]source->target ELSE [toon en stuur de inhoud van dit data item als vrije tekst naar een 2017 ontvanger]                      | AtermeDatum container met onderliggende elementen zijn toegevoegd aan de zib. |

## Mapping

| ConceptID_2017   | ConceptName_2017               | Codelists_2017   | Change                  | ConceptID_2020   | ConceptName_2020               | Codelists_2020            | Bits     | Omschrijving                                                                  | TypeChange                         | Impact_heen   | TRANSLATIE_spec_heen                                                                                                                | Impact_terug   | TRANSLATIE_spec_terug                                                                                                                  |
|:-----------------|:-------------------------------|:-----------------|:------------------------|:-----------------|:-------------------------------|:--------------------------|:---------|:------------------------------------------------------------------------------|:-----------------------------------|:--------------|:------------------------------------------------------------------------------------------------------------------------------------|:---------------|:---------------------------------------------------------------------------------------------------------------------------------------|
| NL-CM:7.14.1     | Zwangerschap                   |                  | oranje: minor change    | NL-CM:7.14.1     | Zwangerschap                   |                           | ZIB-1201 | SNOMED CT DefintionCode concept aangepast                                     | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefinitionCode [364320009 Pregnancy observable] -> [118185001 bevinding betreffende zwangerschap]                               | Medium         | SCT DefinitionCode [118185001 bevinding betreffende zwangerschap] -> [364320009 Pregnancy observable]                                  |
| NL-CM:7.14.2     | Zwanger                        |                  | rood: major change      | NL-CM:7.14.2     | **concept verwijderd in 2020** |                           | ZIB-890  | Boolean concept zwanger is verwijderd.                                        | CONCEPT REMOVED                    | High          | IF [blank]source->target ELSE [toon en stuur de inhoud van dit data item als vrije tekst naar een 2020 ontvanger]                   | Low            |                                                                                                                                        |
| NL-CM:7.14.3     | ATermeDatum                    |                  | geel: patch wijziging   | NL-CM:7.14.3     | ATermeDatum                    |                           | ZIB-907  | Kleine tekstwijzing in engelse vertaling "term date" naar ''due date''.       | SIMPLE PATCH CHANGE (EN)           | Low           |                                                                                                                                     | Low            |                                                                                                                                        |
| NL-CM:7.14.4     | Zwangerschapsduur              |                  | groen: geen wijzigingen | NL-CM:7.14.4     | Zwangerschapsduur              |                           |          |                                                                               |                                    |               |                                                                                                                                     |                |                                                                                                                                        |
| NL-CM:7.14.5     | Graviditeit                    |                  | oranje: minor change    | NL-CM:7.14.5     | Graviditeit                    |                           | ZIB-890  | SNOMED CT en LOINC DefintionCodes concept aangepast                           | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefintionCode [blank] -> [161732006 Gravida]; LOINC DefintionCode[11996-6 Pregnancies] ->[blank]                                | Medium         | SCT DefintionCode [161732006 Gravida] ->[blank] ; LOINC DefintionCode [blank] -> [11996-6 Pregnancies]                                 |
| NL-CM:7.14.6     | Pariteit                       |                  | oranje: minor change    | NL-CM:7.14.6     | Pariteit                       |                           | ZIB-890  | SNOMED CT en LOINC DefintionCodes concept aangepast                           | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefintionCode [blank] -> [364325004 Pariteit]; LOINC DefintionCode[11977-6 Parity] ->[blank]                                    | Medium         | SCT DefintionCode [364325004 Pariteit] -> [blank] ; LOINC DefintionCode [blank] -> [11977-6 Parity]                                    |
| NL-CM:7.14.7     | Toelichting                    |                  | oranje: minor change    | NL-CM:7.14.7     | Toelichting                    |                           | ZIB-890  | SNOMED CT en LOINC DefintionCodes concept aangepast                           | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefintionCode [blank] -> [161714006 Estimated date of delivery]; LOINC DefintionCode[11778-8 Delivery date Estimated] ->[blank] | Medium         | SCT DefintionCode [161714006 Estimated date of delivery] -> [blank] ; LOINC DefintionCode [blank] -> [11778-8 Delivery date Estimated] |
| NL-CM:7.14.8     | DatumLaatsteMenstruatie        |                  | rood: major change      | NL-CM:7.14.8     | DatumLaatsteMenstruatie        |                           | ZIB-890  | AtermeDatum container met onderliggende elementen zijn toegevoegd aan de zib. | CONCEPT ADDITION                   | Low           |                                                                                                                                     | High           | IF [blank]source->target ELSE [toon en stuur de inhoud van dit data item als vrije tekst naar een 2017 ontvanger]                      |
| NL-CM:7.14.9     | **concept toegevoegd in 2020** |                  | rood: major change      | NL-CM:7.14.9     | ATermeDatumItems               |                           | ZIB-890  | AtermeDatum container met onderliggende elementen zijn toegevoegd aan de zib. | CONCEPT ADDITION                   | Low           |                                                                                                                                     | High           | IF [blank]source->target ELSE [toon en stuur de inhoud van dit data item als vrije tekst naar een 2017 ontvanger]                      |
| NL-CM:7.14.10    | **concept toegevoegd in 2020** |                  | rood: major change      | NL-CM:7.14.10    | BepalingsMethode               | BepalingsMethodeCodelijst | ZIB-890  | AtermeDatum container met onderliggende elementen zijn toegevoegd aan de zib. | CONCEPT ADDITION                   | Low           |                                                                                                                                     | High           | IF [blank]source->target ELSE [toon en stuur de inhoud van dit data item als vrije tekst naar een 2017 ontvanger]                      |
| NL-CM:7.14.11    | **concept toegevoegd in 2020** |                  | rood: major change      | NL-CM:7.14.11    | DatumBepaling                  |                           | ZIB-890  | AtermeDatum container met onderliggende elementen zijn toegevoegd aan de zib. | CONCEPT ADDITION                   | Low           |                                                                                                                                     | High           | IF [blank]source->target ELSE [toon en stuur de inhoud van dit data item als vrije tekst naar een 2017 ontvanger]                      |
