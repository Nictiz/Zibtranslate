# StrongKidsScore
## File formats

The translation specs are available as: 
[CSV](../csv/StrongKidsScore.csv) [JSON](../json/StrongKidsScore.json) [XML](../xml/StrongKidsScore.xml)



[StrongKidsScore-v1.0(2017NL)](https://zibs.nl/wiki/StrongKidsScore-v1.0(2017NL))

[StrongKidsScore-v1.1(2020NL)](https://zibs.nl/wiki/StrongKidsScore-v1.1(2020NL))









## Changes

| ConceptID_2017   | ConceptName_2017      | Change               | TypeChange                         | Impact_heen   | TRANSLATIE_spec_heen                                                                       | Impact_terug   | TRANSLATIE_spec_terug                                                                      | Omschrijving                              |
|:-----------------|:----------------------|:---------------------|:-----------------------------------|:--------------|:-------------------------------------------------------------------------------------------|:---------------|:-------------------------------------------------------------------------------------------|:------------------------------------------|
| NL-CM:4.28.1     | StrongKidsScore       | oranje: minor change | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefintionCode [blank] -> [108341000146107 STRONGkids-screeningsinstrument]             | Medium         | SCT DefintionCode [108341000146107 STRONGkids-screeningsinstrument] -> [blank]             | SNOMED CT DefintionCode concept aangepast |
| NL-CM:4.28.2     | TotaalScore           | oranje: minor change | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefintionCode [blank] -> [108911000146107 Short Nutritional Questionnaire total score] | Medium         | SCT DefintionCode [108911000146107 Short Nutritional Questionnaire total score] -> [blank] | SNOMED CT DefintionCode concept aangepast |
| NL-CM:4.28.3     | GewichtsverliesScore  | oranje: minor change | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefintionCode [blank] -> [4028003 StrongKidsScore GewichtsverliesScore]                | Medium         | SCT DefintionCode [4028003 StrongKidsScore GewichtsverliesScore] -> [blank]                | SNOMED CT DefintionCode concept aangepast |
| NL-CM:4.28.4     | ZiekteBeeldScore      | oranje: minor change | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefintionCode [blank] -> [4028004 StrongKidsScore ZiekteBeeldScore]                    | Medium         | SCT DefintionCode  [4028005 StrongKidsScore VoedingsScore] -> [blank]                      | SNOMED CT DefintionCode concept aangepast |
| NL-CM:4.28.5     | VoedingsScore         | oranje: minor change | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefintionCode [blank] -> [4028005 StrongKidsScore VoedingsScore]                       | Medium         | SCT DefintionCode [4028005 StrongKidsScore VoedingsScore] -> [blank]                       | SNOMED CT DefintionCode concept aangepast |
| NL-CM:4.28.8     | VoedingstoestandScore | oranje: minor change | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefintionCode [blank] -> [4028008 StrongKidsScore VoedingstoestandScore]               | Medium         | SCT DefintionCode [4028008 StrongKidsScore VoedingstoestandScore] -> [blank]               | SNOMED CT DefintionCode concept aangepast |

## Mapping

| ZibName         | ConceptID_2017   | ConceptName_2017      | Codelists_2017                  | Change                  | ConceptID_2020   | ConceptName_2020      | Codelists_2020                  | Bits    | Omschrijving                              | TypeChange                         | Impact_heen   | TRANSLATIE_spec_heen                                                                       | Impact_terug   | TRANSLATIE_spec_terug                                                                      |
|:----------------|:-----------------|:----------------------|:--------------------------------|:------------------------|:-----------------|:----------------------|:--------------------------------|:--------|:------------------------------------------|:-----------------------------------|:--------------|:-------------------------------------------------------------------------------------------|:---------------|:-------------------------------------------------------------------------------------------|
| StrongKidsScore | NL-CM:4.28.1     | StrongKidsScore       |                                 | oranje: minor change    | NL-CM:4.28.1     | StrongKidsScore       |                                 | ZIB-932 | SNOMED CT DefintionCode concept aangepast | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefintionCode [blank] -> [108341000146107 STRONGkids-screeningsinstrument]             | Medium         | SCT DefintionCode [108341000146107 STRONGkids-screeningsinstrument] -> [blank]             |
| StrongKidsScore | NL-CM:4.28.2     | TotaalScore           |                                 | oranje: minor change    | NL-CM:4.28.2     | TotaalScore           |                                 | ZIB-932 | SNOMED CT DefintionCode concept aangepast | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefintionCode [blank] -> [108911000146107 Short Nutritional Questionnaire total score] | Medium         | SCT DefintionCode [108911000146107 Short Nutritional Questionnaire total score] -> [blank] |
| StrongKidsScore | NL-CM:4.28.3     | GewichtsverliesScore  | SKGewichtsverliesScoreCodelijst | oranje: minor change    | NL-CM:4.28.3     | GewichtsverliesScore  | SKGewichtsverliesScoreCodelijst | ZIB-932 | SNOMED CT DefintionCode concept aangepast | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefintionCode [blank] -> [4028003 StrongKidsScore GewichtsverliesScore]                | Medium         | SCT DefintionCode [4028003 StrongKidsScore GewichtsverliesScore] -> [blank]                |
| StrongKidsScore | NL-CM:4.28.4     | ZiekteBeeldScore      | SKZiektebeeldScoreCodelijst     | oranje: minor change    | NL-CM:4.28.4     | ZiekteBeeldScore      | SKZiektebeeldScoreCodelijst     | ZIB-932 | SNOMED CT DefintionCode concept aangepast | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefintionCode [blank] -> [4028004 StrongKidsScore ZiekteBeeldScore]                    | Medium         | SCT DefintionCode  [4028005 StrongKidsScore VoedingsScore] -> [blank]                      |
| StrongKidsScore | NL-CM:4.28.5     | VoedingsScore         | SKVoedingsScoreCodelijst        | oranje: minor change    | NL-CM:4.28.5     | VoedingsScore         | SKVoedingsScoreCodelijst        | ZIB-932 | SNOMED CT DefintionCode concept aangepast | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefintionCode [blank] -> [4028005 StrongKidsScore VoedingsScore]                       | Medium         | SCT DefintionCode [4028005 StrongKidsScore VoedingsScore] -> [blank]                       |
| StrongKidsScore | NL-CM:4.28.6     | ScoreDatumTijd        |                                 | groen: geen wijzigingen | NL-CM:4.28.6     | ScoreDatumTijd        |                                 |         |                                           |                                    |               |                                                                                            |                |                                                                                            |
| StrongKidsScore | NL-CM:4.28.7     | Toelichting           |                                 | groen: geen wijzigingen | NL-CM:4.28.7     | Toelichting           |                                 |         |                                           |                                    |               |                                                                                            |                |                                                                                            |
| StrongKidsScore | NL-CM:4.28.8     | VoedingstoestandScore | SKVoedingstoestandCodelijst     | oranje: minor change    | NL-CM:4.28.8     | VoedingstoestandScore | SKVoedingstoestandCodelijst     | ZIB-932 | SNOMED CT DefintionCode concept aangepast | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefintionCode [blank] -> [4028008 StrongKidsScore VoedingstoestandScore]               | Medium         | SCT DefintionCode [4028008 StrongKidsScore VoedingstoestandScore] -> [blank]               |

