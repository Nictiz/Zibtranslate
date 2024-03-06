 # Type changes

 ##	SIMPLE PATCH CHANGE
  
  Hierbij is de tekst in de beschrijving van een zib concept (definitie) of in een beschrijvend onderdeel van de zib (definitie, concept, evidence base, instructions, issues etc.) gewijzigd. De wijziging kan een aanvulling zijn, een aanpassing van tekst of tekst in een zib onderdeel waar voorheen nog niets stond. Wanneer de aanpassing alleen de Engelse tekst betreft is dit met [EN] aangegeven. Bij aanpassingen van de Nederlandse tekst is meestal ook de Engelse tekst aangepast waarbij het verstandig is deze ook altijd te vervangen.

  > Voor een patch change zal het zib-centrum tabellen beschikbaar maken tussen verschillende baselines om deze wijzgingen geautomatiseerd te laten verlopen.

  > Het zibcentrum gaat uitzoeken of deze lijst vanuit Entrerprise Architect kan worden gegenereerd. Dan kan dit onderdeel zijn van een publicatie
   
## CONCEPT NAME or CODELIST NAME CHANGED

 Wanneer een concept naam of de naam van een codelijst wordt aangepast kan dit een 'breaking change' zijn afhankelijk van de implementatie. Dergelijke wijzigingen zijn waar mogelijk vermeden en alleen doorgevoerd als de impact ervan ten tijde van evaluatie klein leek te zijn. Of de impact van een dergelijke aanpassing daadwerkelijk klein is hangt af van de applicatie waar deze zib is ingebouwd en of en hoe vaak het concept of de codelijst elders in de software wordt aangeroepen. Voor deze aanpassingen is altijd aangegeven of het een Engelse en/of Nederlandse wijziging van de naam is.
 
 >Voorbeeld 
 >
 >**CONCEPT NAME CHANGED (EN): ::FarmaceuticalProduct-> ::PharmaceuticalProduct**
 
##	TERMINOLOGY MAPPING CONCEPT CHANGE
 
 Terminologiemapping in zibs verloopt via DCM::DefinitionCodes tags aan een zib element. Wijzigen van een terminologiemapping kan dit verschillende redenen hebben. Soms zijn gebruikte SNOMED CT en LOINC codes deprecated of discouraged in een nieuwe release, een andere keer wordt een wijziging doorgevoerd door het zib centrum omdat het terminologie centrum een beter concept heeft gevonden dat beter past of een fout gecorrigeerd. Tussen 2017 en 2020 zijn veel zibs verrijkt met codes of gelijkgetrokken met gebruikte codes bij een reeds geïmplementeerd informatiemodel (=harmonisatie). Los van de aanleiding of reden van wijziging (die in BITS kan worden bekeken) zijn de wijzigingen op rootconcepten, containers en data elementen van de zib als volgt beschreven.

 >
 >Voorbeeld:
 > 
 >**SCT DefintionCode [46973005 Bloeddrukmeting] -> [blank]**  
 >
 >**LOINC DefinitionCode [85354-9 Blood pressure panel with all children optional] -> [55284-4 Blood pressure systolic and diastolic]**


##	VALUESET CHANGES
 
 Wanneer er wijzigingen zijn in de inhoud van een valueset (dus aan de waarden) is het beter om niet te gaan 'patchen' van oud naar nieuw. Naast het feit dat hiermee translaties zeer complex te automatiseren zullen zijn is het ook niet juist om dit te doen omdat oudere instantiaties zijn vastgelegd met de beschikbare codelijsten/valuesets die horen bij de oudere publicatie. 
 
 Alhoewel het zeker mogelijk is hier per informatiestandaard een andere keuze in te maken stelt Nictiz dringend voor hier van af te zien en als translatie principe en adviseert houders van informatiestandaarden om bij een translatie usecase van 2017 naar 2020 en terug tijdens een migratie periode van een informatiestandaard die deels bestaat uit FHIR STU3 zibs en andere nl-core resources items naar FHIR R4 zibs bij alle deelnemende actoren van de uitwisseling ervoor te zorgen dat zowel de 2017 als de 2020 codelijsten kunnen worden verwerkt bij zowel de zender als de ontvanger. 

 Dit betreft zowel de ondersteuning van in 2020 aangepaste codelijsten die in 2017 al in een zib zaten als nieuwe codelijsten die aan bestaande zibs zijn toegevoegd in de 2020 publicatie (refsets, NHG tabellen, ggz lijsten en overige nieuwe artefacten en codesystemen)

 > Leveranciers geven aan dat een dergelijke aanpak aanzienlijk meer kans maakt op consistente en herbruikbare translaties aangezien de aanpassingen in hun systeem vervolgens voor meerdere implementaties gebruikt kunnen worden.

## STRUCTURAL INFORMATIONMODEL CHANGE

Wijzigingen aan de structuur van een informatiemodel zijn of minor of major changes. Er zijn een aantal catagorieen binnen dit soort wijzgingen met ieder een andere aanpak bij translatie:

### CARDINALITY CHANGES

 Bij zibs als conceptueel informatiemodel worden de kardinaliteiten anders gedefinieerd dan in logische modellen. Hierbij dient te worden opgemerkt dat dit in het verleden niet altijd duidelijk is gemaakt en de definitie van conceptuele kardinaliteit pas later -in 2020 - is beschreven en gepubliceerd https://zibs.nl/wiki/Zib_kardinaliteiten. Hierdoor zijn er in het verleden veel wijzigingsverzoeken om deze kardinaliteit te versoepelen, bijvoorbeeld van 1 naar 0..1, afgewezen terwijl andere wijzigingsverzoeken wel tot aanpassing hebben geleid. Hiermee zijn de zib publicaties van 2017 evenals 2020 de regels zoals beschreven op de wiki niet altijd consistent toegepast.
 Bij de FHIR resources van 2020 is door het HL7 team van Nictiz in de profiling guidelines voor FHIR R4 beschreven hoe wordt omgegaan met de kardinaliteiten in de op zibs gebaseerde nl-core profiles en informatiestandaarden.

* Bij een kardinaliteit ‘1’ tussen 2 zib elementen die via een translatie omgezet wordt naar een ‘0..1’ is er in de regel geen probleem. De andere kant op, van 0..1 naar 1 zijn er mogelijk wel problemen bij de instantiaties. 

> Voorbeeld:
>
> ALS [aantal<>1] DAN [Foutmelding] ANDERS source -> target

* Bij een wijziging van de kardinaliteit van 0..* naar 0..1 zijn er mogelijk problemen bij de translatie. Hier moet worden gecontroleerd of er meer dan 1 zinvolle data items in de instantiatie zitten. Wanneer dit het geval is dan dient er een foutmelding aan de gebruiker te worden getoond en waar nodig zal de gebruiker een keuze worden voorgesteld. Hoe dan ook, in dit scenario zal er dataverlies zal zijn.

> Voorbeeld:
>
> ALS [aantal>1] DAN [Foutmelding] ANDERS source -> target
  
###	CONCEPT ADDITION or REMOVAL

 Wanneer aan een zib tussen een oudere en een nieuwere versie een extra zib element wordt toegevoegd is dit altijd een major change omdat deze wijziging van nieuw terug naar oud zal resulteren in dataverlies.

 *	CONCEPT POINTER ADDITION (naar andere zib)
 *	CONCEPT POINTER REMOVAL (naar andere zib)
 *	CHANGE TO SUB HCIM (komt vaak voor, naar o.a. anatomische locatie)
 *	DATA TYPE CHANGE
 