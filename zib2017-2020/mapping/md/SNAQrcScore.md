# SNAQrcScore
## File formats

The translation specs are available as: 
[CSV](../csv/SNAQrcScore.csv) [JSON](../json/SNAQrcScore.json) [XML](../xml/SNAQrcScore.xml) [Excel](../excel/SNAQrcScore.xlsx)



## Zib SNAQrcScore

[SNAQrcScore-v1.0(2017NL)](https://zibs.nl/wiki/SNAQrcScore-v1.0(2017NL))

[SNAQrcScore-v1.1(2020NL)](https://zibs.nl/wiki/SNAQrcScore-v1.1(2020NL))









## Changes

| ConceptID_2017   | ConceptName_2017     | Change               | TypeChange                         | Impact_heen   | TRANSLATIE_spec_heen                                                                                             | Impact_terug   | TRANSLATIE_spec_terug                                                                                            | Omschrijving                              |
|:-----------------|:---------------------|:---------------------|:-----------------------------------|:--------------|:-----------------------------------------------------------------------------------------------------------------|:---------------|:-----------------------------------------------------------------------------------------------------------------|:------------------------------------------|
| NL-CM:4.29.1     | SNAQrcScore          | oranje: minor change | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefinitionCode [blank] -> [108311000146106 SNAQRC]                                                           | Medium         | SCT DefinitionCode [108311000146106 SNAQRC] -> [blank]                                                           | SNOMED CT DefintionCode concept aangepast |
| NL-CM:4.29.2     | TotaalScore          | oranje: minor change | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefinitionCode [blank] -> [108901000146105 Short Nutritional Questionnaire for residential care total score] | Medium         | SCT DefinitionCode [108901000146105 Short Nutritional Questionnaire for residential care total score] -> [blank] | SNOMED CT DefintionCode concept aangepast |
| NL-CM:4.29.3     | GewichtsverliesScore | oranje: minor change | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefinitionCode [blank] -> [4029003 SNAQrcScore GewichtsverliesScore]                                         | Medium         | SCT DefinitionCode [4029003 SNAQrcScore GewichtsverliesScore] -> [blank]                                         | SNOMED CT DefintionCode concept aangepast |
| NL-CM:4.29.4     | EetlustScore         | oranje: minor change | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefinitionCode [blank] -> [4029004 SNAQrcScore EetlustScore]                                                 | Medium         | SCT DefinitionCode [4029004 SNAQrcScore EetlustScore] -> [blank]                                                 | SNOMED CT DefintionCode concept aangepast |
| NL-CM:4.29.5     | BMIScore             | oranje: minor change | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefinitionCode [blank] -> [4029005 SNAQrcScore BMIScore]                                                     | Medium         | SCT DefinitionCode [4029005 SNAQrcScore BMIScore] -> [blank]                                                     | SNOMED CT DefintionCode concept aangepast |
| NL-CM:4.29.8     | HulpBijEten          | oranje: minor change | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefinitionCode [blank] -> [4029008 SNAQrcScore HulpBijEten]                                                  | Medium         | SCT DefinitionCode [4029008 SNAQrcScore HulpBijEten] -> [blank]                                                  | SNOMED CT DefintionCode concept aangepast |

## Mapping

| ConceptID_2017   | ConceptName_2017     | Codelists_2017                      | Change                  | ConceptID_2020   | ConceptName_2020     | Codelists_2020                      | Bits    | Omschrijving                              | TypeChange                         | Impact_heen   | TRANSLATIE_spec_heen                                                                                             | Impact_terug   | TRANSLATIE_spec_terug                                                                                            |
|:-----------------|:---------------------|:------------------------------------|:------------------------|:-----------------|:---------------------|:------------------------------------|:--------|:------------------------------------------|:-----------------------------------|:--------------|:-----------------------------------------------------------------------------------------------------------------|:---------------|:-----------------------------------------------------------------------------------------------------------------|
| NL-CM:4.29.1     | SNAQrcScore          |                                     | oranje: minor change    | NL-CM:4.29.1     | SNAQrcScore          |                                     | ZIB-930 | SNOMED CT DefintionCode concept aangepast | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefinitionCode [blank] -> [108311000146106 SNAQRC]                                                           | Medium         | SCT DefinitionCode [108311000146106 SNAQRC] -> [blank]                                                           |
| NL-CM:4.29.2     | TotaalScore          |                                     | oranje: minor change    | NL-CM:4.29.2     | TotaalScore          |                                     | ZIB-930 | SNOMED CT DefintionCode concept aangepast | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefinitionCode [blank] -> [108901000146105 Short Nutritional Questionnaire for residential care total score] | Medium         | SCT DefinitionCode [108901000146105 Short Nutritional Questionnaire for residential care total score] -> [blank] |
| NL-CM:4.29.3     | GewichtsverliesScore | SNAQrcGewichtsverliesScoreCodelijst | oranje: minor change    | NL-CM:4.29.3     | GewichtsverliesScore | SNAQrcGewichtsverliesScoreCodelijst | ZIB-930 | SNOMED CT DefintionCode concept aangepast | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefinitionCode [blank] -> [4029003 SNAQrcScore GewichtsverliesScore]                                         | Medium         | SCT DefinitionCode [4029003 SNAQrcScore GewichtsverliesScore] -> [blank]                                         |
| NL-CM:4.29.4     | EetlustScore         | SNAQrcEetlustScoreCodelijst         | oranje: minor change    | NL-CM:4.29.4     | EetlustScore         | SNAQrcEetlustScoreCodelijst         | ZIB-930 | SNOMED CT DefintionCode concept aangepast | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefinitionCode [blank] -> [4029004 SNAQrcScore EetlustScore]                                                 | Medium         | SCT DefinitionCode [4029004 SNAQrcScore EetlustScore] -> [blank]                                                 |
| NL-CM:4.29.5     | BMIScore             | SNAQrcBMIScoreCodelijst             | oranje: minor change    | NL-CM:4.29.5     | BMIScore             | SNAQrcBMIScoreCodelijst             | ZIB-930 | SNOMED CT DefintionCode concept aangepast | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefinitionCode [blank] -> [4029005 SNAQrcScore BMIScore]                                                     | Medium         | SCT DefinitionCode [4029005 SNAQrcScore BMIScore] -> [blank]                                                     |
| NL-CM:4.29.6     | SNAQrcScoreDatumTijd |                                     | groen: geen wijzigingen | NL-CM:4.29.6     | SNAQrcScoreDatumTijd |                                     |         |                                           |                                    |               |                                                                                                                  |                |                                                                                                                  |
| NL-CM:4.29.7     | Toelichting          |                                     | groen: geen wijzigingen | NL-CM:4.29.7     | Toelichting          |                                     |         |                                           |                                    |               |                                                                                                                  |                |                                                                                                                  |
| NL-CM:4.29.8     | HulpBijEten          | SNAQrcHulpBijEtenCodelijst          | oranje: minor change    | NL-CM:4.29.8     | HulpBijEten          | SNAQrcHulpBijEtenCodelijst          | ZIB-930 | SNOMED CT DefintionCode concept aangepast | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefinitionCode [blank] -> [4029008 SNAQrcScore HulpBijEten]                                                  | Medium         | SCT DefinitionCode [4029008 SNAQrcScore HulpBijEten] -> [blank]                                                  |

