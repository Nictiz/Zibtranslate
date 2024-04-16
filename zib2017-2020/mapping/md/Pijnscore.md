# Pijnscore
## File formats

The translation specs are available as: 
[CSV](../csv/Pijnscore.csv) [JSON](../json/Pijnscore.json) [XML](../xml/Pijnscore.xml)



[Pijnscore-v3.1(2017NL)](https://zibs.nl/wiki/Pijnscore-v3.1(2017NL))

[Pijnscore-v4.0(2020NL)](https://zibs.nl/wiki/Pijnscore-v4.0(2020NL))









## Changes

| ConceptID_2017   | ConceptName_2017   | Change               | TypeChange                         | Impact_heen   | TRANSLATIE_spec_heen                                                                                              | Impact_terug   | TRANSLATIE_spec_terug                                                | Omschrijving                              |
|:-----------------|:-------------------|:---------------------|:-----------------------------------|:--------------|:------------------------------------------------------------------------------------------------------------------|:---------------|:---------------------------------------------------------------------|:------------------------------------------|
| NL-CM:12.9.1     | PijnScore          | oranje: minor change | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefintionCode [blank] -> [425401001 Pain intensity rating scale]                                              | Medium         | SCT DefintionCode [425401001 Pain intensity rating scale] -> [blank] | SNOMED CT DefintionCode concept aangepast |
| NL-CM:12.9.6     | AnatomischeLocatie | rood: major change   | CONCEPT REMOVED                    | High          | IF [blank]source->target ELSE [toon en stuur de inhoud van dit data item als vrije tekst naar een 2020 ontvanger] | Low            |                                                                      | anatomische locatie verwijderd            |
| NL-CM:12.9.7     | Lateraliteit       | rood: major change   | CONCEPT REMOVED                    | High          | IF [blank]source->target ELSE [toon en stuur de inhoud van dit data item als vrije tekst naar een 2020 ontvanger] | Low            |                                                                      | anatomische locatie verwijderd            |

## Mapping

| ZibName   | ConceptID_2017   | ConceptName_2017   | Codelists_2017                  | Change                  | ConceptID_2020   | ConceptName_2020               | Codelists_2020           | Bits              | Omschrijving                              | TypeChange                         | Impact_heen   | TRANSLATIE_spec_heen                                                                                              | Impact_terug   | TRANSLATIE_spec_terug                                                |
|:----------|:-----------------|:-------------------|:--------------------------------|:------------------------|:-----------------|:-------------------------------|:-------------------------|:------------------|:------------------------------------------|:-----------------------------------|:--------------|:------------------------------------------------------------------------------------------------------------------|:---------------|:---------------------------------------------------------------------|
| Pijnscore | NL-CM:12.9.1     | PijnScore          |                                 | oranje: minor change    | NL-CM:12.9.1     | PijnScore                      |                          | ZIB-927           | SNOMED CT DefintionCode concept aangepast | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefintionCode [blank] -> [425401001 Pain intensity rating scale]                                              | Medium         | SCT DefintionCode [425401001 Pain intensity rating scale] -> [blank] |
| Pijnscore | NL-CM:12.9.2     | PijnscoreWaarde    |                                 | groen: geen wijzigingen | NL-CM:12.9.2     | PijnscoreWaarde                |                          |                   |                                           |                                    |               |                                                                                                                   |                |                                                                      |
| Pijnscore | NL-CM:12.9.3     | PijnscoreDatumTijd |                                 | groen: geen wijzigingen | NL-CM:12.9.3     | PijnscoreDatumTijd             |                          |                   |                                           |                                    |               |                                                                                                                   |                |                                                                      |
| Pijnscore | NL-CM:12.9.4     | PijnMeetmethode    | PijnMeetmethodeCodelijst        | groen: geen wijzigingen | NL-CM:12.9.4     | PijnMeetmethode                | PijnMeetmethodeCodelijst |                   |                                           |                                    |               |                                                                                                                   |                |                                                                      |
| Pijnscore | NL-CM:12.9.5     | Toelichting        |                                 | groen: geen wijzigingen | NL-CM:12.9.5     | Toelichting                    |                          |                   |                                           |                                    |               |                                                                                                                   |                |                                                                      |
| Pijnscore | NL-CM:12.9.6     | AnatomischeLocatie | PijnAnatomischeLocatieCodelijst | rood: major change      | NL-CM:12.9.6     | **concept verwijderd in 2020** |                          | ZIB-979 ; ZIB-766 | anatomische locatie verwijderd            | CONCEPT REMOVED                    | High          | IF [blank]source->target ELSE [toon en stuur de inhoud van dit data item als vrije tekst naar een 2020 ontvanger] | Low            |                                                                      |
| Pijnscore | NL-CM:12.9.7     | Lateraliteit       | PijnLateraliteitCodelijst       | rood: major change      | NL-CM:12.9.7     | **concept verwijderd in 2020** |                          | ZIB-979 ; ZIB-766 | anatomische locatie verwijderd            | CONCEPT REMOVED                    | High          | IF [blank]source->target ELSE [toon en stuur de inhoud van dit data item als vrije tekst naar een 2020 ontvanger] | Low            |                                                                      |

