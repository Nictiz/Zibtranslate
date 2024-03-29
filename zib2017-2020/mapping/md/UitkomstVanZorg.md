# UitkomstVanZorg
## File formats

The translation specs are available as: 
[CSV](../csv/UitkomstVanZorg.csv) [JSON](../json/UitkomstVanZorg.json) [XML](../xml/UitkomstVanZorg.xml) [Excel](../excel/UitkomstVanZorg.xlsx)



## Zib UitkomstVanZorg

[UitkomstVanZorg-v3.1(2017NL)](https://zibs.nl/wiki/UitkomstVanZorg-v3.1(2017NL))

[UitkomstVanZorg-v3.2(2020NL)](https://zibs.nl/wiki/UitkomstVanZorg-v3.2(2020NL))









## Changes

| ConceptID_2017   | ConceptName_2017                        | Change               | TypeChange                         | Impact_heen   | TRANSLATIE_spec_heen                                                                                                      | Impact_terug   | TRANSLATIE_spec_terug                                                                                                      | Omschrijving                                                                       |
|:-----------------|:----------------------------------------|:---------------------|:-----------------------------------|:--------------|:--------------------------------------------------------------------------------------------------------------------------|:---------------|:---------------------------------------------------------------------------------------------------------------------------|:-----------------------------------------------------------------------------------|
| NL-CM:13.4.1     | UitkomstVanZorg                         | oranje: minor change | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefinitionCode [blank] -> [423100009 Results section]                                                                  | Medium         | SCT DefinitionCode [423100009 Results section] -> [blank]                                                                   | SNOMED CT DefinitionCode concept aangepast                                          |
| NL-CM:13.4.2     | Meetwaarde::AlgemeneMeting              | rood: major change   | CONCEPT REMOVED                    | High          | IF [blank] source->target ELSE [stuur de data van de algemeneMeting instance als vrije tekst naar een 2020 ontvanger]     | Low            |                                                                                                                            | Data reference naar zib AlgemeneMeting is verwijderd                               |
| NL-CM:13.4.4     | Interventie::VerpleegkundigeInterventie | rood: major change   | CARDINALITY CHANGE                 | Low           | ZERO-TO-ONE TO ZERO-TO-MANY                                                                                               | High           | ZERO-TO-MANY TO ZERO-TO-ONE                                                                                                | Relatie naar VerpleegkundigeInterventie (Interventie) veranderd van 0..1 naar 0..* |
| NL-CM:13.4.5     | Zorgresultaat                           | oranje: minor change | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | LOINC DefinitionCode [27574-3 Skilled nursing treatment plan Progress note and attainment of goals (narrative)] -> [blank] | Medium         | LOINC DefinitionCode [blank] ->  [27574-3 Skilled nursing treatment plan Progress note and attainment of goals (narrative)] | SNOMED CT DefinitionCode concept aangepast                                          |

## Mapping

| ConceptID_2017   | ConceptName_2017                                | Codelists_2017   | Change                  | ConceptID_2020   | ConceptName_2020                                | Codelists_2020   | Bits     | Omschrijving                                                                       | TypeChange                         | Impact_heen   | TRANSLATIE_spec_heen                                                                                                      | Impact_terug   | TRANSLATIE_spec_terug                                                                                                      |
|:-----------------|:------------------------------------------------|:-----------------|:------------------------|:-----------------|:------------------------------------------------|:-----------------|:---------|:-----------------------------------------------------------------------------------|:-----------------------------------|:--------------|:--------------------------------------------------------------------------------------------------------------------------|:---------------|:---------------------------------------------------------------------------------------------------------------------------|
| NL-CM:13.4.1     | UitkomstVanZorg                                 |                  | oranje: minor change    | NL-CM:13.4.1     | UitkomstVanZorg                                 |                  | ZIB-1158 | SNOMED CT DefinitionCode concept aangepast                                          | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefinitionCode [blank] -> [423100009 Results section]                                                                  | Medium         | SCT DefinitionCode [423100009 Results section] -> [blank]                                                                   |
| NL-CM:13.4.2     | Meetwaarde::AlgemeneMeting                      |                  | rood: major change      | NL-CM:13.4.2     | **concept verwijderd in 2020**                  |                  | ZIB-1158 | Data reference naar zib AlgemeneMeting is verwijderd                               | CONCEPT REMOVED                    | High          | IF [blank] source->target ELSE [stuur de data van de algemeneMeting instance als vrije tekst naar een 2020 ontvanger]     | Low            |                                                                                                                            |
| NL-CM:13.4.3     | Gezondheidstoestand::FunctioneleOfMentaleStatus |                  | groen: geen wijzigingen | NL-CM:13.4.3     | Gezondheidstoestand::FunctioneleOfMentaleStatus |                  |          |                                                                                    |                                    |               |                                                                                                                           |                |                                                                                                                            |
| NL-CM:13.4.4     | Interventie::VerpleegkundigeInterventie         |                  | rood: major change      | NL-CM:13.4.4     | Interventie::VerpleegkundigeInterventie         |                  | ZIB-1154 | Relatie naar VerpleegkundigeInterventie (Interventie) veranderd van 0..1 naar 0..* | CARDINALITY CHANGE                 | Low           | ZERO-TO-ONE TO ZERO-TO-MANY                                                                                               | High           | ZERO-TO-MANY TO ZERO-TO-ONE                                                                                                |
| NL-CM:13.4.5     | Zorgresultaat                                   |                  | oranje: minor change    | NL-CM:13.4.5     | Zorgresultaat                                   |                  | ZIB-1158 | SNOMED CT DefinitionCode concept aangepast                                          | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | LOINC DefinitionCode [27574-3 Skilled nursing treatment plan Progress note and attainment of goals (narrative)] -> [blank] | Medium         | LOINC DefinitionCode [blank] ->  [27574-3 Skilled nursing treatment plan Progress note and attainment of goals (narrative)] |

