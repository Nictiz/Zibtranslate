# Probleem
## File formats

The translation specs are available as: 
[CSV](../csv/Probleem.csv) [JSON](../json/Probleem.json) [XML](../xml/Probleem.xml) [Excel](../excel/Probleem.xlsx)



## Zib Probleem

[Probleem-v4.1(2017NL)](https://zibs.nl/wiki/Probleem-v4.1(2017NL))

[Probleem-v4.4(2020NL)](https://zibs.nl/wiki/Probleem-v4.4(2020NL))



voor Tabel 40, wat Thesaurus 40 moet zijn zie https://www.z-index.nl/g-standaard ; voor diagnose thesaurus zie https://www.dhd.nl/producten-diensten/registratie-data/oplossingen-voor-registratievraagstukken ; voor ICD-10 NL zie https://www.whofic.nl : voor kernsets zie https://nictiz.nl/wat-we-doen/activiteiten/terminologie/referentielijsten/nationale-kernset/ ; voor ICPC zie https://www.nhg.org/praktijkvoering/informatisering/nhg-tabellen-voor-in-his/; voor ggz codelijsten zie https://www.denederlandseggz.nl/en. zie ook https://nationalebibliotheek.nictiz.nl/ en https://nandanicnoc.bsl.nl voor NIC NOC en NANDA 

de GGZ diagnoselijst (in excel)  wordt momenteel omgezet in een SNOMED CT referentieset. Zie ook https://nictiz.atlassian.net/browse/ZIB-2087

## Zib-level changes

| ConceptID_2017    | ConceptName_2017   | Change                | TypeChange          | Omschrijving                   |
|:------------------|:-------------------|:----------------------|:--------------------|:-------------------------------|
| DCM::Instructions | Instructions       | geel: patch wijziging | SIMPLE PATCH CHANGE | Tekstwijziging in instructions |

## Changes

| ConceptID_2017   | ConceptName_2017               | Change                | TypeChange          | Impact_heen   | TRANSLATIE_spec_heen                                                                                                                                                | Impact_terug   | TRANSLATIE_spec_terug                                                                                                                                               | Omschrijving                                                          |
|:-----------------|:-------------------------------|:----------------------|:--------------------|:--------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|:---------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------------------------------------------------------------------|
| NL-CM:5.1.3      | ProbleemNaam                   | oranje: minor change  | VALUESET CHANGES    | Low           | valuesets 2017 -> valueset 2020 regel                                                                                                                               | Medium         | valuesets 2017 <- valueset 2020 regel                                                                                                                               | diverse wijzigingen in codelijst (codestelsels en referentiesets)     |
| NL-CM:5.1.6      | ProbleemBeginDatum             | geel: patch wijziging | SIMPLE PATCH CHANGE | Low           |                                                                                                                                                                     | Low            |                                                                                                                                                                     | Tekstwijziging aan defintie concept                                   |
| NL-CM:5.1.8      | ProbleemType                   | oranje: minor change  | VALUESET CHANGES    | Low           | valuesets 2017 -> valueset 2020 regel                                                                                                                               | Medium         | valuesets 2017 <- valueset 2020 regel                                                                                                                               | uitbreiding codelijst met item 'bevinding'                            |
| NL-CM:5.1.11     | ProbleemAnatomischeLocatie     | oranje: minor change  | CHANGE TO SUB HCIM  | Medium        | codelist [ProbleemAnatomischeLocatieCodelijst]->[LocatieCodelijst (http://decor.nictiz.nl/fhir/ValueSet/2.16.840.1.113883.2.4.3.11.60.40.2.20.7.1--20200901000000)] | Medium         | codelist [LocatieCodelijst (http://decor.nictiz.nl/fhir/ValueSet/2.16.840.1.113883.2.4.3.11.60.40.2.20.7.1--20200901000000)]->[ProbleemAnatomischeLocatieCodelijst] | nieuwe verwijzing naar sub-bouwsteen anatomischeLocatie               |
| NL-CM:5.1.11     | ProbleemAnatomischeLocatie     | geel: patch wijziging | SIMPLE PATCH CHANGE | Low           |                                                                                                                                                                     | Low            |                                                                                                                                                                     | Tekstwijziging definitie concept                                      |
| NL-CM:5.1.12     | ProbleemLateraliteit           | oranje: minor change  | CHANGE TO SUB HCIM  | Medium        | codelist [ProbleemLateraliteitCodelijst]->[LateraliteitCodelijst (http://decor.nictiz.nl/fhir/ValueSet/2.16.840.1.113883.2.4.3.11.60.40.2.20.7.2--20200901000000)]  | Medium         | codelist [LateraliteitCodelijst (http://decor.nictiz.nl/fhir/ValueSet/2.16.840.1.113883.2.4.3.11.60.40.2.20.7.2--20200901000000)]->[ProbleemLateraliteitCodelijst]  | nieuwe verwijzing naar sub-bouwsteen anatomischeLocatie               |
| NL-CM:5.1.13     | **concept toegevoegd in 2020** | rood: major change    | CONCEPT ADDITION    | Low           |                                                                                                                                                                     | High           | IF [blank]source->target ELSE [toon en stuur de inhoud van dit data item als vrije tekst naar een 2017 ontvanger]                                                   | Item 'NadereSpecificatieProbleemNaam' toegevoegd aan informatiemodel. |

## Mapping

| ConceptID_2017   | ConceptName_2017               | Codelists_2017                                                                                                                                                                                                                   | Change                  | ConceptID_2020   | ConceptName_2020                               | Codelists_2020                                                                                                                                                                                                                                                                           | Bits                                                                    | Omschrijving                                                          | TypeChange          | Impact_heen   | TRANSLATIE_spec_heen                                                                                                                                                | Impact_terug   | TRANSLATIE_spec_terug                                                                                                                                               |
|:-----------------|:-------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:------------------------|:-----------------|:-----------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:------------------------------------------------------------------------|:----------------------------------------------------------------------|:--------------------|:--------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|:---------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| NL-CM:5.1.1      | Probleem                       |                                                                                                                                                                                                                                  | groen: geen wijzigingen | NL-CM:5.1.1      | Probleem                                       |                                                                                                                                                                                                                                                                                          |                                                                         |                                                                       | NO CHANGE           |               |                                                                                                                                                                     |                |                                                                                                                                                                     |
| NL-CM:5.1.3      | ProbleemNaam                   | ProbleemNaamCodelijst = Diagnosethesaurus DHD (SNOMED CT) ; ICD-10 ; Nationale Kernset Patiëntproblemen V&VN (SNOMED CT) ; NANDA-I ; Omaha Systems ; ICF ; ICPC-1 NL ; G-Standaard Contra Indicaties (Tabel 40) ; DSM-IV ; DSM-V | oranje: minor change    | NL-CM:5.1.3      | ProbleemNaam                                   | ProbleemNaamCodelijst = Omaha Systems [DEPRECATED] ; G-Standaard Contra Indicaties (Tabel 40) [DEPRECATED] ; DHD Diagnosethesaurus ; ICD-10, dutch translation ; SNOMED CT: ^11721000146100 ; Nationale kernset patiëntproblemen ; ICF ; ICPC-1 NL ; DSM-IV ; DSM-5 ; GGZ Diagnoselijst) | ZIB-1110 ; ZIB-661 ; ZIB-987 ; ZIB-1133 ; ZIB-1175 ; ZIB-624 ; ZIB-1477 | diverse wijzigingen in codelijst (codestelsels en referentiesets)     | VALUESET CHANGES    | Low           | valuesets 2017 -> valueset 2020 regel                                                                                                                               | Medium         | valuesets 2017 <- valueset 2020 regel                                                                                                                               |
| NL-CM:5.1.4      | ProbleemStatus                 | ProbleemStatusCodelijst                                                                                                                                                                                                          | groen: geen wijzigingen | NL-CM:5.1.4      | ProbleemStatus                                 | ProbleemStatusCodelijst                                                                                                                                                                                                                                                                  |                                                                         |                                                                       | NO CHANGE           |               |                                                                                                                                                                     |                |                                                                                                                                                                     |
| NL-CM:5.1.5      | Toelichting                    |                                                                                                                                                                                                                                  | groen: geen wijzigingen | NL-CM:5.1.5      | Toelichting                                    |                                                                                                                                                                                                                                                                                          |                                                                         |                                                                       | NO CHANGE           |               |                                                                                                                                                                     |                |                                                                                                                                                                     |
| NL-CM:5.1.6      | ProbleemBeginDatum             |                                                                                                                                                                                                                                  | geel: patch wijziging   | NL-CM:5.1.6      | ProbleemBeginDatum                             |                                                                                                                                                                                                                                                                                          | ZIB-963 ; ZIB-1202                                                      | Tekstwijziging aan defintie concept                                   | SIMPLE PATCH CHANGE | Low           |                                                                                                                                                                     | Low            |                                                                                                                                                                     |
| NL-CM:5.1.8      | ProbleemType                   | ProbleemTypeCodelijst                                                                                                                                                                                                            | oranje: minor change    | NL-CM:5.1.8      | ProbleemType                                   | ProbleemTypeCodelijst                                                                                                                                                                                                                                                                    | ZIB-627                                                                 | uitbreiding codelijst met item 'bevinding'                            | VALUESET CHANGES    | Low           | valuesets 2017 -> valueset 2020 regel                                                                                                                               | Medium         | valuesets 2017 <- valueset 2020 regel                                                                                                                               |
| NL-CM:5.1.9      | ProbleemEindDatum              |                                                                                                                                                                                                                                  | groen: geen wijzigingen | NL-CM:5.1.9      | ProbleemEindDatum                              |                                                                                                                                                                                                                                                                                          |                                                                         |                                                                       | NO CHANGE           |               |                                                                                                                                                                     |                |                                                                                                                                                                     |
| NL-CM:5.1.10     | VerificatieStatus              | VerificatieStatusCodelijst                                                                                                                                                                                                       | groen: geen wijzigingen | NL-CM:5.1.10     | VerificatieStatus                              | VerificatieStatusCodelijst                                                                                                                                                                                                                                                               |                                                                         |                                                                       | NO CHANGE           |               |                                                                                                                                                                     |                |                                                                                                                                                                     |
| NL-CM:5.1.11     | ProbleemAnatomischeLocatie     | ProbleemAnatomischeLocatieCodelijst                                                                                                                                                                                              | oranje: minor change    | NL-CM:5.1.14     | ProbleemAnatomischeLocatie::AnatomischeLocatie | LocatieCodelijst                                                                                                                                                                                                                                                                         | ZIB-816 ; ZIB-1116                                                      | nieuwe verwijzing naar sub-bouwsteen anatomischeLocatie               | CHANGE TO SUB HCIM  | Medium        | codelist [ProbleemAnatomischeLocatieCodelijst]->[LocatieCodelijst (http://decor.nictiz.nl/fhir/ValueSet/2.16.840.1.113883.2.4.3.11.60.40.2.20.7.1--20200901000000)] | Medium         | codelist [LocatieCodelijst (http://decor.nictiz.nl/fhir/ValueSet/2.16.840.1.113883.2.4.3.11.60.40.2.20.7.1--20200901000000)]->[ProbleemAnatomischeLocatieCodelijst] |
| NL-CM:5.1.11     | ProbleemAnatomischeLocatie     | ProbleemAnatomischeLocatieCodelijst                                                                                                                                                                                              | geel: patch wijziging   | NL-CM:5.1.14     | ProbleemAnatomischeLocatie::AnatomischeLocatie | AnatomischeLocatieCodelijst                                                                                                                                                                                                                                                              | ZIB-816 ; ZIB-1116                                                      | Tekstwijziging definitie concept                                      | SIMPLE PATCH CHANGE | Low           |                                                                                                                                                                     | Low            |                                                                                                                                                                     |
| NL-CM:5.1.12     | ProbleemLateraliteit           | ProbleemLateraliteitCodelijst                                                                                                                                                                                                    | oranje: minor change    | NL-CM:5.1.14     | ProbleemAnatomischeLocatie::Lateraliteit       | LateraliteitCodelijs                                                                                                                                                                                                                                                                     | ZIB-1116                                                                | nieuwe verwijzing naar sub-bouwsteen anatomischeLocatie               | CHANGE TO SUB HCIM  | Medium        | codelist [ProbleemLateraliteitCodelijst]->[LateraliteitCodelijst (http://decor.nictiz.nl/fhir/ValueSet/2.16.840.1.113883.2.4.3.11.60.40.2.20.7.2--20200901000000)]  | Medium         | codelist [LateraliteitCodelijst (http://decor.nictiz.nl/fhir/ValueSet/2.16.840.1.113883.2.4.3.11.60.40.2.20.7.2--20200901000000)]->[ProbleemLateraliteitCodelijst]  |
| NL-CM:5.1.13     | **concept toegevoegd in 2020** |                                                                                                                                                                                                                                  | rood: major change      | NL-CM:5.1.13     | NadereSpecificatieProbleemNaam                 |                                                                                                                                                                                                                                                                                          | ZIB-1147                                                                | Item 'NadereSpecificatieProbleemNaam' toegevoegd aan informatiemodel. | CONCEPT ADDITION    | Low           |                                                                                                                                                                     | High           | IF [blank]source->target ELSE [toon en stuur de inhoud van dit data item als vrije tekst naar een 2017 ontvanger]                                                   |
