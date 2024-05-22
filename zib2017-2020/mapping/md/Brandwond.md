# Brandwond
## File formats

The translation specs are available as: 
[CSV](../csv/Brandwond.csv) [JSON](../json/Brandwond.json) [XML](../xml/Brandwond.xml)



[Brandwond-v3.2(2017NL)](https://zibs.nl/wiki/Brandwond-v3.2(2017NL))

[Brandwond-v3.4(2020NL)](https://zibs.nl/wiki/Brandwond-v3.4(2020NL))









## Changes

| ConceptID_2017   | ConceptName_2017               | Change               | TypeChange                    | Impact_heen   | TRANSLATIE_spec_heen   | Impact_terug   | TRANSLATIE_spec_terug                                     | Omschrijving                                                                                       |
|:-----------------|:-------------------------------|:---------------------|:------------------------------|:--------------|:-----------------------|:---------------|:----------------------------------------------------------|:---------------------------------------------------------------------------------------------------|
| NL-CM:19.4.4     | AnatomischeLocatie             | oranje: minor change | CHANGE TO SUB HCIM            | Medium        | source -> target       | Medium         | source -> target                                          | nieuwe verwijzing naar sub-bouwsteen anatomischeLocatie                                            |
| NL-CM:19.4.9     | BrandwondSoort                 | rood: major change   | OTHER INFORMATIONMODEL CHANGE | Low           | source -> target       | Low            | source -> target                                          | erratum:Het element BrandwondSoort per ongeluk verwijderd in publicatie 2020 en is weer toegevoegd |
| NL-CM:19.4.10    | Lateraliteit                   | oranje: minor change | CHANGE TO SUB HCIM            | Medium        | source -> target       | Medium         | source -> target                                          | nieuwe verwijzing naar sub-bouwsteen anatomischeLocatie                                            |
| NL-CM:19.4.11    | **concept toegevoegd in 2020** | rood: major change   | CONCEPT ADDITION              | Low           |                        | High           | IF source <> [blank] THEN source -> target=[non-zib item] | Concept Wondfoto toegevoegd aan zib brandwond                                                      |

## Mapping

| ZibName   | ConceptID_2017   | ConceptName_2017               | Codelists_2017                       | Change                  | ConceptID_2020   | ConceptName_2020                  | Codelists_2020          | Bits     | Omschrijving                                                                                       | TypeChange                    | Impact_heen   | TRANSLATIE_spec_heen   | Impact_terug   | TRANSLATIE_spec_terug                                     |
|:----------|:-----------------|:-------------------------------|:-------------------------------------|:------------------------|:-----------------|:----------------------------------|:------------------------|:---------|:---------------------------------------------------------------------------------------------------|:------------------------------|:--------------|:-----------------------|:---------------|:----------------------------------------------------------|
| Brandwond | NL-CM:19.4.1     | Brandwond                      |                                      | groen: geen wijzigingen | NL-CM:19.4.1     | Brandwond                         |                         |          |                                                                                                    |                               |               |                        |                |                                                           |
| Brandwond | NL-CM:19.4.2     | Dieptegraad                    | DieptegraadCodelijst                 | groen: geen wijzigingen | NL-CM:19.4.2     | Dieptegraad                       | DieptegraadCodelijst    |          |                                                                                                    |                               |               |                        |                |                                                           |
| Brandwond | NL-CM:19.4.3     | OntstaansDatum                 |                                      | groen: geen wijzigingen | NL-CM:5.2.1      | Stoma                             |                         |          |                                                                                                    |                               |               |                        |                |                                                           |
| Brandwond | NL-CM:19.4.4     | AnatomischeLocatie             | BrandwondAnatomischeLocatieCodelijst | oranje: minor change    | NL-CM:19.1.14    | Locatie                           | LocatieCodelijst        | ZIB-1116 | nieuwe verwijzing naar sub-bouwsteen anatomischeLocatie                                            | CHANGE TO SUB HCIM            | Medium        | source -> target       | Medium         | source -> target                                          |
| Brandwond | NL-CM:19.4.5     | Toelichting                    |                                      | groen: geen wijzigingen | NL-CM:19.4.5     | Toelichting                       |                         |          |                                                                                                    |                               |               |                        |                |                                                           |
| Brandwond | NL-CM:19.4.7     | Uitgebreidheid                 |                                      | groen: geen wijzigingen | NL-CM:5.2.3      | StomaMateriaal::MedischHulpmiddel |                         |          |                                                                                                    |                               |               |                        |                |                                                           |
| Brandwond | NL-CM:19.4.8     | DatumLaatsteVerbandwissel      |                                      | groen: geen wijzigingen | NL-CM:19.4.8     | DatumLaatsteVerbandwissel         |                         |          |                                                                                                    |                               |               |                        |                |                                                           |
| Brandwond | NL-CM:19.4.9     | BrandwondSoort                 | BrandwondSoortCodelijst              | rood: major change      | NL-CM:19.4.9     | BrandwondSoort                    | BrandwondSoortCodelijst | ZIB-1296 | erratum:Het element BrandwondSoort per ongeluk verwijderd in publicatie 2020 en is weer toegevoegd | OTHER INFORMATIONMODEL CHANGE | Low           | source -> target       | Low            | source -> target                                          |
| Brandwond | NL-CM:19.4.10    | Lateraliteit                   | BrandwondLateraliteitCodelijst       | oranje: minor change    | NL-CM:19.1.14    | Lateraliteit                      | LateraliteitCodelijst   | ZIB-1116 | nieuwe verwijzing naar sub-bouwsteen anatomischeLocatie                                            | CHANGE TO SUB HCIM            | Medium        | source -> target       | Medium         | source -> target                                          |
| Brandwond | NL-CM:19.4.11    | **concept toegevoegd in 2020** |                                      | rood: major change      | NL-CM:19.4.11    | WondFoto                          |                         | ZIB-828  | Concept Wondfoto toegevoegd aan zib brandwond                                                      | CONCEPT ADDITION              | Low           |                        | High           | IF source <> [blank] THEN source -> target=[non-zib item] |

