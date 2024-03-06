# BurgerlijkeStaat
## File formats

The translation specs are available as: 
[CSV](../csv/BurgerlijkeStaat.csv) [JSON](../json/BurgerlijkeStaat.json) [XML](../xml/BurgerlijkeStaat.xml) [Excel](../excel/BurgerlijkeStaat.xlsx)



## Zib BurgerlijkeStaat

[BurgerlijkeStaat-v3.0(2017NL)](https://zibs.nl/wiki/BurgerlijkeStaat-v3.0(2017NL))

[BurgerlijkeStaat-v3.1(2020NL)](https://zibs.nl/wiki/BurgerlijkeStaat-v3.1(2020NL))







## Zib-level changes

| ConceptID_2017    | ConceptName_2017   | Change                | TypeChange          | Omschrijving                  |
|:------------------|:-------------------|:----------------------|:--------------------|:------------------------------|
| DCM::Instructions | Instructions       | geel: patch wijziging | SIMPLE PATCH CHANGE | Tekst instructions gewijzigd. |

## Changes

| ConceptID_2017   | ConceptName_2017   | Change               | TypeChange       | Impact_heen   | TRANSLATIE_spec_heen                  | Impact_terug   | TRANSLATIE_spec_terug                 | Omschrijving                                                                     |
|:-----------------|:-------------------|:---------------------|:-----------------|:--------------|:--------------------------------------|:---------------|:--------------------------------------|:---------------------------------------------------------------------------------|
| NL-CM:7.9.2      | BurgerlijkeStaat   | oranje: minor change | VALUESET CHANGES | Low           | valuesets 2017 -> valueset 2020 regel | Medium         | valuesets 2017 <- valueset 2020 regel | Unmarried/ongehuwd toegevoegd aan codelijst. Never married op discouraged gezet. |

## Mapping

| ConceptID_2017   | ConceptName_2017   | Codelists_2017            | Change                  | ConceptID_2020   | ConceptName_2020   | Codelists_2020            | Bits    | Omschrijving                                                                     | TypeChange       | Impact_heen   | TRANSLATIE_spec_heen                  | Impact_terug   | TRANSLATIE_spec_terug                 |
|:-----------------|:-------------------|:--------------------------|:------------------------|:-----------------|:-------------------|:--------------------------|:--------|:---------------------------------------------------------------------------------|:-----------------|:--------------|:--------------------------------------|:---------------|:--------------------------------------|
| NL-CM:7.9.1      | BurgerlijkeStaatRC |                           | groen: geen wijzigingen | NL-CM:7.9.1      | BurgerlijkeStaatRC |                           |         |                                                                                  | NO CHANGE        |               |                                       |                |                                       |
| NL-CM:7.9.2      | BurgerlijkeStaat   | BurgerlijkeStaatCodelijst | oranje: minor change    | NL-CM:7.9.2      | BurgerlijkeStaat   | BurgerlijkeStaatCodelijst | ZIB-735 | Unmarried/ongehuwd toegevoegd aan codelijst. Never married op discouraged gezet. | VALUESET CHANGES | Low           | valuesets 2017 -> valueset 2020 regel | Medium         | valuesets 2017 <- valueset 2020 regel |

