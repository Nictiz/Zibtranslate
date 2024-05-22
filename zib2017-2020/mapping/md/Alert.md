# Alert
## File formats

The translation specs are available as: 
[CSV](../csv/Alert.csv) [JSON](../json/Alert.json) [XML](../xml/Alert.xml)



[Alert-v3.2(2017NL)](https://zibs.nl/wiki/Alert-v3.2(2017NL))

[Alert-v4.1(2020NL)](https://zibs.nl/wiki/Alert-v4.1(2020NL))



zie ZIB-1769 de leveranciers hebben gevraagd wordt om de contra-indicaties weer op te nemen in de zib Alert. Hiermee zou de zib MedicatieContraindicatie komen te vervallen in 2024 vanwege backward compatibility issues en de Thesaurus 40 uit de g-standaard weer worden toegevoegd aan AlertNaamCodelijst in publicatie 2024.

zie ook https://www.rivm.nl/antibioticaresistentie/nationale-aanpak-antibioticaresistentie/eenheid-van-taal-antibioticaresistentie

## Zib-level changes

| ConceptID_2017    | ConceptName_2017   | Change                | TypeChange          | Omschrijving                                                                                   |
|:------------------|:-------------------|:----------------------|:--------------------|:-----------------------------------------------------------------------------------------------|
| DCM::Instructions | Instructions       | geel: patch wijziging | SIMPLE PATCH CHANGE | Tekstueel en in voorbeelden aanpassen zib Alert vanwege de nieuwe zib MedicatieContraindicatie |

## Changes

| ConceptID_2017   | ConceptName_2017               | Change                | TypeChange          | Impact_heen   | TRANSLATIE_spec_heen                                        | Impact_terug   | TRANSLATIE_spec_terug                                       | Omschrijving                                                                                                                                   |
|:-----------------|:-------------------------------|:----------------------|:--------------------|:--------------|:------------------------------------------------------------|:---------------|:------------------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------|
| NL-CM:8.3.3      | Conditie::Probleem             | geel: patch wijziging | SIMPLE PATCH CHANGE | Low           | leeg maken                                                  | Low            |                                                             | Tekstueel en in voorbeelden aanpassen zib Alert vanwege de nieuwe zib MedicatieContraindicatie                                                 |
| NL-CM:8.3.4      | AlertNaam                      | geel: patch wijziging | SIMPLE PATCH CHANGE | Low           | leeg maken                                                  | Low            |                                                             | Typo in de definite van alertnaam (vastgelegd) is aangepast                                                                                    |
| NL-CM:8.3.4      | AlertNaam                      | oranje: minor change  | VALUESET CHANGES    | Low           | existing valueset [valuesetname] changed in [baseline 2020] | Medium         | existing valueset [valuesetname] changed in [baseline 2020] | De vanuit het programma antibioticaresistentie (ABR) aangeleverde lijst met 7 BMRO groepen zijn toegevoegd/aangepast in de AlertNaamCodelijst. |
| NL-CM:8.3.7      | **concept toegevoegd in 2020** | rood: major change    | CONCEPT ADDITION    | Low           |                                                             | High           | IF source <> [blank] THEN source -> target=[non-zib item]   | Element is toegevoegd aan het rootconcept                                                                                                      |
| NL-CM:8.3.8      | **concept toegevoegd in 2020** | rood: major change    | CONCEPT ADDITION    | Low           |                                                             | High           | IF source <> [blank] THEN source -> target=[non-zib item]   | Toevoegen EindDatum bij zibs die ook BeginDatum kennen                                                                                         |

## Mapping

| ZibName   | ConceptID_2017   | ConceptName_2017               | Codelists_2017     | Change                  | ConceptID_2020   | ConceptName_2020   | Codelists_2020     | Bits              | Omschrijving                                                                                                                                   | TypeChange          | Impact_heen   | TRANSLATIE_spec_heen                                        | Impact_terug   | TRANSLATIE_spec_terug                                       |
|:----------|:-----------------|:-------------------------------|:-------------------|:------------------------|:-----------------|:-------------------|:-------------------|:------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------|:--------------------|:--------------|:------------------------------------------------------------|:---------------|:------------------------------------------------------------|
| Alert     | NL-CM:8.3.1      | Alert                          |                    | groen: geen wijzigingen | NL-CM:8.3.1      | Alert              |                    |                   |                                                                                                                                                |                     |               |                                                             |                |                                                             |
| Alert     | NL-CM:8.3.3      | Conditie::Probleem             |                    | geel: patch wijziging   | NL-CM:8.3.3      | Conditie::Probleem |                    | ZIB-1209          | Tekstueel en in voorbeelden aanpassen zib Alert vanwege de nieuwe zib MedicatieContraindicatie                                                 | SIMPLE PATCH CHANGE | Low           | leeg maken                                                  | Low            |                                                             |
| Alert     | NL-CM:8.3.4      | AlertNaam                      | AlertNaamCodelijst | geel: patch wijziging   | NL-CM:8.3.4      | AlertNaam          | AlertNaamCodelijst | ZIB-905           | Typo in de definite van alertnaam (vastgelegd) is aangepast                                                                                    | SIMPLE PATCH CHANGE | Low           | leeg maken                                                  | Low            |                                                             |
| Alert     | NL-CM:8.3.4      | AlertNaam                      | AlertNaamCodelijst | oranje: minor change    | NL-CM:8.3.4      | AlertNaam          | AlertNaamCodelijst | ZIB-905 ; ZIB-813 | De vanuit het programma antibioticaresistentie (ABR) aangeleverde lijst met 7 BMRO groepen zijn toegevoegd/aangepast in de AlertNaamCodelijst. | VALUESET CHANGES    | Low           | existing valueset [valuesetname] changed in [baseline 2020] | Medium         | existing valueset [valuesetname] changed in [baseline 2020] |
| Alert     | NL-CM:8.3.5      | BeginDatumTijd                 |                    | groen: geen wijzigingen | NL-CM:8.3.5      | BeginDatumTijd     |                    |                   |                                                                                                                                                |                     |               | ALS [aantal >1] DAN [doe iets] ANDERS source -> target      |                |                                                             |
| Alert     | NL-CM:8.3.6      | AlertType                      | AlertTypeCodelijst | groen: geen wijzigingen | NL-CM:8.3.6      | AlertType          | AlertTypeCodelijst |                   |                                                                                                                                                |                     |               |                                                             |                |                                                             |
| Alert     | NL-CM:8.3.7      | **concept toegevoegd in 2020** |                    | rood: major change      | NL-CM:8.3.7      | Toelichting        |                    | ZIB-682           | Element is toegevoegd aan het rootconcept                                                                                                      | CONCEPT ADDITION    | Low           |                                                             | High           | IF source <> [blank] THEN source -> target=[non-zib item]   |
| Alert     | NL-CM:8.3.8      | **concept toegevoegd in 2020** |                    | rood: major change      | NL-CM:8.3.8      | EindDatumTijd      |                    | ZIB-526           | Toevoegen EindDatum bij zibs die ook BeginDatum kennen                                                                                         | CONCEPT ADDITION    | Low           |                                                             | High           | IF source <> [blank] THEN source -> target=[non-zib item]   |

