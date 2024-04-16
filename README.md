 # Generieke translatiespecificaties zibs (CONCEPT)

Bij het opstellen van deze translatiespecificaties is gekeken naar de wijzigingen en mogelijkheden voor translaties per zib-element. Een zib-element is een dataconcept van het het informatiemodel, een codelijst of een andere zib-sectie (zie ook https://zibs.nl/wiki/Zib_secties) 

## Aanleiding
De aanleiding en achtergrond bij dit verzoek en het nut van deze semantische translatiespecificaties is te lezen in de memo over de implementatie FHIR https://www.rijksoverheid.nl/documenten/publicaties/2022/10/21/implementatie-fhir

In deze memo op pagina 4 , ad 4 staat:
>*.....Het is ongewenst dat gegevensuitwisseling wordt bemoeilijkt tussen partijen die werken met verschillende generieke uitwisselingsstandaarden. In dit geval gaat het om de twee versies van Zibs op de verschillende versies van FHIR. Op verzoek van VWS stelt Nictiz de translatiespecificatie op tussen de twee Zib versies en neemt deze daarna in beheer. Het is vervolgens aan softwareleveranciers om de translatie in systemen in te bouwen op verzoek van zorgaanbieders wanneer dit nodig is voor de gegevensuitwisseling met ketenpartners. Deze translatie kan mogelijk ook gebruikt worden om ondersteuning te bieden in situaties waarbij gegevens in de EPD worden verwerkt op basis van Zibs 2017, maar in de uitwisseling al over gaat naar Zibs 2020*.

## Translatietabellen zibs (CONCEPT)
Dit is de eerste conceptversie van de translatiespecificaties met alle **95 zibs** die zowel in de 2017 als in de 2020 publicatie zitten. 
De **5 zibs die zijn deprecated** alsook de **15 nieuwe zibs** die er in publicatie 2020 zijn bijgekomen, zitten wel als tabel in deze specificaties maar zijn (nog) niet uitgewerkt. Ook de medicatie-zibs staan nog even on hold vanwege afstemming met MP-project.

Per zib zijn de translatiespecificaties te downloaden in CSV-, JSON-, XML- en Excel-formaat.

Zie [de index](zib2017-2020/index.md) om de beschikbare translatiespecificaties per zib te bekijken alsook de files te downloaden. 

Per zib zijn er 2 of 3 tabellen.
- Changes, met hierin alleen de zib-concepten waarop tussen 2017 en 2020 een wijziging heeft plaatsgevonden.
- Een mapping-tabel met hierin alle-zib concepten, met wat meer informatie zoals waardenlijsten en de BITS-issues waarin de details staan van het wijzigingsverzoek dat heeft geleid tot 1 of meer wijzigingen.
- Waar van toepassing een tabel met overige wijzigingen op de zib (momenteel alleen de tekstuele wijzigingen op definities van beschrijvende velden zoals concept, purpose, evidence base etc).

Voor de verschillende typen wijzigingen en bijbehorende translatieregels, zie [de type changes](typechanges.md).

## zib translatie bestanden ##

| Kolom | Omschrijving|
| --- | ----------- |
| **ConceptID_2017** | NL-CM code van het concept van het informatiemodel van de zib |
| **ConceptName_2017**| Nederlandse naam van het concept |
| **Codelists_2017**| de naam van de waardenlijst (indien een _CO_ of _CD_ datatype) |
| **Change** | zwaarte van de wijziging van 2017 naar 2020 zib | 
| * groen| geen wijziging op concept |
| * geel| patchwijziging (geen wijziging met impact op het informatiemodel van de zib)|
| * oranje | minor change
| * rood| major change, niet 'backward-compatibel' of geheel nieuwe zib |
| **ConceptID_2020** | NL-CM code van het concept van het informatiemodel van de zib |
| **ConceptName_2020**| Nederlandse naam van het concept |
| **Codelists_2020**| de naam van de waardenlijst (indien een _CO_ of _CD_ datatype) 
| **Change** | de wijzigingsverzoeken met daarin details over het wijzigingsproces, die na afstemming en autorisatie zijn gepubliceerd in de nieuwe release 2020. Voor details zie BITS. bijvoorbeeld https://nictiz.atlassian.net/browse/ZIB-647
|**Omschrijving** | zeer beknopte beschrijving van de wijziging op het concept. Voor meer details zie BITS of bekijk de zib op de wiki. Let op, er kunnen meerdere wijzigingen op 1 zib-concept zijn doorgevoerd in prepublicaties tussen 2017 en 2020|
| **Type change** | Het type of categorie wijziging. Voor uitleg en wat de translatieprincipes zijn rondom de wijziging op het zib concept zie [type changes](typechanges.md)|
| **Impact heen** | De impact van de wijziging op de translatie wanneer een 2017-zib naar een 2020-zib wordt vertaald (heen)|
| **Translatie spec heen** | Voor een aantal type changes zoals wijzigingen in terminology bindings en voor wijzigingen waar een concept is verwijderd of toegevoegd staat in een simple query-stijl beschreven hoe hier mee om te gaan. zie [type changes](typechanges.md)|
| **Impact terug** | De impact van de wijziging op de translatie wanneer een 2020-zib naar een 2017-zib wordt vertaald (terug)|
| **Translatie spec terug** | Voor een aantal type changes zoals wijzigingen in terminology bindings en voor wijzigingen waar een concept is verwijderd of toegevoegd staat in een simple query-stijl beschreven hoe hier mee om te gaan. zie [type changes](typechanges.md)|
