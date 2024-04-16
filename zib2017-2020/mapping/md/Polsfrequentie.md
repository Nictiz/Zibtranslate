# Polsfrequentie
## File formats

The translation specs are available as: 
[CSV](../csv/Polsfrequentie.csv) [JSON](../json/Polsfrequentie.json) [XML](../xml/Polsfrequentie.xml)



[Polsfrequentie-v3.1(2017NL)](https://zibs.nl/wiki/Polsfrequentie-v3.1(2017NL))

[Polsfrequentie-v3.3(2020NL)](https://zibs.nl/wiki/Polsfrequentie-v3.3(2020NL))









## Changes

| ConceptID_2017   | ConceptName_2017     | Change               | TypeChange                         | Impact_heen   | TRANSLATIE_spec_heen                                                  | Impact_terug   | TRANSLATIE_spec_terug                                                 | Omschrijving                                                                                                                                                                |
|:-----------------|:---------------------|:---------------------|:-----------------------------------|:--------------|:----------------------------------------------------------------------|:---------------|:----------------------------------------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| NL-CM:12.7.2     | PolsfrequentieWaarde | oranje: minor change | CARDINALITY CHANGE                 | Medium        | ZERO-TO-ONE TO ONE                                                    | Low            | ONE TO ZERO-TO-ONE                                                    | De cardinaliteit van het element Polsfrequentiewaarde  (0..1) en Hartfrequentiewaarde uit zib Hartfrequentie (1) waren niet consistent. Dit is verbeterd, beiden zijn nu 1. |
| NL-CM:12.7.5     | PolsRegelmatigheid   | oranje: minor change | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | LOINC DefinitionCode [blank] -> [44969-4 Heart rate rhythm palpation] | Medium         | LOINC DefinitionCode [44969-4 Heart rate rhythm palpation] -> [blank] | LOINC DefintionCodes concept aangepast                                                                                                                                      |

## Mapping

| ZibName        | ConceptID_2017   | ConceptName_2017        | Codelists_2017              | Change                  | ConceptID_2020   | ConceptName_2020        | Codelists_2020              | Bits    | Omschrijving                                                                                                                                                                | TypeChange                         | Impact_heen   | TRANSLATIE_spec_heen                                                  | Impact_terug   | TRANSLATIE_spec_terug                                                 |
|:---------------|:-----------------|:------------------------|:----------------------------|:------------------------|:-----------------|:------------------------|:----------------------------|:--------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-----------------------------------|:--------------|:----------------------------------------------------------------------|:---------------|:----------------------------------------------------------------------|
| Polsfrequentie | NL-CM:12.7.1     | Polsfrequentie          |                             | groen: geen wijzigingen | NL-CM:12.7.1     | Polsfrequentie          |                             |         |                                                                                                                                                                             | NO CHANGE                          |               |                                                                       |                |                                                                       |
| Polsfrequentie | NL-CM:12.7.2     | PolsfrequentieWaarde    |                             | oranje: minor change    | NL-CM:12.7.2     | PolsfrequentieWaarde    |                             | ZIB-705 | De cardinaliteit van het element Polsfrequentiewaarde  (0..1) en Hartfrequentiewaarde uit zib Hartfrequentie (1) waren niet consistent. Dit is verbeterd, beiden zijn nu 1. | CARDINALITY CHANGE                 | Medium        | ZERO-TO-ONE TO ONE                                                    | Low            | ONE TO ZERO-TO-ONE                                                    |
| Polsfrequentie | NL-CM:12.7.3     | PolsfrequentieDatumTijd |                             | groen: geen wijzigingen | NL-CM:12.7.3     | PolsfrequentieDatumTijd |                             |         |                                                                                                                                                                             | NO CHANGE                          |               |                                                                       |                |                                                                       |
| Polsfrequentie | NL-CM:12.7.4     | Toelichting             |                             | groen: geen wijzigingen | NL-CM:12.7.4     | Toelichting             |                             |         |                                                                                                                                                                             | NO CHANGE                          |               |                                                                       |                |                                                                       |
| Polsfrequentie | NL-CM:12.7.5     | PolsRegelmatigheid      | PolsRegelmatigheidCodelijst | oranje: minor change    | NL-CM:12.7.5     | PolsRegelmatigheid      | PolsRegelmatigheidCodelijst | ZIB-689 | LOINC DefintionCodes concept aangepast                                                                                                                                      | TERMINOLOGY MAPPING CONCEPT CHANGE | Medium        | LOINC DefinitionCode [blank] -> [44969-4 Heart rate rhythm palpation] | Medium         | LOINC DefinitionCode [44969-4 Heart rate rhythm palpation] -> [blank] |

