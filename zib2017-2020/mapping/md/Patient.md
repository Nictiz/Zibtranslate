# Patient
## File formats

The translation specs are available as: 
[CSV](../csv/Patient.csv) [JSON](../json/Patient.json) [XML](../xml/Patient.xml) [Excel](../excel/Patient.xlsx)



## Zib Patient

[Patient-v3.1(2017NL)](https://zibs.nl/wiki/Patient-v3.1(2017NL))

[Patient-v3.2(2020NL)](https://zibs.nl/wiki/Patient-v3.2(2020NL))







## Zib-level changes

| ConceptID_2017    | ConceptName_2017   | Change                | TypeChange          | Omschrijving                                 |
|:------------------|:-------------------|:----------------------|:--------------------|:---------------------------------------------|
| DCM::EvidenceBase | Evidence Base      | geel: patch wijziging | SIMPLE PATCH CHANGE | Concept definitie en evidence base aangepast |
| DCM::Concept      | Concept            | geel: patch wijziging | SIMPLE PATCH CHANGE | Concept definitie en evidence base aangepast |

## Changes

| ConceptID_2017   | ConceptName_2017   | Change               | TypeChange                         | Impact_heen   | TRANSLATIE_spec_heen                             | Impact_terug   | TRANSLATIE_spec_terug                            | Omschrijving                                                         |
|:-----------------|:-------------------|:---------------------|:-----------------------------------|:--------------|:-------------------------------------------------|:---------------|:-------------------------------------------------|:---------------------------------------------------------------------|
| NL-CM:0.1.1      | Patient            | oranje: minor change | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefinitionCode [blank] -> [116154003 Patiënt] | Medium         | SCT DefinitionCode [116154003 Patiënt] -> [blank] | SNOMED CT DefinitionCode concept aangepast                            |
| NL-CM:0.1.6      | NameInformation    | oranje: minor change | CARDINALITY CHANGE                 | Low           | ONE TO ZERO-TO-ONE                               | Medium         | ZERO-TO-ONE TO ONE                               | Kardinaliteit van het element Naamgegevens gewijzigd van 1 naar 0..1 |
| NL-CM:0.1.9      | Gender             | oranje: minor change | CARDINALITY CHANGE                 | Low           | ONE TO ZERO-TO-ONE                               | Medium         | ZERO-TO-ONE TO ONE                               | Kardinaliteit Geslacht gewijzigd van 1 naar 0..1                     |
| NL-CM:0.1.10     | DateOfBirth        | oranje: minor change | CARDINALITY CHANGE                 | Low           | ONE TO ZERO-TO-ONE                               | Medium         | ZERO-TO-ONE TO ONE                               | Kardinaliteit Geboortedatum gewijzigd van 1 naar 0..1                |

## Mapping

| ConceptID_2017   | ConceptName_2017            | Codelists_2017               | Change                  | ConceptID_2020   | ConceptName_2020            | Codelists_2020               | Bits     | Omschrijving                                                         | TypeChange                         | Impact_heen   | TRANSLATIE_spec_heen                             | Impact_terug   | TRANSLATIE_spec_terug                            |
|:-----------------|:----------------------------|:-----------------------------|:------------------------|:-----------------|:----------------------------|:-----------------------------|:---------|:---------------------------------------------------------------------|:-----------------------------------|:--------------|:-------------------------------------------------|:---------------|:-------------------------------------------------|
| NL-CM:0.1.1      | Patient                     |                              | oranje: minor change    | NL-CM:0.1.1      | Patient                     |                              | ZIB-1189 | SNOMED CT DefinitionCode concept aangepast                            | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefinitionCode [blank] -> [116154003 Patiënt] | Medium         | SCT DefinitionCode [116154003 Patiënt] -> [blank] |
| NL-CM:0.1.4      | AddressInformation          | nl.zorg.part.Adresgegevens   | groen: geen wijzigingen | NL-CM:0.1.4      | AddressInformation          | nl.zorg.part.Adresgegevens   |          |                                                                      | NO CHANGE                          |               |                                                  |                |                                                  |
| NL-CM:0.1.5      | ContactInformation          | nl.zorg.part.Contactgegevens | groen: geen wijzigingen | NL-CM:0.1.5      | ContactInformation          | nl.zorg.part.Contactgegevens |          |                                                                      | NO CHANGE                          |               |                                                  |                |                                                  |
| NL-CM:0.1.6      | NameInformation             | nl.zorg.part.Naamgegevens    | oranje: minor change    | NL-CM:0.1.6      | NameInformation             |                              | ZIB-961  | Kardinaliteit van het element Naamgegevens gewijzigd van 1 naar 0..1 | CARDINALITY CHANGE                 | Low           | ONE TO ZERO-TO-ONE                               | Medium         | ZERO-TO-ONE TO ONE                               |
| NL-CM:0.1.7      | PatientIdentificationNumber |                              | groen: geen wijzigingen | NL-CM:0.1.7      | PatientIdentificationNumber |                              |          |                                                                      | NO CHANGE                          |               |                                                  |                |                                                  |
| NL-CM:0.1.9      | Gender                      |                              | oranje: minor change    | NL-CM:0.1.9      | Gender                      |                              | ZIB-1029 | Kardinaliteit Geslacht gewijzigd van 1 naar 0..1                     | CARDINALITY CHANGE                 | Low           | ONE TO ZERO-TO-ONE                               | Medium         | ZERO-TO-ONE TO ONE                               |
| NL-CM:0.1.10     | DateOfBirth                 |                              | oranje: minor change    | NL-CM:0.1.10     | DateOfBirth                 |                              | ZIB-1029 | Kardinaliteit Geboortedatum gewijzigd van 1 naar 0..1                | CARDINALITY CHANGE                 | Low           | ONE TO ZERO-TO-ONE                               | Medium         | ZERO-TO-ONE TO ONE                               |
| NL-CM:0.1.31     | MultipleBirthIndicator      |                              | groen: geen wijzigingen | NL-CM:0.1.31     | MultipleBirthIndicator      |                              |          |                                                                      | NO CHANGE                          |               |                                                  |                |                                                  |
| NL-CM:0.1.32     | OverlijdensIndicator        |                              | groen: geen wijzigingen | NL-CM:0.1.32     | OverlijdensIndicator        |                              |          |                                                                      | NO CHANGE                          |               |                                                  |                |                                                  |
| NL-CM:0.1.33     | DateOfDeath                 |                              | groen: geen wijzigingen | NL-CM:0.1.33     | DateOfDeath                 |                              |          |                                                                      | NO CHANGE                          |               |                                                  |                |                                                  |

