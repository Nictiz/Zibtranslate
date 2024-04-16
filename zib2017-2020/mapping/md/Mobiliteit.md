# Mobiliteit
## File formats

The translation specs are available as: 
[CSV](../csv/Mobiliteit.csv) [JSON](../json/Mobiliteit.json) [XML](../xml/Mobiliteit.xml)



[Mobiliteit-v3.1(2017NL)](https://zibs.nl/wiki/Mobiliteit-v3.1(2017NL))

[Mobiliteit-v3.3(2020NL)](https://zibs.nl/wiki/Mobiliteit-v3.3(2020NL))









## Changes

| ConceptID_2017   | ConceptName_2017   | Change               | TypeChange       | Impact_heen   | TRANSLATIE_spec_heen                         | Impact_terug   | TRANSLATIE_spec_terug                        | Omschrijving                 |
|:-----------------|:-------------------|:---------------------|:-----------------|:--------------|:---------------------------------------------|:---------------|:---------------------------------------------|:-----------------------------|
| NL-CM:4.3.3      | Lopen              | oranje: minor change | DATATYPE CHANGE  | Low           | valueset datatype CO -> valueset datatype CD | Low            | valueset datatype CD -> valueset datatype CO | Datatype CO gewijzigd in CD  |
| NL-CM:4.3.5      | UitvoerenTransfer  | oranje: minor change | DATATYPE CHANGE  | Low           | valueset datatype CO -> valueset datatype CD | Low            | valueset datatype CD -> valueset datatype CO | Datatype CO gewijzigd in CD  |
| NL-CM:4.3.5      | UitvoerenTransfer  | oranje: minor change | VALUESET CHANGES | Low           | valuesets 2017 -> valueset 2020 regel        | Medium         | valuesets 2017 <- valueset 2020 regel        | Deprecated code in codelijst |
| NL-CM:4.3.8      | HoudingVeranderen  | oranje: minor change | DATATYPE CHANGE  | Low           | valueset datatype CO -> valueset datatype CD | Low            | valueset datatype CD -> valueset datatype CO | Datatype CO gewijzigd in CD  |
| NL-CM:4.3.12     | HoudingHandhaven   | oranje: minor change | DATATYPE CHANGE  | Low           | valueset datatype CO -> valueset datatype CD | Low            | valueset datatype CD -> valueset datatype CO | Datatype CO gewijzigd in CD  |
| NL-CM:4.3.18     | Traplopen          | oranje: minor change | DATATYPE CHANGE  | Low           | valueset datatype CO -> valueset datatype CD | Low            | valueset datatype CD -> valueset datatype CO | Datatype CO gewijzigd in CD  |

## Mapping

| ZibName    | ConceptID_2017   | ConceptName_2017   | Codelists_2017             | Change                  | ConceptID_2020   | ConceptName_2020   | Codelists_2020             | Bits     | Omschrijving                 | TypeChange       | Impact_heen   | TRANSLATIE_spec_heen                         | Impact_terug   | TRANSLATIE_spec_terug                        |
|:-----------|:-----------------|:-------------------|:---------------------------|:------------------------|:-----------------|:-------------------|:---------------------------|:---------|:-----------------------------|:-----------------|:--------------|:---------------------------------------------|:---------------|:---------------------------------------------|
| Mobiliteit | NL-CM:4.3.1      | Mobiliteit         |                            | groen: geen wijzigingen | NL-CM:4.3.1      | Mobiliteit         |                            |          |                              |                  |               |                                              |                |                                              |
| Mobiliteit | NL-CM:4.3.3      | Lopen              | LopenCodelijst             | oranje: minor change    | NL-CM:4.3.3      | Lopen              | LopenCodelijst             | ZIB-1113 | Datatype CO gewijzigd in CD  | DATATYPE CHANGE  | Low           | valueset datatype CO -> valueset datatype CD | Low            | valueset datatype CD -> valueset datatype CO |
| Mobiliteit | NL-CM:4.3.4      | MedischHulpmiddel  |                            | groen: geen wijzigingen | NL-CM:4.3.4      | MedischHulpmiddel  |                            |          |                              |                  |               |                                              |                |                                              |
| Mobiliteit | NL-CM:4.3.5      | UitvoerenTransfer  | UitvoerenTransferCodelijst | oranje: minor change    | NL-CM:4.3.5      | UitvoerenTransfer  | UitvoerenTransferCodelijst | ZIB-1113 | Datatype CO gewijzigd in CD  | DATATYPE CHANGE  | Low           | valueset datatype CO -> valueset datatype CD | Low            | valueset datatype CD -> valueset datatype CO |
| Mobiliteit | NL-CM:4.3.5      | UitvoerenTransfer  | UitvoerenTransferCodelijst | oranje: minor change    | NL-CM:4.3.5      | UitvoerenTransfer  | UitvoerenTransferCodelijst | ZIB-732  | Deprecated code in codelijst | VALUESET CHANGES | Low           | valuesets 2017 -> valueset 2020 regel        | Medium         | valuesets 2017 <- valueset 2020 regel        |
| Mobiliteit | NL-CM:4.3.8      | HoudingVeranderen  | HoudingVeranderenCodelijst | oranje: minor change    | NL-CM:4.3.8      | HoudingVeranderen  | HoudingVeranderenCodelijst | ZIB-1113 | Datatype CO gewijzigd in CD  | DATATYPE CHANGE  | Low           | valueset datatype CO -> valueset datatype CD | Low            | valueset datatype CD -> valueset datatype CO |
| Mobiliteit | NL-CM:4.3.12     | HoudingHandhaven   | HoudingHandhavenCodelijst  | oranje: minor change    | NL-CM:4.3.12     | HoudingHandhaven   | HoudingHandhavenCodelijst  | ZIB-1113 | Datatype CO gewijzigd in CD  | DATATYPE CHANGE  | Low           | valueset datatype CO -> valueset datatype CD | Low            | valueset datatype CD -> valueset datatype CO |
| Mobiliteit | NL-CM:4.3.16     | Toelichting        |                            | groen: geen wijzigingen | NL-CM:4.3.16     | Toelichting        |                            |          |                              |                  |               |                                              |                |                                              |
| Mobiliteit | NL-CM:4.3.18     | Traplopen          | TraplopenCodelijst         | oranje: minor change    | NL-CM:4.3.18     | Traplopen          | TraplopenCodelijst         | ZIB-1113 | Datatype CO gewijzigd in CD  | DATATYPE CHANGE  | Low           | valueset datatype CO -> valueset datatype CD | Low            | valueset datatype CD -> valueset datatype CO |

