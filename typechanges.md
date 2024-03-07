# Type changes
 ##	SIMPLE PATCH CHANGE
  
  Hierbij is de tekst in de beschrijving van een zib concept (definitie) of in een beschrijvend onderdeel van de zib (defintie, concept, evidece base, instructions, issues etc) gewijzigd. De wijziging kan een aanvulling zijn, een aanpassing van tekst of tekst in een zib onderdeel waar voorheen nog niets stond. Wanneer de aanpassing alleen de Engelse tekst betreft is dit met [EN] aangegeven. Bij aanpassingen van de Nederlandse tekst is meestal ook de Engelse tekst aangepast waarbij het verstandig is deze ook altijd te vervangen. 
  > [ ] Voor een patch change zal het zib-centrum tabellen beschikbaar maken tussen verschillende baselines om deze wijzgingen geautomatiseerd te laten verlopen.
  >
  > [ ] zibcentrum gaat uitzoeken of deze lijst vanuit Enterprise Architect kan worden gegenereerd. Dan kan dit onderdeel zijn van een publicatie
   
## CONCEPT NAME or CODELIST NAME CHANGED

 Wanneer een concept naam of de naam van een codelijst wordt aangepast kan dit een ‘breaking change’ zijn afhankelijk van de implementatie. Dergelijke wijzigingen zijn waar mogelijk vermeden en alleen doorgevoerd als de impact ervan ten tijde van evaluatie klein leek te zijn. Of de impact van een dergelijke aanpassing daadwerkelijk klein is hangt af van de applicatie waar deze zib is ingebouwd en of en hoe vaak het concept of de codelijst elders in de software wordt aangeroepen. Voor deze aanpassingen is altijd aangegeven of het een Engelse en of Nederlandse name change is. 
 >Voorbeeld 
 >
 >**CONCEPT NAME CHANGED (EN): ::FarmaceuticalProduct-> ::PharmaceuticalProduct**
 
##	TERMINOLOGY MAPPING CONCEPT CHANGE
 
 Terminology mapping is zibs verloopt via DCM::DefinitionCodes tags aan een zib element. Wijzigen van een terminology mapping kan dit verschillende redenen hebben. Soms zijn gebruikte SNOMED CT en LOINC codes deprecated of discourgaged in een nieuwe release, een andere keer wordt een wijziging doorgevoerd door het zib centrum omdat het terminologie centrum een beter concept heeft gevonden die beter past of een fout corrigeert. Tussen 2017 en 2020 zijn veel zibs verrijkt met codes of gelijkgetrokken met gebruikte codes bij een ouder en reeds geimplementeerd informatiemodel (=harmonisatie). Los van de aanleiding of reden van wijziging die in bits kan worden bekeken zijn de wijzigingen op rootconcepten, containers en data elementen van de zib alsvolgt beschreven.

 >
 >Voorbeeld:
 > 
 >**SCT DefintionCode [46973005 Bloeddrukmeting] -> [blank]**  
 >
 >**LOINC DefinitionCode [85354-9 Blood pressure panel with all children optional] -> [55284-4 Blood pressure systolic and diastolic]**

 
 
##	VALUESET CHANGES
 
 Wanneer er wijzigingen zijn in de inhoud van een valueset (dus aan de keuze opties) is het beter om niet te gaan 'patchen' van oud naar nieuw. Naast het feit dat hiermee translaties zeer complex te automatiseren zullen zijn is het ook niet juist om dit te doen omdat oudere instantiaties zijn vastgelegd met de beschikbare codelijsten/valuesets die horen bij de 2017 publicatie.
 Alhoewel het zeker mogelijk is hier per informatiestandaard een andere keuze in te maken stelt Nictiz dringend voor hier van af te zien en als translatie principe en adviseerd houders van informatiestandaarden om bij een translatie usecase van 2017 naar 2020 en terug tijdens een migratie periode van een informatiestandaard die deels bestaat uit FHIR STU3 zibs en andere nl-core resources items naar FHIR R4 zibs bij alle deelnemende actoren van de uitwisseling ervoor te zorgen dat zowel de 2017 als de 2020 codelijsten kunnen worden verwerkt bij zowel de zender als de ontvanger.
 Dit betreft zowel de ondersteuning van in 2020 aangepaste codelijsten die in 2017 al in een zib zaten als nieuwe codelijsten die aan bestaande zibs zijn toegevoegd in de 2020 publicatie (refsets, NHG tabellen, ggz lijsten en overige nieuwe artefacten en codesystemen)
 
 
##	STRUCTURAL INFORMATIONMODEL CHANGES

Wijzigingen aan de structuur van een informatiemodel zijn of minor of major changes. Er zijn een aantal catagorieen binnen dit soort wijzgingen met ieder een andere aanpak bij translatie:

### CARDINALITY CHANGES

Bij zibs als conceptueel informatiemodel worden de kardinaliteiten anders gedefinieerd dan in logische modellen. Hierbij dient te worden opgemerkt dat dit in het verleden niet altijd duidelijk is gemaakt en de definitie van conceptuele kardinaliteit pas later -in 2020- is beschreven en gepubliceerd https://zibs.nl/wiki/Zib_kardinaliteiten . Hierdoor zijn er in het verleden veel wijzigingsverzoeken om deze kardinaliteit te versoepelen, bijvoorbeeld van 1 naar 0..1 afgewezen terwijl andere wijzigingsverzoeken wel tot aanpassing hebben geleid. Hiermee zijn de zib publicaties van 2017 als ook 2020 de regels zoals beschreven op de wiki niet altijd consistent toegepast. Bij de FHIR resources van 2020 is door het HL7 team van nictiz in de profileling guidelines for FHIR R4 hoe wordt omgegaan met de kardinaliteiten van de ZIB in de op de zibs gebaseerde nl-core profiles en informatiestandaarden gebaseerd op zibs.  
Bij een kardinaliteit ‘1’ tussen 2 zib elementen die via een translatie omgezet wordt naar een ‘0..1’ is er in de regel geen probleem. De andere kant op, van -..1 naar 1 zijn er mogelijk wel problemen bij de instantiaties. Een denkbare oplossing kan zijn om in deze gevallen een check te doen en hierbij een foutmelding en/of een (automatische)actie te koppelen aan het voorkomen ervan in datasets. 

 >**ALS [aantal<>1] DAN [Foutmelding] ANDERS source -> target**

Bij een kardinaliteit tussen 2 zib elementen van 0..* naar 0..1 zijn er mogelijk problemen bij translatie. Hier moet worden gecheckt of er meer dan 1 zinvolle data items in de instantiatie zitten. Wanneer dit het geval is dan kan er een foutmelding aan de gebruiker worden getoond en waar nodig zal de gebruiker een keuze worden voorgesteld. Hoe dan ook, in dit scenario zal er waarschijnlijk dataverlies zijn waarbij het aan de houder van de informatiestandaard is om hierin een juiste keuze te maken hoe hier mee om te gaan.

 > **ALS [aantal >1] DAN [Foutmelding] ANDERS source -> target**
  

###	CONCEPT ADDITION or REMOVAL

 Wanneer aan een zib tussen een oudere en een nieuwere versie een extra zib element wordt toegevoegd (of wordt verwijderd) is dit altijd een major change omdat deze wijziging van nieuw naar oud (of andersom) zal resulteren in dataverlies. 
 > voorbeeld:  
 **'Er is een einddatum toegevoegd aan de zib alert'**   
 >**'het boolean concept zwanger is verwijderd'**.  

 Bij een verwijderd concept in een 2020 zib is er sprake van data verlies bij vertalen van 2017 naar 2020 (heen). Bij een toegevoegd concept in 2020 is er sprake van dataverlies bij het vertalen van 2020 naar 2017 (terug). Dit is een niet backward compatible wijziging waarbij zonder aanpassing sprake zal zijn van dataverlies. Hierbij is een mogelijke oplossing denkbaar waarbij data op een andere manier (non-zib) wordt overgestuurd.
 Dit is een niet backward compatible wijzging waarbij zonder aanpassing sprake zal zijn van dataverlies. Hierbij is een mogelijke oplossing denkbaar waarbij data op een andere manier (non-zib) wordt overgestuurd. 

 >voorbeeld:   
 **IF [blank]source->target ELSE [toon en stuur de inhoud van dit data item als vrije tekst naar een 2020 ontvanger]**  
 >  
 >of iets complexer als nodig:  
  **IF [blank] source->target ELSE [toon en stuur de relatie tussen de labuitslag en UitgevoerdDoor::Zorgaanbieder naar een 2017 ontvanger. Maak eventueel een zorgaanbieder instance aan als deze nog niet bestaat ]**

  Dit soort translaties vergt goede analyse waarbij ook de reeds geinstantieerde data aan zowel de kant van de sturende als ontvangende/vragende applicatie van een informatiestandaard moeten worden bestudeerd. 


###	CHANGE TO SUB HCIM
In publicatie 2020 is een nieuwe sub-bouwsteen voor anatomische locatie gepubliceerd omdat de 2 concepten anatomische locatie en lateraliteit in veel zibs voorkwamen. Hierbij zijn de 2 concepten voor locatie en lateraliteit gewijzigd naar 1 verwijzing naar de nieuwe zib. In de 2020 zib staat er dan bijvoorbeeld VerrichtingAnatomischeLocatie::AnatomischeLocatie. Alhoewel dit wat verwarrend lijkt zal dit voor translatie heen en terug waarschijnlijk een eenvoudige wijzing zijn. De inhoud van de codelijsten uit 2017 zijn namelijk bij deze wijzigingen gelijk gebleven in 2017 waardoor de translatie bestaat uit simpel weg de geinstantieerde waarde van de een over zetten in de andere.

### DATA TYPE CHANGE
De enige data type change die voorkomt tussen 2017 en 2020 gaat om het wijzigen van het datatype van een aantal codelijsten. Deze waren in 2017 van het type CO. Dit was echter een fout want de valuesets welke zijn uitgegeven waren in feite toch van het type CD. Een translatie is hierdoor simpel en betreft alleen de defintie en niet de data of de structuur van het informatiemodel.

### DATETIME IN FUTURE ALLOWED
In de 2020 publicatie is de zib OverdrachtGeplandeZorgactiviteit komen te vervallen. Om alle type zorgactiviteiten in deze zib toch te kunnen plannen zijn voor deze zibs in 2020 is het constraint op de begin- en einddatums opgeheven waardoor het mogelijk is om ook een datum in de toekomst hier op te nemen. Deze wijziging is 7 x toegepast op begin- en einddatums in de zibs Vaccinatie, Verrichting, VerpleegkundigeInterventie en Contact.
Van 2017 naar 2020 zal dit niet tot problemen leiden maar van 2020 terug naar 2017 zal het nodig zijn om de eventuele checks aan de ontvangende 2017 kant die een datum in de toekomt niet toestaan te verwijderen of onderdrukken.
De mapping van de 2017 zib OverdrachtGeplandeZorgactiviteit naar de 2020 zibs Vaccinatie, Verrichting, VerpleegkundigeInterventie en Contact is nog niet beschikbaar [volgt indien hier behoefte aan is]. 


### OTHER INFORMATIONMODEL CHANGE
Er is een klein restgroepje van wijzigingen die niet echt passen bij de bovengenoemde typen. Zo is er een erratum op de zib Brandwond in publicatie 2020 waarbij in een pre-release onbedoeld een zib concept is verwijderd. Deze is weer toegevoegd maar helaas niet zichtbaar op de zibs wiki. Een andere wijzing betreft een aanvulling op de sub bouwsteen 'Bereik'. Hier is een invariant toegevoegd in UML modellering welke misschien van impact kan zijn op een translatie van 2017 naar 2020 maar geen probleem is van 2020 naar 2017.