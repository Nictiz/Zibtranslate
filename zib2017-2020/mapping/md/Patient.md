# Patient
## File formats

The translation specs are available as: 
[CSV](../csv/Patient.csv) [JSON](../json/Patient.json) [XML](../xml/Patient.xml)



[Patient-v3.1(2017NL)](https://zibs.nl/wiki/Patient-v3.1(2017NL))

[Patient-v3.2(2020NL)](https://zibs.nl/wiki/Patient-v3.2(2020NL))







## Zib-level changes

| ConceptID_2017    | ConceptName_2017   | Change                | TypeChange          | Omschrijving                                 |
|:------------------|:-------------------|:----------------------|:--------------------|:---------------------------------------------|
| DCM::EvidenceBase | Evidence Base      | geel: patch wijziging | SIMPLE PATCH CHANGE | Concept definitie en evidence base aangepast |
| DCM::Concept      | Concept            | geel: patch wijziging | SIMPLE PATCH CHANGE | Concept definitie en evidence base aangepast |

## Changes

| ConceptID_2017   | ConceptName_2017   | Change               | TypeChange                         | Impact_heen   | TRANSLATIE_spec_heen                             | Impact_terug   | TRANSLATIE_spec_terug                                  | Omschrijving                                                         |
|:-----------------|:-------------------|:---------------------|:-----------------------------------|:--------------|:-------------------------------------------------|:---------------|:-------------------------------------------------------|:---------------------------------------------------------------------|
| NL-CM:0.1.1      | Patient            | oranje: minor change | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefintionCode [blank] -> [116154003 Patiënt] | Medium         | SCT DefintionCode [116154003 Patiënt] -> [blank]       | SNOMED CT DefintionCode concept aangepast                            |
| NL-CM:0.1.6      | NameInformation    | oranje: minor change | CARDINALITY CHANGES (1 to 0..1)    | Low           |                                                  | Medium         | ALS [aantal<>1] DAN [doe iets] ANDERS source -> target | Kardinaliteit van het element Naamgegevens gewijzigd van 1 naar 0..1 |
| NL-CM:0.1.9      | Gender             | oranje: minor change | CARDINALITY CHANGES (1 to 0..1)    | Low           |                                                  | Medium         | ALS [aantal<>1] DAN [doe iets] ANDERS source -> target | Kardinaliteit Geslacht gewijzigd van 1 naar 0..1                     |
| NL-CM:0.1.10     | DateOfBirth        | oranje: minor change | CARDINALITY CHANGES (1 to 0..1)    | Low           |                                                  | Medium         | ALS [aantal<>1] DAN [doe iets] ANDERS source -> target | Kardinaliteit Geboortedatum gewijzigd van 1 naar 0..1                |

## Mapping

| ZibName   | ConceptID_2017   | ConceptName_2017            | Codelists_2017               | Change                  | ConceptID_2020   | ConceptName_2020            | Codelists_2020               | Bits     | Omschrijving                                                         | TypeChange                         | Impact_heen   | TRANSLATIE_spec_heen                             | Impact_terug   | TRANSLATIE_spec_terug                                  |
|:----------|:-----------------|:----------------------------|:-----------------------------|:------------------------|:-----------------|:----------------------------|:-----------------------------|:---------|:---------------------------------------------------------------------|:-----------------------------------|:--------------|:-------------------------------------------------|:---------------|:-------------------------------------------------------|
| Patient   | NL-CM:0.1.1      | Patient                     |                              | oranje: minor change    | NL-CM:0.1.1      | Patient                     |                              | ZIB-1189 | SNOMED CT DefintionCode concept aangepast                            | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefintionCode [blank] -> [116154003 Patiënt] | Medium         | SCT DefintionCode [116154003 Patiënt] -> [blank]       |
| Patient   | NL-CM:0.1.4      | AddressInformation          | nl.zorg.part.Adresgegevens   | groen: geen wijzigingen | NL-CM:0.1.4      | AddressInformation          | nl.zorg.part.Adresgegevens   |          |                                                                      |                                    |               |                                                  |                |                                                        |
| Patient   | NL-CM:0.1.5      | ContactInformation          | nl.zorg.part.Contactgegevens | groen: geen wijzigingen | NL-CM:0.1.5      | ContactInformation          | nl.zorg.part.Contactgegevens |          |                                                                      |                                    |               |                                                  |                |                                                        |
| Patient   | NL-CM:0.1.6      | NameInformation             | nl.zorg.part.Naamgegevens    | oranje: minor change    | NL-CM:0.1.6      | NameInformation             |                              | ZIB-961  | Kardinaliteit van het element Naamgegevens gewijzigd van 1 naar 0..1 | CARDINALITY CHANGES (1 to 0..1)    | Low           |                                                  | Medium         | ALS [aantal<>1] DAN [doe iets] ANDERS source -> target |
| Patient   | NL-CM:0.1.7      | PatientIdentificationNumber |                              | groen: geen wijzigingen | NL-CM:0.1.7      | PatientIdentificationNumber |                              |          |                                                                      |                                    |               |                                                  |                |                                                        |
| Patient   | NL-CM:0.1.9      | Gender                      |                              | oranje: minor change    | NL-CM:0.1.9      | Gender                      |                              | ZIB-1029 | Kardinaliteit Geslacht gewijzigd van 1 naar 0..1                     | CARDINALITY CHANGES (1 to 0..1)    | Low           |                                                  | Medium         | ALS [aantal<>1] DAN [doe iets] ANDERS source -> target |
| Patient   | NL-CM:0.1.10     | DateOfBirth                 |                              | oranje: minor change    | NL-CM:0.1.10     | DateOfBirth                 |                              | ZIB-1029 | Kardinaliteit Geboortedatum gewijzigd van 1 naar 0..1                | CARDINALITY CHANGES (1 to 0..1)    | Low           |                                                  | Medium         | ALS [aantal<>1] DAN [doe iets] ANDERS source -> target |
| Patient   | NL-CM:0.1.31     | MultipleBirthIndicator      |                              | groen: geen wijzigingen | NL-CM:0.1.31     | MultipleBirthIndicator      |                              |          |                                                                      |                                    |               |                                                  |                |                                                        |
| Patient   | NL-CM:0.1.32     | OverlijdensIndicator        |                              | groen: geen wijzigingen | NL-CM:0.1.32     | OverlijdensIndicator        |                              |          |                                                                      |                                    |               |                                                  |                |                                                        |
| Patient   | NL-CM:0.1.33     | DateOfDeath                 |                              | groen: geen wijzigingen | NL-CM:0.1.33     | DateOfDeath                 |                              |          |                                                                      |                                    |               |                                                  |                |                                                        |

