# Woonsituatie
## File formats

The translation specs are available as: 
[CSV](../csv/Woonsituatie.csv) [JSON](../json/Woonsituatie.json) [XML](../xml/Woonsituatie.xml)



[Woonsituatie-v3.1(2017NL)](https://zibs.nl/wiki/Woonsituatie-v3.1(2017NL))

[Woonsituatie-v3.3(2020NL)](https://zibs.nl/wiki/Woonsituatie-v3.3(2020NL))









## Changes

| ConceptID_2017   | ConceptName_2017               | Change               | TypeChange       | Impact_heen   | TRANSLATIE_spec_heen                                        | Impact_terug   | TRANSLATIE_spec_terug                                       | Omschrijving                                                                    |
|:-----------------|:-------------------------------|:---------------------|:-----------------|:--------------|:------------------------------------------------------------|:---------------|:------------------------------------------------------------|:--------------------------------------------------------------------------------|
| NL-CM:7.8.3      | WoningType                     | oranje: minor change | VALUESET CHANGES | Low           | existing valueset [valuesetname] changed in [baseline 2020] | Medium         | existing valueset [valuesetname] changed in [baseline 2020] | Codelijst aangepast met meerdere aanpassingen                                   |
| NL-CM:7.8.4      | **concept toegevoegd in 2020** | rood: major change   | CONCEPT ADDITION | Low           |                                                             | High           | IF source <> [blank] THEN source -> target=[non-zib item]   | Aan het model twee elementen toegevoegd, WoningAanpassing en WoonOmstandigheid. |
| NL-CM:7.8.5      | **concept toegevoegd in 2020** | rood: major change   | CONCEPT ADDITION | Low           |                                                             | High           | IF source <> [blank] THEN source -> target=[non-zib item]   | Aan het model twee elementen toegevoegd, WoningAanpassing en WoonOmstandigheid. |

## Mapping

| ZibName      | ConceptID_2017   | ConceptName_2017               | Codelists_2017      | Change                  | ConceptID_2020   | ConceptName_2020   | Codelists_2020             | Bits                                  | Omschrijving                                                                    | TypeChange       | Impact_heen   | TRANSLATIE_spec_heen                                        | Impact_terug   | TRANSLATIE_spec_terug                                       |
|:-------------|:-----------------|:-------------------------------|:--------------------|:------------------------|:-----------------|:-------------------|:---------------------------|:--------------------------------------|:--------------------------------------------------------------------------------|:-----------------|:--------------|:------------------------------------------------------------|:---------------|:------------------------------------------------------------|
| Woonsituatie | NL-CM:7.8.1      | Woonsituatie                   |                     | groen: geen wijzigingen | NL-CM:7.8.1      | Woonsituatie       |                            |                                       |                                                                                 |                  |               |                                                             |                |                                                             |
| Woonsituatie | NL-CM:7.8.2      | Toelichting                    |                     | groen: geen wijzigingen | NL-CM:7.8.2      | Toelichting        |                            |                                       |                                                                                 |                  |               |                                                             |                |                                                             |
| Woonsituatie | NL-CM:7.8.3      | WoningType                     | WoningTypeCodelijst | oranje: minor change    | NL-CM:7.8.3      | WoningType         | WoningTypeCodelijst        | ZIB-653 ; ZIB-1100 ; ZIB-810 ; ZIB769 | Codelijst aangepast met meerdere aanpassingen                                   | VALUESET CHANGES | Low           | existing valueset [valuesetname] changed in [baseline 2020] | Medium         | existing valueset [valuesetname] changed in [baseline 2020] |
| Woonsituatie | NL-CM:7.8.4      | **concept toegevoegd in 2020** |                     | rood: major change      | NL-CM:7.8.4      | WoonOmstandigheid  | WoonOmstandigheidCodelijst | ZIB-694                               | Aan het model twee elementen toegevoegd, WoningAanpassing en WoonOmstandigheid. | CONCEPT ADDITION | Low           |                                                             | High           | IF source <> [blank] THEN source -> target=[non-zib item]   |
| Woonsituatie | NL-CM:7.8.5      | **concept toegevoegd in 2020** |                     | rood: major change      | NL-CM:7.8.5      | WoningAanpassing   | WoningAanpassingCodelijst  | ZIB-694                               | Aan het model twee elementen toegevoegd, WoningAanpassing en WoonOmstandigheid. | CONCEPT ADDITION | Low           |                                                             | High           | IF source <> [blank] THEN source -> target=[non-zib item]   |

