# Behandeldoel
## File formats

The translation specs are available as: 
[CSV](../csv/Behandeldoel.csv) [JSON](../json/Behandeldoel.json) [XML](../xml/Behandeldoel.xml)



[Behandeldoel-v3.1(2017NL)](https://zibs.nl/wiki/Behandeldoel-v3.1(2017NL))

[Behandeldoel-v3.2(2020NL)](https://zibs.nl/wiki/Behandeldoel-v3.2(2020NL))









## Changes

| ConceptID_2017   | ConceptName_2017             | Change               | TypeChange                         | Impact_heen   | TRANSLATIE_spec_heen                                                                                                                        | Impact_terug   | TRANSLATIE_spec_terug                                                                                                                       | Omschrijving                                   |
|:-----------------|:-----------------------------|:---------------------|:-----------------------------------|:--------------|:--------------------------------------------------------------------------------------------------------------------------------------------|:---------------|:--------------------------------------------------------------------------------------------------------------------------------------------|:-----------------------------------------------|
| NL-CM:13.5.2     | Streefwaarde::AlgemeneMeting | rood: major change   | CONCEPT REMOVED                    | High          | IF [blank] source->target ELSE [stuur de data van de algemeneMeting instance als vrije tekst naar een 2020 ontvanger]                       | Low            |                                                                                                                                             | referentie naar zib AlgemeneMeting verwijderd. |
| NL-CM:13.5.5     | GewenstZorgresultaat         | oranje: minor change | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefintionCode [27574-3 Skilled nursing treatment plan Progress note and attainment of goals (narrative)] -> [423100009 Results section] | Medium         | SCT DefintionCode [423100009 Results section] -> [27574-3 Skilled nursing treatment plan Progress note and attainment of goals (narrative)] | SNOMED CT DefintionCode concept aangepast      |

## Mapping

| ZibName      | ConceptID_2017   | ConceptName_2017                                        | Codelists_2017   | Change                  | ConceptID_2020   | ConceptName_2020                                        | Codelists_2020   | Bits     | Omschrijving                                   | TypeChange                         | Impact_heen   | TRANSLATIE_spec_heen                                                                                                                        | Impact_terug   | TRANSLATIE_spec_terug                                                                                                                       |
|:-------------|:-----------------|:--------------------------------------------------------|:-----------------|:------------------------|:-----------------|:--------------------------------------------------------|:-----------------|:---------|:-----------------------------------------------|:-----------------------------------|:--------------|:--------------------------------------------------------------------------------------------------------------------------------------------|:---------------|:--------------------------------------------------------------------------------------------------------------------------------------------|
| Behandeldoel | NL-CM:13.5.1     | Behandeldoel                                            |                  | groen: geen wijzigingen | NL-CM:13.5.1     | Behandeldoel                                            |                  |          |                                                |                                    |               |                                                                                                                                             |                |                                                                                                                                             |
| Behandeldoel | NL-CM:13.5.2     | Streefwaarde::AlgemeneMeting                            |                  | rood: major change      | NL-CM:13.5.2     | **concept verwijderd in 2020**                          |                  | ZIB-1174 | referentie naar zib AlgemeneMeting verwijderd. | CONCEPT REMOVED                    | High          | IF [blank] source->target ELSE [stuur de data van de algemeneMeting instance als vrije tekst naar een 2020 ontvanger]                       | Low            |                                                                                                                                             |
| Behandeldoel | NL-CM:13.5.3     | GewensteGezondheidstoestand::FunctioneleOfMentaleStatus |                  | groen: geen wijzigingen | NL-CM:13.5.3     | GewensteGezondheidstoestand::FunctioneleOfMentaleStatus |                  |          |                                                |                                    |               |                                                                                                                                             |                |                                                                                                                                             |
| Behandeldoel | NL-CM:13.5.4     | Probleem                                                |                  | groen: geen wijzigingen | NL-CM:13.5.4     | Probleem                                                |                  |          |                                                |                                    |               |                                                                                                                                             |                |                                                                                                                                             |
| Behandeldoel | NL-CM:13.5.5     | GewenstZorgresultaat                                    |                  | oranje: minor change    | NL-CM:13.5.5     | GewenstZorgresultaat                                    |                  | ZIB-1174 | SNOMED CT DefintionCode concept aangepast      | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefintionCode [27574-3 Skilled nursing treatment plan Progress note and attainment of goals (narrative)] -> [423100009 Results section] | Medium         | SCT DefintionCode [423100009 Results section] -> [27574-3 Skilled nursing treatment plan Progress note and attainment of goals (narrative)] |

