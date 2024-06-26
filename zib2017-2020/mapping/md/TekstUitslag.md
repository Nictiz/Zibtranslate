# TekstUitslag
## File formats

The translation specs are available as: 
[CSV](../csv/TekstUitslag.csv) [JSON](../json/TekstUitslag.json) [XML](../xml/TekstUitslag.xml)



[TekstUitslag-v4.1(2017NL)](https://zibs.nl/wiki/TekstUitslag-v4.1(2017NL))

[TekstUitslag-v4.4(2020NL)](https://zibs.nl/wiki/TekstUitslag-v4.4(2020NL))









## Changes

| ConceptID_2017   | ConceptName_2017               | Change                | TypeChange                         | Impact_heen   | TRANSLATIE_spec_heen                                               | Impact_terug   | TRANSLATIE_spec_terug                                               | Omschrijving                                                |
|:-----------------|:-------------------------------|:----------------------|:-----------------------------------|:--------------|:-------------------------------------------------------------------|:---------------|:--------------------------------------------------------------------|:------------------------------------------------------------|
| NL-CM:13.2.1     | TekstUitslag                   | oranje: minor change  | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefintionCode [blank] -> [371525003 Clinical procedure report] | Medium         | SCT DefintionCode  [371525003 Clinical procedure report] -> [blank] | SNOMED CT DefintionCode concept aangepast                   |
| NL-CM:13.2.2     | TekstResultaat                 | geel: patch wijziging | SIMPLE PATCH CHANGE                | Low           |                                                                    | Low            |                                                                     | Aanpassing spelfout in defintie concept TekstResultaat.     |
| NL-CM:13.2.2     | TekstResultaat                 | oranje: minor change  | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefintionCode [blank] -> [423100009 Results section]           | Medium         | SCT DefintionCode [423100009 Results section] -> [blank]            | SNOMED CT DefintionCode concept aangepast                   |
| NL-CM:13.2.3     | TekstUitslagDatumTijd          | geel: patch wijziging | SIMPLE PATCH CHANGE                | Low           |                                                                    | Low            |                                                                     | Tekstwijzging defintie concept                              |
| NL-CM:13.2.3     | TekstUitslagDatumTijd          | oranje: minor change  | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefintionCode [blank] -> [399651003 Date of report]            | Medium         | SCT DefintionCode [399651003 Date of report] -> [blank]             | SNOMED CT DefintionCode concept aangepast                   |
| NL-CM:13.2.4     | TekstUitslagType               | oranje: minor change  | VALUESET CHANGES                   | Low           | existing valueset [valuesetname] changed in [baseline 2020]        | Medium         | existing valueset [valuesetname] changed in [baseline 2020]         | SNOMED code PET CT aan TekstuitslagTypeCodelijst toegevoegd |
| NL-CM:13.2.5     | Verrichting                    | oranje: minor change  | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefintionCode [363714003 Interprets] -> [71388002 Verrichting] | Medium         | SCT DefintionCode  [71388002 Verrichting] -> [363714003 Interprets] | SNOMED CT DefintionCode concept aangepast                   |
| NL-CM:13.2.6     | TekstUitslagStatus             | oranje: minor change  | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefintionCode [blank] -> [308552006 Status van verslag]        | Medium         | SCT DefintionCode [308552006 Status van verslag] -> [blank]         | SNOMED CT DefintionCode concept aangepast                   |
| NL-CM:13.2.7     | **concept toegevoegd in 2020** | rood: major change    | CONCEPT ADDITION                   | Low           |                                                                    | High           | IF source <> [blank] THEN source -> target=[non-zib item]           | Element toegevoegd om naar beeldmateriaal te verwijzen.     |

## Mapping

| ZibName      | ConceptID_2017   | ConceptName_2017               | Codelists_2017            | Change                | ConceptID_2020   | ConceptName_2020      | Codelists_2020            | Bits     | Omschrijving                                                | TypeChange                         | Impact_heen   | TRANSLATIE_spec_heen                                               | Impact_terug   | TRANSLATIE_spec_terug                                               |
|:-------------|:-----------------|:-------------------------------|:--------------------------|:----------------------|:-----------------|:----------------------|:--------------------------|:---------|:------------------------------------------------------------|:-----------------------------------|:--------------|:-------------------------------------------------------------------|:---------------|:--------------------------------------------------------------------|
| TekstUitslag | NL-CM:13.2.1     | TekstUitslag                   |                           | oranje: minor change  | NL-CM:13.2.1     | TekstUitslag          |                           | ZIB-1187 | SNOMED CT DefintionCode concept aangepast                   | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefintionCode [blank] -> [371525003 Clinical procedure report] | Medium         | SCT DefintionCode  [371525003 Clinical procedure report] -> [blank] |
| TekstUitslag | NL-CM:13.2.2     | TekstResultaat                 |                           | geel: patch wijziging | NL-CM:13.2.2     | TekstResultaat        |                           | ZIB-955  | Aanpassing spelfout in defintie concept TekstResultaat.     | SIMPLE PATCH CHANGE                | Low           |                                                                    | Low            |                                                                     |
| TekstUitslag | NL-CM:13.2.2     | TekstResultaat                 |                           | oranje: minor change  | NL-CM:13.2.2     | TekstResultaat        |                           | ZIB-1187 | SNOMED CT DefintionCode concept aangepast                   | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefintionCode [blank] -> [423100009 Results section]           | Medium         | SCT DefintionCode [423100009 Results section] -> [blank]            |
| TekstUitslag | NL-CM:13.2.3     | TekstUitslagDatumTijd          |                           | geel: patch wijziging | NL-CM:13.2.3     | TekstUitslagDatumTijd |                           | ZIB-955  | Tekstwijzging defintie concept                              | SIMPLE PATCH CHANGE                | Low           |                                                                    | Low            |                                                                     |
| TekstUitslag | NL-CM:13.2.3     | TekstUitslagDatumTijd          |                           | oranje: minor change  | NL-CM:13.2.3     | TekstUitslagDatumTijd |                           | ZIB-1187 | SNOMED CT DefintionCode concept aangepast                   | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefintionCode [blank] -> [399651003 Date of report]            | Medium         | SCT DefintionCode [399651003 Date of report] -> [blank]             |
| TekstUitslag | NL-CM:13.2.4     | TekstUitslagType               | TekstUitslagTypeCodelijst | oranje: minor change  | NL-CM:13.2.4     | TekstUitslagType      | TekstUitslagTypeCodelijst | ZIB-630  | SNOMED code PET CT aan TekstuitslagTypeCodelijst toegevoegd | VALUESET CHANGES                   | Low           | existing valueset [valuesetname] changed in [baseline 2020]        | Medium         | existing valueset [valuesetname] changed in [baseline 2020]         |
| TekstUitslag | NL-CM:13.2.5     | Verrichting                    |                           | oranje: minor change  | NL-CM:13.2.5     | Verrichting           |                           | ZIB-1187 | SNOMED CT DefintionCode concept aangepast                   | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefintionCode [363714003 Interprets] -> [71388002 Verrichting] | Medium         | SCT DefintionCode  [71388002 Verrichting] -> [363714003 Interprets] |
| TekstUitslag | NL-CM:13.2.6     | TekstUitslagStatus             | TekstStatusCodelijst      | oranje: minor change  | NL-CM:13.2.6     | TekstUitslagStatus    | TekstStatusCodelijst      | ZIB-1187 | SNOMED CT DefintionCode concept aangepast                   | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | SCT DefintionCode [blank] -> [308552006 Status van verslag]        | Medium         | SCT DefintionCode [308552006 Status van verslag] -> [blank]         |
| TekstUitslag | NL-CM:13.2.7     | **concept toegevoegd in 2020** |                           | rood: major change    | NL-CM:13.2.7     | VisueelResultaat      |                           | ZIB-631  | Element toegevoegd om naar beeldmateriaal te verwijzen.     | CONCEPT ADDITION                   | Low           |                                                                    | High           | IF source <> [blank] THEN source -> target=[non-zib item]           |

