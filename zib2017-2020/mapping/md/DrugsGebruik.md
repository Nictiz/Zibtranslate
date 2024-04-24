# DrugsGebruik
## File formats

The translation specs are available as: 
[CSV](../csv/DrugsGebruik.csv) [JSON](../json/DrugsGebruik.json) [XML](../xml/DrugsGebruik.xml)



[DrugsGebruik-v3.2(2017NL)](https://zibs.nl/wiki/DrugsGebruik-v3.2(2017NL))

[DrugsGebruik-v3.3(2020NL)](https://zibs.nl/wiki/DrugsGebruik-v3.3(2020NL))









## Changes

| ConceptID_2017   | ConceptName_2017   | Change               | TypeChange                         | Impact_heen   | TRANSLATIE_spec_heen                                                         | Impact_terug   | TRANSLATIE_spec_terug                                                        | Omschrijving                                                                      |
|:-----------------|:-------------------|:---------------------|:-----------------------------------|:--------------|:-----------------------------------------------------------------------------|:---------------|:-----------------------------------------------------------------------------|:----------------------------------------------------------------------------------|
| NL-CM:7.4.1      | DrugsGebruik       | oranje: minor change | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefintionCode  [blank] -> [228366006 Bevinding betreffende drugsgebruik] | Medium         | SCT DefintionCode  [228366006 Bevinding betreffende drugsgebruik] -> [blank] | SNOMED CT DefintionCode concept aangepast                                         |
| NL-CM:7.4.3      | DrugsGebruikStatus | oranje: minor change | VALUESET CHANGES                   | Low           | valuesets 2017 -> valueset 2020 regel                                        | Medium         | valuesets 2017 <- valueset 2020 regel                                        | SNOMED CT Code voor huidig druggebruiker aangepast in DrugGebruikStatusCodelijst. |

## Mapping

| ZibName      | ConceptID_2017   | ConceptName_2017         | Codelists_2017                    | Change                  | ConceptID_2020   | ConceptName_2020         | Codelists_2020                    | Bits     | Omschrijving                                                                      | TypeChange                         | Impact_heen   | TRANSLATIE_spec_heen                                                         | Impact_terug   | TRANSLATIE_spec_terug                                                        |
|:-------------|:-----------------|:-------------------------|:----------------------------------|:------------------------|:-----------------|:-------------------------|:----------------------------------|:---------|:----------------------------------------------------------------------------------|:-----------------------------------|:--------------|:-----------------------------------------------------------------------------|:---------------|:-----------------------------------------------------------------------------|
| DrugsGebruik | NL-CM:7.4.1      | DrugsGebruik             |                                   | oranje: minor change    | NL-CM:7.4.1      | DrugsGebruik             |                                   | ZIB-1181 | SNOMED CT DefintionCode concept aangepast                                         | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefintionCode  [blank] -> [228366006 Bevinding betreffende drugsgebruik] | Medium         | SCT DefintionCode  [228366006 Bevinding betreffende drugsgebruik] -> [blank] |
| DrugsGebruik | NL-CM:7.4.2      | DrugsOfGeneesmiddelSoort | DrugsOfGeneesmiddelSoortCodelijst | groen: geen wijzigingen | NL-CM:7.4.2      | DrugsOfGeneesmiddelSoort | DrugsOfGeneesmiddelSoortCodelijst |          |                                                                                   |                                    |               |                                                                              |                |                                                                              |
| DrugsGebruik | NL-CM:7.4.3      | DrugsGebruikStatus       | DrugsGebruikStatusCodelijst       | oranje: minor change    | NL-CM:7.4.3      | DrugsGebruikStatus       | DrugsGebruikStatusCodelijst       | ZIB-936  | SNOMED CT Code voor huidig druggebruiker aangepast in DrugGebruikStatusCodelijst. | VALUESET CHANGES                   | Low           | valuesets 2017 -> valueset 2020 regel                                        | Medium         | valuesets 2017 <- valueset 2020 regel                                        |
| DrugsGebruik | NL-CM:7.4.4      | Toedieningsweg           | ToedieningswegCodelijst           | groen: geen wijzigingen | NL-CM:7.4.4      | Toedieningsweg           | ToedieningswegCodelijst           |          |                                                                                   |                                    |               |                                                                              |                |                                                                              |
| DrugsGebruik | NL-CM:7.4.5      | WaarnemingGebruik        |                                   | groen: geen wijzigingen | NL-CM:7.4.5      | WaarnemingGebruik        |                                   |          |                                                                                   |                                    |               |                                                                              |                |                                                                              |
| DrugsGebruik | NL-CM:7.4.6      | StartDatum               |                                   | groen: geen wijzigingen | NL-CM:7.4.6      | StartDatum               |                                   |          |                                                                                   |                                    |               |                                                                              |                |                                                                              |
| DrugsGebruik | NL-CM:7.4.7      | StopDatum                |                                   | groen: geen wijzigingen | NL-CM:7.4.7      | StopDatum                |                                   |          |                                                                                   |                                    |               |                                                                              |                |                                                                              |
| DrugsGebruik | NL-CM:7.4.8      | Hoeveelheid              |                                   | groen: geen wijzigingen | NL-CM:7.4.8      | Hoeveelheid              |                                   |          |                                                                                   |                                    |               |                                                                              |                |                                                                              |
| DrugsGebruik | NL-CM:7.4.9      | Toelichting              |                                   | groen: geen wijzigingen | NL-CM:7.4.9      | Toelichting              |                                   |          |                                                                                   |                                    |               |                                                                              |                |                                                                              |

