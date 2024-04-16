# Wilsverklaring
## File formats

The translation specs are available as: 
[CSV](../csv/Wilsverklaring.csv) [JSON](../json/Wilsverklaring.json) [XML](../xml/Wilsverklaring.xml)



[Wilsverklaring-v3.1(2017NL)](https://zibs.nl/wiki/Wilsverklaring-v3.1(2017NL))

[Wilsverklaring-v3.1.1(2020NL)](https://zibs.nl/wiki/Wilsverklaring-v3.1.1(2020NL))







## Zib-level changes

| ConceptID_2017   | ConceptName_2017   | Change                | TypeChange          | Omschrijving                                                                            |
|:-----------------|:-------------------|:----------------------|:--------------------|:----------------------------------------------------------------------------------------|
| DCM::References  | References         | geel: patch wijziging | SIMPLE PATCH CHANGE | Referenties in sectie 'References' bijgewerkt naar juiste url van de NPCF, NVVE en NPV. |

## Changes

| ConceptID_2017   | ConceptName_2017   | Change               | TypeChange       | Impact_heen   | TRANSLATIE_spec_heen                  | Impact_terug   | TRANSLATIE_spec_terug                 | Omschrijving                                                                   |
|:-----------------|:-------------------|:---------------------|:-----------------|:--------------|:--------------------------------------|:---------------|:--------------------------------------|:-------------------------------------------------------------------------------|
| NL-CM:7.15.2     | WilsverklaringType | oranje: minor change | VALUESET CHANGES | Low           | valuesets 2017 -> valueset 2020 regel | Medium         | valuesets 2017 <- valueset 2020 regel | Zelfbindingsverklaring is als item toegevoegd aan WilsverklaringTypeCodelijst. |

## Mapping

| ZibName        | ConceptID_2017   | ConceptName_2017                  | Codelists_2017              | Change                  | ConceptID_2020   | ConceptName_2020                  | Codelists_2020              | Bits    | Omschrijving                                                                   | TypeChange       | Impact_heen   | TRANSLATIE_spec_heen                  | Impact_terug   | TRANSLATIE_spec_terug                 |
|:---------------|:-----------------|:----------------------------------|:----------------------------|:------------------------|:-----------------|:----------------------------------|:----------------------------|:--------|:-------------------------------------------------------------------------------|:-----------------|:--------------|:--------------------------------------|:---------------|:--------------------------------------|
| Wilsverklaring | NL-CM:7.15.1     | Wilsverklaring                    |                             | groen: geen wijzigingen | NL-CM:7.15.1     | Wilsverklaring                    |                             |         |                                                                                |                  |               |                                       |                |                                       |
| Wilsverklaring | NL-CM:7.15.2     | WilsverklaringType                | WilsverklaringTypeCodelijst | oranje: minor change    | NL-CM:7.15.2     | WilsverklaringType                | WilsverklaringTypeCodelijst | ZIB-739 | Zelfbindingsverklaring is als item toegevoegd aan WilsverklaringTypeCodelijst. | VALUESET CHANGES | Low           | valuesets 2017 -> valueset 2020 regel | Medium         | valuesets 2017 <- valueset 2020 regel |
| Wilsverklaring | NL-CM:7.15.3     | Vertegenwoordiger::Contactpersoon |                             | groen: geen wijzigingen | NL-CM:7.15.3     | Vertegenwoordiger::Contactpersoon |                             |         |                                                                                |                  |               |                                       |                |                                       |
| Wilsverklaring | NL-CM:7.15.4     | Aandoening::Probleem              |                             | groen: geen wijzigingen | NL-CM:7.15.4     | Aandoening::Probleem              |                             |         |                                                                                |                  |               |                                       |                |                                       |
| Wilsverklaring | NL-CM:7.15.5     | WilsverklaringDocument            |                             | groen: geen wijzigingen | NL-CM:7.15.5     | WilsverklaringDocument            |                             |         |                                                                                |                  |               |                                       |                |                                       |
| Wilsverklaring | NL-CM:7.15.6     | Toelichting                       |                             | groen: geen wijzigingen | NL-CM:7.15.6     | Toelichting                       |                             |         |                                                                                |                  |               |                                       |                |                                       |
| Wilsverklaring | NL-CM:7.15.7     | WilsverklaringDatum               |                             | groen: geen wijzigingen | NL-CM:7.15.7     | WilsverklaringDatum               |                             |         |                                                                                |                  |               |                                       |                |                                       |

