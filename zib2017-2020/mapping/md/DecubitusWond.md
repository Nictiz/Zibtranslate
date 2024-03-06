# DecubitusWond
## File formats

The translation specs are available as: 
[CSV](../csv/DecubitusWond.csv) [JSON](../json/DecubitusWond.json) [XML](../xml/DecubitusWond.xml) [Excel](../excel/DecubitusWond.xlsx)



## Zib DecubitusWond

[DecubitusWond-v3.2(2017NL)](https://zibs.nl/wiki/DecubitusWond-v3.2(2017NL))

[DecubitusWond-v3.4(2020NL)](https://zibs.nl/wiki/DecubitusWond-v3.4(2020NL))









## Changes

| ConceptID_2017   | ConceptName_2017   | Change               | TypeChange         | Impact_heen   | TRANSLATIE_spec_heen                                                                                                                                                     | Impact_terug   | TRANSLATIE_spec_terug                                                                                                                                                    | Omschrijving                                            |
|:-----------------|:-------------------|:---------------------|:-------------------|:--------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:---------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:--------------------------------------------------------|
| NL-CM:19.1.4     | AnatomischeLocatie | oranje: minor change | CHANGE TO SUB HCIM | Medium        | codelist [DecubitusWondAnatomischeLocatieCodelijst]->[LocatieCodelijst (http://decor.nictiz.nl/fhir/ValueSet/2.16.840.1.113883.2.4.3.11.60.40.2.20.7.1--20200901000000)] | Medium         | codelist [LocatieCodelijst (http://decor.nictiz.nl/fhir/ValueSet/2.16.840.1.113883.2.4.3.11.60.40.2.20.7.1--20200901000000)]->[DecubitusWondAnatomischeLocatieCodelijst] | nieuwe verwijzing naar sub-bouwsteen anatomischeLocatie |
| NL-CM:19.1.13    | Lateraliteit       | oranje: minor change | CHANGE TO SUB HCIM | Medium        | codelist [DecubitusWondLateraliteitCodelijst]->[LateraliteitCodelijst (http://decor.nictiz.nl/fhir/ValueSet/2.16.840.1.113883.2.4.3.11.60.40.2.20.7.2--20200901000000)]  | Medium         | codelist [LateraliteitCodelijst (http://decor.nictiz.nl/fhir/ValueSet/2.16.840.1.113883.2.4.3.11.60.40.2.20.7.2--20200901000000)]->[DecubitusWondLateraliteitCodelijst]  | nieuwe verwijzing naar sub-bouwsteen anatomischeLocatie |

## Mapping

| ConceptID_2017   | ConceptName_2017          | Codelists_2017                           | Change                  | ConceptID_2020   | ConceptName_2020          | Codelists_2020        | Bits     | Omschrijving                                            | TypeChange         | Impact_heen   | TRANSLATIE_spec_heen                                                                                                                                                     | Impact_terug   | TRANSLATIE_spec_terug                                                                                                                                                    |
|:-----------------|:--------------------------|:-----------------------------------------|:------------------------|:-----------------|:--------------------------|:----------------------|:---------|:--------------------------------------------------------|:-------------------|:--------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:---------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| NL-CM:19.1.1     | DecubitusWond             |                                          | groen: geen wijzigingen | NL-CM:19.1.1     | DecubitusWond             |                       |          |                                                         |                    |               |                                                                                                                                                                          |                |                                                                                                                                                                          |
| NL-CM:19.1.2     | DecubitusCategorie        |                                          | groen: geen wijzigingen | NL-CM:19.1.2     | DecubitusCategorie        |                       |          |                                                         |                    |               |                                                                                                                                                                          |                |                                                                                                                                                                          |
| NL-CM:19.1.3     | OntstaansDatum            |                                          | groen: geen wijzigingen | NL-CM:19.1.3     | OntstaansDatum            |                       |          |                                                         |                    |               |                                                                                                                                                                          |                |                                                                                                                                                                          |
| NL-CM:19.1.4     | AnatomischeLocatie        | DecubitusWondAnatomischeLocatieCodelijst | oranje: minor change    | NL-CM:19.1.14    | Locatie                   | LocatieCodelijst      | ZIB-1116 | nieuwe verwijzing naar sub-bouwsteen anatomischeLocatie | CHANGE TO SUB HCIM | Medium        | codelist [DecubitusWondAnatomischeLocatieCodelijst]->[LocatieCodelijst (http://decor.nictiz.nl/fhir/ValueSet/2.16.840.1.113883.2.4.3.11.60.40.2.20.7.1--20200901000000)] | Medium         | codelist [LocatieCodelijst (http://decor.nictiz.nl/fhir/ValueSet/2.16.840.1.113883.2.4.3.11.60.40.2.20.7.1--20200901000000)]->[DecubitusWondAnatomischeLocatieCodelijst] |
| NL-CM:19.1.5     | Toelichting               |                                          | groen: geen wijzigingen | NL-CM:19.1.5     | Toelichting               |                       |          |                                                         |                    |               |                                                                                                                                                                          |                |                                                                                                                                                                          |
| NL-CM:19.1.8     | DatumLaatsteVerbandwissel |                                          | groen: geen wijzigingen | NL-CM:19.1.8     | DatumLaatsteVerbandwissel |                       |          |                                                         |                    |               |                                                                                                                                                                          |                |                                                                                                                                                                          |
| NL-CM:19.1.9     | Wondlengte                |                                          | groen: geen wijzigingen | NL-CM:19.1.9     | Wondlengte                |                       |          |                                                         |                    |               |                                                                                                                                                                          |                |                                                                                                                                                                          |
| NL-CM:19.1.10    | Wondbreedte               |                                          | groen: geen wijzigingen | NL-CM:19.1.10    | Wondbreedte               |                       |          |                                                         |                    |               |                                                                                                                                                                          |                |                                                                                                                                                                          |
| NL-CM:19.1.11    | Wonddiepte                |                                          | groen: geen wijzigingen | NL-CM:19.1.11    | Wonddiepte                |                       |          |                                                         |                    |               |                                                                                                                                                                          |                |                                                                                                                                                                          |
| NL-CM:19.1.12    | WondFoto                  |                                          | groen: geen wijzigingen | NL-CM:19.1.12    | WondFoto                  |                       |          |                                                         |                    |               |                                                                                                                                                                          |                |                                                                                                                                                                          |
| NL-CM:19.1.13    | Lateraliteit              | DecubitusWondLateraliteitCodelijst       | oranje: minor change    | NL-CM:19.1.14    | Lateraliteit              | LateraliteitCodelijst | ZIB-1116 | nieuwe verwijzing naar sub-bouwsteen anatomischeLocatie | CHANGE TO SUB HCIM | Medium        | codelist [DecubitusWondLateraliteitCodelijst]->[LateraliteitCodelijst (http://decor.nictiz.nl/fhir/ValueSet/2.16.840.1.113883.2.4.3.11.60.40.2.20.7.2--20200901000000)]  | Medium         | codelist [LateraliteitCodelijst (http://decor.nictiz.nl/fhir/ValueSet/2.16.840.1.113883.2.4.3.11.60.40.2.20.7.2--20200901000000)]->[DecubitusWondLateraliteitCodelijst]  |
