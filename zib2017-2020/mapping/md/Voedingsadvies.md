# Voedingsadvies
## File formats

The translation specs are available as: 
[CSV](../csv/Voedingsadvies.csv) [JSON](../json/Voedingsadvies.json) [XML](../xml/Voedingsadvies.xml)



[Voedingsadvies-v3.1(2017NL)](https://zibs.nl/wiki/Voedingsadvies-v3.1(2017NL))

[Voedingsadvies-v3.2(2020NL)](https://zibs.nl/wiki/Voedingsadvies-v3.2(2020NL))









## Changes

| ConceptID_2017   | ConceptName_2017               | Change             | TypeChange       | Impact_heen   | TRANSLATIE_spec_heen   | Impact_terug   | TRANSLATIE_spec_terug                                                                                                                                                                             | Omschrijving                            |
|:-----------------|:-------------------------------|:-------------------|:-----------------|:--------------|:-----------------------|:---------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------------------------------------|
| NL-CM:7.11.5     | **concept toegevoegd in 2020** | rood: major change | CONCEPT ADDITION | Low           |                        | High           | IF [blank] source->target ELSE [toon en stuur de relatie tussen het voedings advies en het probleem naar een 2017 ontvanger. Maak eventueel een probleem instance aan als deze nog niet bestaat ] | Verwijzing naar zib probleem toegeveogd |

## Mapping

| ZibName        | ConceptID_2017   | ConceptName_2017               | Codelists_2017   | Change                  | ConceptID_2020   | ConceptName_2020    | Codelists_2020   | Bits    | Omschrijving                            | TypeChange       | Impact_heen   | TRANSLATIE_spec_heen   | Impact_terug   | TRANSLATIE_spec_terug                                                                                                                                                                             |
|:---------------|:-----------------|:-------------------------------|:-----------------|:------------------------|:-----------------|:--------------------|:-----------------|:--------|:----------------------------------------|:-----------------|:--------------|:-----------------------|:---------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Voedingsadvies | NL-CM:7.11.1     | Voedingsadvies                 |                  | groen: geen wijzigingen | NL-CM:7.11.1     | Voedingsadvies      |                  |         |                                         |                  |               |                        |                |                                                                                                                                                                                                   |
| Voedingsadvies | NL-CM:7.11.2     | DieetType                      |                  | groen: geen wijzigingen | NL-CM:7.11.2     | DieetType           |                  |         |                                         |                  |               |                        |                |                                                                                                                                                                                                   |
| Voedingsadvies | NL-CM:7.11.3     | Consistentie                   |                  | groen: geen wijzigingen | NL-CM:7.11.3     | Consistentie        |                  |         |                                         |                  |               |                        |                |                                                                                                                                                                                                   |
| Voedingsadvies | NL-CM:7.11.4     | Toelichting                    |                  | groen: geen wijzigingen | NL-CM:7.11.4     | Toelichting         |                  |         |                                         |                  |               |                        |                |                                                                                                                                                                                                   |
| Voedingsadvies | NL-CM:7.11.5     | **concept toegevoegd in 2020** |                  | rood: major change      | NL-CM:7.11.5     | Indicatie::Probleem |                  | ZIB_707 | Verwijzing naar zib probleem toegeveogd | CONCEPT ADDITION | Low           |                        | High           | IF [blank] source->target ELSE [toon en stuur de relatie tussen het voedings advies en het probleem naar een 2017 ontvanger. Maak eventueel een probleem instance aan als deze nog niet bestaat ] |

