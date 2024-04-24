# Stoma
## File formats

The translation specs are available as: 
[CSV](../csv/Stoma.csv) [JSON](../json/Stoma.json) [XML](../xml/Stoma.xml)



[Stoma-v3.2(2017NL)](https://zibs.nl/wiki/Stoma-v3.2(2017NL))

[Stoma-v3.3(2020NL)](https://zibs.nl/wiki/Stoma-v3.3(2020NL))









## Changes

| ConceptID_2017   | ConceptName_2017   | Change               | TypeChange         | Impact_heen   | TRANSLATIE_spec_heen                                                                                                                                             | Impact_terug   | TRANSLATIE_spec_terug                                           | Omschrijving                                            |
|:-----------------|:-------------------|:---------------------|:-------------------|:--------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------|:---------------|:----------------------------------------------------------------|:--------------------------------------------------------|
| NL-CM:5.2.4      | AnatomischeLocatie | oranje: minor change | CHANGE TO SUB HCIM | Medium        | codelist [StomaAnatomischeLocatieCodelijst]->[LocatieCodelijst (http://decor.nictiz.nl/fhir/ValueSet/2.16.840.1.113883.2.4.3.11.60.40.2.20.7.1--20200901000000)] | Medium         | codelist [LocatieCodelijst]->[StomaAnatomischeLocatieCodelijst] | nieuwe verwijzing naar sub-bouwsteen anatomischeLocatie |
| NL-CM:5.2.8      | Lateraliteit       | oranje: minor change | CHANGE TO SUB HCIM | Medium        | codelist [StomaLateraliteitCodelijst]->[LateraliteitCodelijst (http://decor.nictiz.nl/fhir/ValueSet/2.16.840.1.113883.2.4.3.11.60.40.2.20.7.2--20200901000000)]  | Medium         | codelist [LateraliteitCodelijst]->[StomaLateraliteitCodelijst]  | nieuwe verwijzing naar sub-bouwsteen anatomischeLocatie |

## Mapping

| ZibName   | ConceptID_2017   | ConceptName_2017                  | Codelists_2017                   | Change                  | ConceptID_2020   | ConceptName_2020                               | Codelists_2020        | Bits     | Omschrijving                                            | TypeChange         | Impact_heen   | TRANSLATIE_spec_heen                                                                                                                                             | Impact_terug   | TRANSLATIE_spec_terug                                           |
|:----------|:-----------------|:----------------------------------|:---------------------------------|:------------------------|:-----------------|:-----------------------------------------------|:----------------------|:---------|:--------------------------------------------------------|:-------------------|:--------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------|:---------------|:----------------------------------------------------------------|
| Stoma     | NL-CM:5.2.1      | Stoma                             |                                  | groen: geen wijzigingen | NL-CM:5.2.1      | Stoma                                          |                       |          |                                                         |                    |               |                                                                                                                                                                  |                |                                                                 |
| Stoma     | NL-CM:5.2.2      | StomaType                         | StomaTypeCodelijst               | groen: geen wijzigingen | NL-CM:5.2.2      | StomaType                                      | StomaTypeCodelijst    |          |                                                         |                    |               |                                                                                                                                                                  |                |                                                                 |
| Stoma     | NL-CM:5.2.3      | StomaMateriaal::MedischHulpmiddel |                                  | groen: geen wijzigingen | NL-CM:5.2.3      | StomaMateriaal::MedischHulpmiddel              |                       |          |                                                         |                    |               |                                                                                                                                                                  |                |                                                                 |
| Stoma     | NL-CM:5.2.4      | AnatomischeLocatie                | StomaAnatomischeLocatieCodelijst | oranje: minor change    | NL-CM:5.1.14     | ProbleemAnatomischeLocatie::AnatomischeLocatie | LocatieCodelijst      | ZIB-1116 | nieuwe verwijzing naar sub-bouwsteen anatomischeLocatie | CHANGE TO SUB HCIM | Medium        | codelist [StomaAnatomischeLocatieCodelijst]->[LocatieCodelijst (http://decor.nictiz.nl/fhir/ValueSet/2.16.840.1.113883.2.4.3.11.60.40.2.20.7.1--20200901000000)] | Medium         | codelist [LocatieCodelijst]->[StomaAnatomischeLocatieCodelijst] |
| Stoma     | NL-CM:5.2.5      | AanlegDatum                       |                                  | groen: geen wijzigingen | NL-CM:5.2.5      | AanlegDatum                                    |                       |          |                                                         |                    |               |                                                                                                                                                                  |                |                                                                 |
| Stoma     | NL-CM:5.2.7      | Toelichting                       |                                  | groen: geen wijzigingen | NL-CM:5.2.7      | Toelichting                                    |                       |          |                                                         |                    |               |                                                                                                                                                                  |                |                                                                 |
| Stoma     | NL-CM:5.2.8      | Lateraliteit                      | StomaLateraliteitCodelijst       | oranje: minor change    | NL-CM:5.1.14     | ProbleemAnatomischeLocatie::AnatomischeLocatie | LateraliteitCodelijst | ZIB-1116 | nieuwe verwijzing naar sub-bouwsteen anatomischeLocatie | CHANGE TO SUB HCIM | Medium        | codelist [StomaLateraliteitCodelijst]->[LateraliteitCodelijst (http://decor.nictiz.nl/fhir/ValueSet/2.16.840.1.113883.2.4.3.11.60.40.2.20.7.2--20200901000000)]  | Medium         | codelist [LateraliteitCodelijst]->[StomaLateraliteitCodelijst]  |

