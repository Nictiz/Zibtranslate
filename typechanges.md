# Type changes
 ##	SIMPLE PATCH CHANGE
  
  Hierbij is de tekst in de beschrijving van een zib-concept (definitie) of in een beschrijvend onderdeel van de zib (definitie, concept, evidence base, instructions, issues etc) gewijzigd. De wijziging kan een aanvulling zijn, een aanpassing van tekst of tekst in een zib onderdeel waar voorheen nog niets stond. Wanneer de aanpassing alleen de Engelse tekst betreft is dit met [EN] aangegeven. Bij aanpassingen van de Nederlandse tekst is meestal ook de Engelse tekst aangepast waarbij het verstandig is deze ook altijd te vervangen. 
  > [ ] Voor een patch change zal het Zib-centrum tabellen beschikbaar maken tussen verschillende baselines om deze wijzigingen geautomatiseerd te laten verlopen.
  >
  > [ ] Zib-centrum gaat uitzoeken of deze lijst vanuit Enterprise Architect kan worden gegenereerd. Dan kan dit onderdeel zijn van een publicatie
   
## CONCEPT NAME or CODELIST NAME CHANGED

 Wanneer een conceptnaam of de naam van een codelijst wordt aangepast kan dit een 'breaking change' zijn afhankelijk van de implementatie. Dergelijke wijzigingen zijn waar mogelijk vermeden en alleen doorgevoerd als de impact ervan ten tijde van evaluatie klein leek te zijn. Of de impact van een dergelijke aanpassing daadwerkelijk klein is hangt af van de applicatie waar deze zib is ingebouwd en of en hoe vaak het concept of de codelijst elders in de software wordt aangeroepen. Voor deze aanpassingen is altijd aangegeven of het een Engelse en of Nederlandse name change is. 
 >Voorbeeld 
 >
 >**CONCEPT NAME CHANGED (EN): ::FarmaceuticalProduct-> ::PharmaceuticalProduct**
 
##	TERMINOLOGY MAPPING CONCEPT CHANGE
 
 Terminology mapping in zibs verloopt via DCM::DefinitionCodes tags aan een zib-element. Wijzigen van een terminology mapping kan verschillende redenen hebben. Soms zijn gebruikte SNOMED CT- en LOINC-codes deprecated of discourgaged in een nieuwe release, een andere keer wordt een wijziging doorgevoerd door het Zib-centrum omdat het Terminologiecentrum een beter concept heeft gevonden dat beter past of een fout corrigeert. Tussen 2017 en 2020 zijn veel zibs verrijkt met codes of gelijkgetrokken met gebruikte codes bij een ouder en reeds geïmplementeerd informatiemodel (=harmonisatie). Los van de aanleiding of reden van wijziging, die in BITS kan worden bekeken, zijn de wijzigingen op rootconcepten, containers en data-elementen van de zib als volgt beschreven.

 >
 >Voorbeeld:
 > 
 >**SCT DefintionCode [46973005 Bloeddrukmeting] -> [blank]**  
 >
 >**LOINC DefinitionCode [85354-9 Blood pressure panel with all children optional] -> [55284-4 Blood pressure systolic and diastolic]**

 
 
##	VALUESET CHANGES
 
 Wanneer er wijzigingen zijn in de inhoud van een waardenlijst (dus aan de keuze-opties) is het beter om niet te gaan 'patchen' van oud naar nieuw. Naast het feit dat hiermee translaties zeer complex te automatiseren zullen zijn is het ook niet juist om dit te doen omdat oudere instantiaties zijn vastgelegd met de beschikbare codelijsten/valuesets die horen bij de 2017-publicatie.

 Bij een translatie-usecase van 2017 naar 2020 en terug adviseert Nictiz houders van informatiestandaarden dringend om af te zien van translatie tussen waardenlijsten. In plaats daarvan zouden alle actoren in de uitwisseling tijdens de migratieperiode zowel de 2017- als 2020-waardenlijsten moeten ondersteunen. Dit geldt zowel voor de zender als de ontvanger en dit betreft zowel de waardenlijsten die aangepast zijn in de 2020-publicatie als de waardenlijsten die zijn toegevoegd aan bestaande zibs in de 2020-publicatie (refsets, NHG-tabellen, ggz-lijsten en overige nieuwe artefacten en codestelsels).
 
##	STRUCTURAL INFORMATIONMODEL CHANGES

Wijzigingen aan de structuur van een informatiemodel zijn of minor of major changes. Er zijn een aantal categorieën binnen dit soort wijzigingen met ieder een andere aanpak bij translatie:

### CARDINALITY CHANGES

Bij zibs als conceptueel informatiemodel worden de kardinaliteiten anders gedefinieerd dan in logische modellen. Hierbij dient te worden opgemerkt dat dit in het verleden niet altijd duidelijk is gemaakt en de definitie van conceptuele kardinaliteit pas later - in 2020 - is beschreven en gepubliceerd (<https://zibs.nl/wiki/Zib_kardinaliteiten>). Hierdoor zijn er in het verleden veel wijzigingsverzoeken om deze kardinaliteit te versoepelen (bijvoorbeeld van '1' naar '0..1') afgewezen, terwijl andere wijzigingsverzoeken wel tot aanpassing hebben geleid. Hiermee zijn de zib-publicaties van 2017 alsook 2020 de regels zoals beschreven op de wiki niet altijd consistent toegepast. Bij de FHIR-resources van 2020 heeft het HL7-team van Nictiz in de profiling guidelines for FHIR R4 beschreven hoe wordt omgegaan met de kardinaliteiten van de zibs in de zib-profielen en de daarop gebaseerde nl-core-profielen.

Wanneer een element met kardinaliteit '1' via translatie omgezet wordt naar element met kardinaliteit  '0..1' is er in de regel geen probleem. De andere kant op, van 0..1 naar 1, kan mogelijk leiden tot problemen. Een denkbare oplossing is om in deze gevallen een check te doen en een foutmelding af te geven en/of een (automatische) actie te koppelen aan het voorkomen ervan in de brondata.

 >**ALS [aantal<>1] DAN [Foutmelding] ANDERS source -> target**

Bij een kardinaliteit tussen 2 zib elementen van 0..* naar 0..1 zijn er mogelijk problemen bij translatie. Hier moet worden gecheckt of er meer dan 1 zinvolle data items in de instantiatie zitten. Wanneer dit het geval is dan kan er een foutmelding aan de gebruiker worden getoond en waar nodig zal de gebruiker een keuze worden voorgesteld. Hoe dan ook, in dit scenario zal er waarschijnlijk dataverlies zijn waarbij het aan de houder van de informatiestandaard is om hierin een juiste keuze te maken hoe hier mee om te gaan.

 > **ALS [aantal >1] DAN [Foutmelding] ANDERS source -> target**
  

###	CONCEPT ADDITION or REMOVAL

 Wanneer een zib-element wordt toegevoegd of wordt verwijderd tussen een oudere en een nieuwere versie, is dit altijd een major change omdat de translatie beide richtingen op zal resulteren in dataverlies.

Bij een verwijderd concept in een 2020 zib is er sprake van dataverlies bij vertalen van 2017 naar 2020 (heen). Bij een toegevoegd concept in 2020 is er sprake van dataverlies bij het vertalen van 2020 naar 2017 (terug). 

 > voorbeeld:  
 **'Er is een einddatum toegevoegd aan de zib alert'**   
 >**'het boolean concept zwanger is verwijderd'**
 
 Hierbij is een mogelijke oplossing denkbaar waarbij data op een andere manier (non-zib) wordt overgestuurd.

 >voorbeeld:   
 **IF [blank]source->target ELSE [toon en stuur de inhoud van dit data item als vrije tekst naar een 2020 ontvanger]**  
 >  
 >of iets complexer als nodig:  
  **IF [blank] source->target ELSE [toon en stuur de relatie tussen de labuitslag en UitgevoerdDoor::Zorgaanbieder naar een 2017 ontvanger. Maak eventueel een zorgaanbieder instance aan als deze nog niet bestaat ]**

  Dit soort translaties vergt goede analyse waarbij ook de reeds geïnstantieerde data aan zowel de kant van de sturende als ontvangende/vragende applicatie van een informatiestandaard moeten worden bestudeerd. 


###	CHANGE TO SUB HCIM
In publicatie 2020 is een nieuwe sub-bouwsteen voor anatomische locatie gepubliceerd omdat de 2 concepten anatomische locatie en lateraliteit in veel zibs voorkwamen. Hierbij zijn de 2 concepten voor locatie en lateraliteit gewijzigd naar 1 verwijzing naar de nieuwe zib. In de 2020 zib staat er dan bijvoorbeeld VerrichtingAnatomischeLocatie::AnatomischeLocatie. Alhoewel dit wat verwarrend lijkt, zal dit voor translatie heen en terug waarschijnlijk een eenvoudige wijziging zijn. De inhoud van de waardenlijsten uit publicatie 2017 is namelijk gelijk gebleven in publicatie 2020. De translatie bestaat daardoor simpelweg uit het overzetten van de geïnstantieerde waarde.

### DATA TYPE CHANGE
De enige data type change die voorkomt tussen 2017 en 2020 gaat om een aantal codelijsten. Deze waren in 2017 van het type _CO_ (Coded Ordinal). Dit was echter een fout, want de waardenlijsten die waren uitgegeven waren in feite toch van het type _CD_ (Coded Description). Een translatie betreft hierdoor alleen de definitie en niet de data of de structuur van het informatiemodel.

### DATETIME IN FUTURE ALLOWED
In de 2020-publicatie is de zib OverdrachtGeplandeZorgactiviteit komen te vervallen. Om alle type zorgactiviteiten in deze zib toch te kunnen plannen, is voor de desbetreffende zibs in 2020 het constraint op de begin- en einddatums opgeheven waardoor het mogelijk is om ook een datum in de toekomst te gebruiken. Deze wijziging is 7 keer toegepast op begin- en einddatums in de zibs Vaccinatie, Verrichting, VerpleegkundigeInterventie en Contact.
Van 2017 naar 2020 zal dit niet tot problemen leiden maar van 2020 terug naar 2017 zal het nodig zijn om de eventuele checks aan de ontvangende 2017-kant die een datum in de toekomt niet toestaan te verwijderen of onderdrukken.
De mapping van de 2017 zib OverdrachtGeplandeZorgactiviteit naar de 2020 zibs Vaccinatie, Verrichting, VerpleegkundigeInterventie en Contact is nog niet beschikbaar (volgt indien hier behoefte aan is).

### OTHER INFORMATIONMODEL CHANGE
Er is een klein restgroepje van wijzigingen die niet echt passen bij de bovengenoemde typen. Zo is er een erratum op de zib Brandwond in publicatie 2020 waarbij in een pre-release onbedoeld een zib concept is verwijderd. Deze is weer toegevoegd maar helaas niet zichtbaar op de zibs-wiki. Een andere wijziging betreft een aanvulling op de sub-bouwsteen 'Bereik'. Hier is een invariant toegevoegd in UML-modellering welke misschien van impact kan zijn op een translatie van 2017 naar 2020 maar geen probleem is van 2020 naar 2017.