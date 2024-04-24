# Huidaandoening
## File formats

The translation specs are available as: 
[CSV](../csv/Huidaandoening.csv) [JSON](../json/Huidaandoening.json) [XML](../xml/Huidaandoening.xml)



[Huidaandoening-v3.2(2017NL)](https://zibs.nl/wiki/Huidaandoening-v3.2(2017NL))

[Huidaandoening-v3.3(2020NL)](https://zibs.nl/wiki/Huidaandoening-v3.3(2020NL))









## Changes

| ConceptID_2017   | ConceptName_2017   | Change               | TypeChange         | Impact_heen   | TRANSLATIE_spec_heen                                                                                                                                                     | Impact_terug   | TRANSLATIE_spec_terug                                                    | Omschrijving                                            |
|:-----------------|:-------------------|:---------------------|:-------------------|:--------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:---------------|:-------------------------------------------------------------------------|:--------------------------------------------------------|
| NL-CM:19.3.4     | AnatomischeLocatie | oranje: minor change | CHANGE TO SUB HCIM | Medium        | codelist [HuidaandoeningAnatomischeLocatieCodelijst]->[LocatieCodelijst]                                                                                                 | Medium         | codelist [LocatieCodelijst]->[HuidaandoeningAnatomischeLocatieCodelijst] | nieuwe verwijzing naar sub-bouwsteen anatomischeLocatie |
| NL-CM:19.3.8     | Lateraliteit       | oranje: minor change | CHANGE TO SUB HCIM | Medium        | codelist [HuidaandoeningLateraliteitCodelijst]->[LateraliteitCodelijst (http://decor.nictiz.nl/fhir/ValueSet/2.16.840.1.113883.2.4.3.11.60.40.2.20.7.2--20200901000000)] | Medium         | codelist [LateraliteitCodelijst]->[HuidaandoeningLateraliteitCodelijst]  | nieuwe verwijzing naar sub-bouwsteen anatomischeLocatie |

## Mapping

| ZibName        | ConceptID_2017   | ConceptName_2017   | Codelists_2017                            | Change                  | ConceptID_2020   | ConceptName_2020   | Codelists_2020           | Bits     | Omschrijving                                            | TypeChange         | Impact_heen   | TRANSLATIE_spec_heen                                                                                                                                                     | Impact_terug   | TRANSLATIE_spec_terug                                                    |
|:---------------|:-----------------|:-------------------|:------------------------------------------|:------------------------|:-----------------|:-------------------|:-------------------------|:---------|:--------------------------------------------------------|:-------------------|:--------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:---------------|:-------------------------------------------------------------------------|
| Huidaandoening | NL-CM:19.3.1     | Huidaandoening     |                                           | groen: geen wijzigingen | NL-CM:19.3.1     | Huidaandoening     |                          |          |                                                         |                    |               |                                                                                                                                                                          |                |                                                                          |
| Huidaandoening | NL-CM:19.3.2     | SoortAandoening    | SoortAandoeningCodelijst                  | groen: geen wijzigingen | NL-CM:19.3.2     | SoortAandoening    | SoortAandoeningCodelijst |          |                                                         |                    |               |                                                                                                                                                                          |                |                                                                          |
| Huidaandoening | NL-CM:19.3.3     | OntstaansDatum     |                                           | groen: geen wijzigingen | NL-CM:19.3.3     | OntstaansDatum     |                          |          |                                                         |                    |               |                                                                                                                                                                          |                |                                                                          |
| Huidaandoening | NL-CM:19.3.4     | AnatomischeLocatie | HuidaandoeningAnatomischeLocatieCodelijst | oranje: minor change    | NL-CM:19.1.14    | Locatie            | LocatieCodelijst         | ZIB-1116 | nieuwe verwijzing naar sub-bouwsteen anatomischeLocatie | CHANGE TO SUB HCIM | Medium        | codelist [HuidaandoeningAnatomischeLocatieCodelijst]->[LocatieCodelijst]                                                                                                 | Medium         | codelist [LocatieCodelijst]->[HuidaandoeningAnatomischeLocatieCodelijst] |
| Huidaandoening | NL-CM:19.3.6     | Toelichting        |                                           | groen: geen wijzigingen | NL-CM:19.3.6     | Toelichting        |                          |          |                                                         |                    |               |                                                                                                                                                                          |                |                                                                          |
| Huidaandoening | NL-CM:19.3.7     | Oorzaak::Probleem  |                                           | groen: geen wijzigingen | NL-CM:19.3.7     | Oorzaak::Probleem  |                          |          |                                                         |                    |               |                                                                                                                                                                          |                |                                                                          |
| Huidaandoening | NL-CM:19.3.8     | Lateraliteit       | HuidaandoeningLateraliteitCodelijst       | oranje: minor change    | NL-CM:19.1.14    | Lateraliteit       | LateraliteitCodelijst    | ZIB-1116 | nieuwe verwijzing naar sub-bouwsteen anatomischeLocatie | CHANGE TO SUB HCIM | Medium        | codelist [HuidaandoeningLateraliteitCodelijst]->[LateraliteitCodelijst (http://decor.nictiz.nl/fhir/ValueSet/2.16.840.1.113883.2.4.3.11.60.40.2.20.7.2--20200901000000)] | Medium         | codelist [LateraliteitCodelijst]->[HuidaandoeningLateraliteitCodelijst]  |

