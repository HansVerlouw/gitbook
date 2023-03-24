# release\_notes

## Release notes

### Release 1.92

Release date: _upcoming_

#### Features

* **Prio taken:** De volgende twee taken zijn verlaagd van prio taak naar niet prio taak:
  * Bel waterschap om de details van het incident te bespreken?
  * Aanmelden bij Servicepunt?\
    De volgende twee taken zijn verhoogd naar prio taak:
  * Einde inzet WIS; geef aan als incident voor WVL is afgerond
  * Extra WIS inschakelen (formtaak)\
    _Opmerking_: alleen de stakeholder ziet prio taken vetgedrukt.
* **PDF rapportage:** De PDF rapportage (intern of extern) wordt nu aangemaakt via het nieuwe Update tabblad, formulier: "PDF rapportage aanmaken" (zie wiki: PDF rapportage). De taak PD rapportage genereren wordt niet meer gedeployed.
* **Incident afsluiten:** Het is niet meer mogelijk om een incident af te sluiten via de prullenbak knop. Dit moet nu altijd via een taak gebeuren: _Kan het dossier worden afgesloten?_ of _Sluit incident af_.
* **Update tabblad:** Er is een nieuw tabblad bijgekomen, waarbij de gebruiker, na het verwerken van de intake, verdere informatie kan geven over het incident. (zie incidenttabbladen -> update)
* **Overige info verwijderen:** In het intakeformulier zijn de velden voor overige info verwijderd bij alle subformulieren, behalve bij 'Beschikbaarheid infrastructuur' en 'Overige info'. Bij 'Overige info' is dit veld verplicht. Bij het taakformulier behorende bij de taak 'Inventarisatie schade areaal' verschijnt de toelichting als de optie 'Ja' is gekozen. Het veld is dan verplicht.

#### Fixes

#### Known issues

* **OV-bedrijf alarmeren:** De verschillende ov-bedrijf alarmeertaken worden niet naast elkaar weergegeven na verwerken in de takenlijst.
* **OV-bedrijf alarmeren:** De Bel OV-bedrijf taken kunnen dubbel worden gedeployed op een verwerkt incident als de waarde van InfrasctructuurStatus meerdere keren verandert naar Hinder of Afgesloten.
* **Update tabblad:** Op dit moment hebben nog niet alle formulieren een opslaan knop (Beschikbaarheid infrastructuur en overige informatie). Hierdoor worden logboekregels nog niet goed weggeschreven voor deze formulieren. Dit wordt opgelost bij de volgende product update.
* **Update tabblad:** Het prognose formulier werkt nog niet goed als formulier in het update tabblad. Daarom is er voor gekozen om het als los tabblad te houden.
* **Update tabblad:** De WVL heeft ook toegang tot het update tabblad, zodat de WVL de interne en externe rapportages kan downloaden over het incident.

### Release 1.91

Release date: 2019-10-02

#### Features

* **MIR3 gebruikers:** er is een account aangemaakt om gebruikersgegevens te configureren voor productieomgeving. Zie uitleg onder _MIR3 configuratie_
* **Meldingen importeren** : Het is mogelijk om nieuwe incidenten aan te maken via de import endpoint in icms-webapi. Zie wiki > _Meldingen importeren_ voor meer details
* **Overige info verwijderen:** In het intakeformulier zijn de velden voor overige info verwijderd bij alle subformulieren, behalve bij 'Beschikbaarheid infrastructuur' en 'Overige info'. Bij 'Overige info' is dit veld verplicht. Bij het taakformulier behorende bij de taak 'Inventarisatie schade areaal' verschijnt de toelichting als de optie 'Ja' is gekozen. Het veld is dan verplicht.

#### Fixes

* **MIR3 alarmeren:** Mir3 probleem door een verlopen apikey van initiator opgelost.
* **Extra wis:** Vanaf nu is de status van de rol Extra Wis ook te zien op het totaalbeeld.

### Release 1.9

Release date: 14-08-2019

#### Features

* **Kaart:** symbolen op het informatiepaneel zijn aangepast.

#### Fixes

* **Nieuwe melding:** 1ste keer na het inloggen wordt nu bij aanmaken incident de Intake tab default geselecteerd
* **Selecteren op de kaart:** "Selecteer incident intake" link is verwijderd van het default incident info panel form.

## Release notes

### Release 1.8

Release date: 29-07-2019

#### Features

* **Extra WIS inschakelen** : Er is een mogelijkheid toegevoegd voor de WIS om een extra WIS in te schakelen. Zie _>Taken > WIS > Extra WIS inschakelen_ voor meer informatie
* **IEP-lijst** : de lijst van IEPs is nu beschikbaar op de wiki: https://apps.geodan.nl/icms/pnh/icms-webapi/api/document/doc/customer/iep-lijst-pnh.html
* **PDF rapportage** :Voor de WIS en WVL is de mogelijkheid beschikbaar om een rapportage te downloaden van het betreffende incident. Bij het verwerken van een incident verschijnt er de taak "PDF rapportage genereren". Hierbij kan er een PDF worden gedownload met een overzicht van het betreffende incident. Zie wiki > _PDF rapportage_ voor meer details
* **Locatievelden** : De locatievelden worden getoond in een nieuw formulier onder de locatie. Afhankelijk of de huidige incident locatie in de bijbehorende polygonen valt: Calamiteitenaannemer, waterschap. OV bedrijf: zes verschillende velden met naam ovbedrijf. Als de locatie van het incident verandert, dan worden deze velden opnieuw berekend&#x20;

#### Fixes

* **Locatie zoeken** : De foutmelding bij zoeken op locaties voor gebruikers die inloggen via AzureAD is opgelost.
* **Emailbericht naar WIS** : WVL gebruikersnaam (emailadres) is toegevoegd. Als overige informatie niet gevuld is, ziet de gebruiker een lege string ipv 'undefined'.
* **TrafficFleet**: de URL van de TrafficFleet API is gewijzigd naar HTTPS

### Release 1.7

Release date: 17-07-2019

#### Features

* **Inlogsessie**: er worden waarschuwingen getoond 2 uur en daarna 5 minuten voordat de sessie verlopen is zodat de gebruiker opnieuw kan inloggen
* **Verbindingsstatus** : het symbool van de verbindingsstatus is veranderd:&#x20;
* **Info panel** : Het is nu mogelijk om het informatie over kaartlagen op de informatiepaneel te zien door op een positie op de kaart te klikken.&#x20;

#### Known issues

* **Nieuwe melding**: 1ste keer na het inloggen wordt bij aanmaken incident de Taken tab default geselecteerd i.p.v. Intake

### Release 1.6

Release date: _21-06-2019_

#### Features

* **Nieuwe Melding** : Bij het aanmaken van een nieuwe melding opent deze automatisch in het tabblad 'Intake', ook wanneer daarvoor een ander tabblad was geselecteerd.
* **Weergave afgesloten incident**: Bij de weergave van een afgesloten incident worden de formulieren standaard in uitgeklapte staat getoond.
* **Uitloggen**: Een gebruiker kan nu uitloggen uit de applicatie via de link 'Uitloggen' in het gebruikersmenu rechtsboven in het scherm.
* **Kaart** : Incidenten worden nu bovenaan alle custom lagen weergegeven.
* **Intake** : De stijl van de knoppen "wijzig locatie op de kaart" en "zoom naar" is aangepast:\
  &#x20;Bovendien werkt de rechterknop 'Wijzig locatie op de kaart' nu ook al zonder eerst op wijzig locatie te drukken.

#### Fixes

* **Logboek** : De prefix die gebruikt wordt bij de logberichten in de categorie 'Prognose' in het logboek is nu Nederlandstalig (ipv Engels), nl. 'Prognose is nu ..'.

### Release 1.5

Release date: _4-06-2019_

#### Features

* **Incidentgroepen** : De opklapbare incidentgroepen 'Nieuwe meldingen' en 'In Behandeling' worden nu standaard getoond in het overzicht aan de linkerzijde\


#### Fixes

* **WIS alarmeren**: De 'bevestigen'-links zijn de uit de ICMS-alarmeer-e-mails verwijderd.

### 1.4

Release date: _21-5-2019_

#### Features

* **Kaart**: Het standaard zoomniveau van de kaart is iets hoger, en de kaart is gecentreerd op Noord-Holland
* **Kaartlagen**: De kaartlagen wegnummering en WIS zijn nu standaard aangevinkt
* **Kaartlagen**: De verkeersinformatielagen van Be-Mobile zijn geconfigureerd in de kaart. In de legenda zijn deze lagen te vinden onder het kopje 'Thematische lagen'

#### Fixes

* **Verplichte Locatie**: Het locatieveld wordt nu in oranje omrand wanneer deze niet ingevuld is, aangezien het een verplicht veld is
* **Incident IDs overlappen op de kaart**: Alleen main incident ID is nu zichtbaar op de kaart

### 1.3

Release date: _1-5-2019_

#### Features

* **Layer manager**: De kleuren van de layermanager zijn aangepast naar licht blauw
* **Extra gegevens bij incident popup**: Bij het klikken van een incident op de kaart worden de volgende gegevens weergegeven in tabelform: Incidentype, Locatie, Tijd melding, Prognose, WISnaam\


#### Fixes

* **Velden intake bij nieuw incident niet altijd gevuld**: Standaard waarden van velden zouden nu altijd worden gezet
* **Taken**: Alle vereiste taken zouden nu altijd beschikbaar moeten zijn
* **Verwerken**: De volgende onterechte waarschuwing bij verwerken is opgelost: "Incident kan nog niet worden verwerkt: Er is nog een nieuw incident in aanmaak". Verwerkt knop onterecht uitgegrijsd is opgelost
* **Iconen per incidenttype**: incidentsymbool in de incidentenlijst wordt nu geupdated zonder verversen.
* **Incidenten in 'Overig' afsluiten**: Incidenten in 'Overig' afgesloten.
* **Wegnummer op Totaalbeeld**: Wegnummer, hectometerpaal en wegzijde zijn nu zichtbaar op het Totaalbeeld
* **Prognose afgesloten incidenten**:  prognose wijzigen is niet meer mogelijk nadat het incident is afgesloten

### 1.2

Release date: _17-4-2019_

#### Features

* **Locatie incident**: Afkorting a: (a;) is toegevoegd om adressen te zoeken bij Locatie incident.\

* **Formulier Wateroverlast**: Keuzemogelijkheden in formulier Wateroverlast aangepast naar: 'Binnen een tunnel', 'Buiten een tunnel', 'Onbekend'
* **Formulier Verontreiniging wegdek**: Bij "verontreiniging wegdek" verschijnt een nieuw formulier waarop het type verontreiniging van het wegdek kan worden ingevuld (modder/olie/overig/onbekend) en een toelichting kan worden gegeven.
* **Formulier Installatie in storing**: Bij "installatie in storing" verschijnt een nieuw formulier waarop soort storing kan worden ingevuld (Brug | OVL/VRI | Busbaan | Overige installatie | Onbekend; Onbekend is de default waarde) en een toelichting kan worden gegeven.

#### Fixes

* **Dubbele taken**: Door een technische aanpassing zouden dubbele taken nu niet meer moeten plaatsvinden
* **'Kan het dossier worden afgesloten' taak**: de taak verdwijnt nu na het verwerken van de incident
* **Geen taken**: het niet verschijnen van taken na verwerken is gefixed
* **Formulier Wateroverlast**: de vraag is veranderd in: "Betreft het overlast binnen de tunnel?"
* **Incident blijft na verwerken in 'Nieuwe meldingen' staan**: na het verwerken wordt het incident naar 'In behandeling' verplaatst
* **Disablen intakevelden na verwerken**: wanneer een incident verwerkt is, worden vanaf nu de intake formulieren gedisabled. Daardoor is het niet meer mogelijk voor de wegverkeersleider om na verwerken informatie van de intake te veranderen. Een uitzondering is het veld "Overige informatie", deze blijft aanpasbaar ook na verwerking.
* **Gesloten incidenten**: gesloten incidenten van de laatste 3 dagen zijn nu zichtbaar

#### Known issues

* **Iconen per incidenttype**: Soms blijft het incidentsymbool in de incidentenlijst een vraagteken tot verversen. Dit wordt in de volgende release opgelost.
* **Velden intake bij nieuw incident niet altijd gevuld**: Dit wordt in de volgende release opgelost.

### 1.1

Release date: _8-4-2019_

#### Features

* **Incident popup**: De incident popup is verplaatst naar de panel aan de linkerzijde (onder de layer manager).&#x20;
* **Zichtbaarheid trafficfleet lagen**: Deze lagen kunnen nu standaard zichtbaar zijn als de webapplicatie start. Dit is voorlopig ingesteld voor de TrafficFleet testomgeving.
* **Volgorde en prioritering van taken**: De volgorde van het verschijnen van taken is gewijzigd, om meer overeen te komen met de gewenste volgorde. Daarnaast is er prioritering aan de taken meegegeven, en zijn niet alle taken meer standaard "prio", te zien aan de blauwe rand links van een taak. Een taak is overigens alleen een prio taak voor degene aan wie de taak toegewezen is.
* **Voorwaarde IM-weg bij LCM/CMV-taak**: De taken voor LCM en CMV worden nu alleen gezet als het incident op een IM-weg heeft plaatsgevonden, of wanneer dit onbekend is. Als het incident niet op een IM-weg is worden de taken voor LCM en CMV niet getoond.
* **Configuratie verplichte velden intake-formulier**: Het is nu mogelijk om verplichte velden te configureren voor het intakeformulier. Deze velden zijn nu geconfigureerd volgens de specicaties in het stroomschema.

#### Fixes

* **Waterschap en telefoonnummer**: De naam en het telefoonnummer van het waterschap worden nu -op basis van de incidentlocatie- automatisch ingevuld in de taak 'Bel waterschap...':\

* **WIS alarmeren**: Het gebeurde soms dat een WIS gealarmeerd werd maar geen berichten ontving. Dit probleem is opgelost.
* **Iconen per incidenttype**: Soms bleef het incidentsymbool in de incidentenlijst een vraagteken en was het nodig te verversen. Dit is opgelost.
* **Tijd/datum wordt niet altijd automatisch gevuld**: In het meldingformulier werd de tijd/datum van de melding niet altijd automatisch ingevuld. Dit is opgelost.
* **Mogelijk om incident te verwerken zonder een enkel gegeven in te vullen**: De verplichte velden voor het intakeformulier zijn ingesteld (waaronder de locatie). Hierdoor is het niet meer mogelijk een niet ingevulde intake te verwerken.
* **OVD taak verschijnt dubbel**: Dit is opgelost.
* **Eenzijdig staat onterecht als default**: Dit is opgelost. Het subformulier Ongeval toont nu de standaardwaarde 'Onbekend' bij de vraag 'Wat voor een ongeval?'.

#### Known issues

* **Alarmeren WIS**: WIS'en worden soms ten onrechte twee keer gealarmeerd. We hebben een verbetering doorgevoerd waardoor dit minder vaak gebeurt, maar het kan nog niet helemaal uitgesloten worden.
* **Incidenten kunnen niet afgesloten worden**: Heel af en toe verschijnt de taak waarmee een incident afgesloten kan worden niet.
* **Volgorde van taken**: Taken die toegevoegd worden via een andere taak worden onderaan de takenlijst bijgeplaatst (en dus -nog- niet op de gewenste positie). Dit zal in een latere oplevering gecorrigeerd worden.
* **Logging vanuit Rollen ter plaatse-formulier**: Vanuit dit formulier (gebruikt in de taken 'De gealarmeerde WIS'en hebben geweigerd of zijn niet beschikbaar, alarmeer handmatig een andere WIS', 'OVD: leg bevindingen vast', 'Geef uw verwachte tijd ter plaatse aan' en 'Geef uw tijd ter plaatse aan') worden na iedere wijziging ALLE velden met een waarde gelogd in het logboek, i.p.v. alleen de velden die gewijzigd zijn.
* **WIS kaartlaag**: Heel af en toe wordt de WIS status in de kaart niet geüpdatet ook al is dit wel goed doorgevoerd in trafficFleet. Dit komt omdat de Sensorbroker onderdeel een herstart nodig heeft. Dit wordt verbeterd in het basisproduct.
* **Verwerkknop blijf uitgegrijsd**: Soms wordt de 'Verwerk incident' knop in het meldingformulier niet actief, pas na herladen van het incident wordt de knop actief. Dit wordt in een volgende versie opgelost.

### 1.0

Release date: _25-3-2019_

#### 1.0 Features (voor meer uitleg kijk in het bijbehorende wiki-artikel)

* **locatie incident**: De mapservice https://gisservices.noord-holland.nl/ags/rest/services/extern/pnh\_ic\_weghectometrering/MapServer/0/query wordt nu gebruikt als standaard locator. Er hoeft in het veld 'Locatie incident' nu geen prefix meer gebruikt te worden.
* **configuratie PNH kaartlagen**: nieuwe kaartlagen zijn toegevoegd aan het kaartbeeld van ICMS
* **milieuvervuiling inventariseren**: bij elk incident wordt voor de Weginspecteur de taak '_Inventarisatie milieuvervuiling_' klaargezet
* **schade aan het areaal**: taak en taakformulier voor schade areaal toegevoegd voor WIS. Bij kiezen voor "OVL/VRI" wordt een taak voor de WVL gestart "Aanmelden bij Servicepunt?".
* **voertuiginventarisatie bijwerken**: bij het verwerken van de incidenttypes Ongeval, Pechgeval en Verlaten Voertuig is er voor de Weginspecteur een taak beschikbaar om de inventarisatie van betrokken voertuigen toe te voegen.
* **berging coördineren**: In het geval van een incident van het type Ongeval, Pechgeval, of Verlaten voertuig wordt de taak '_Bel LCM_' neergezet voor WVL. Als het een incident is waarin een voertuig zwaarder dan 3500kg is betrokken, dan wordt ook de taak '_Bel CMV_' neergezet.
* **VOA-team ter plaatse komt**: Bij verwerking van een incident verschijnt bij het incidenttype 'ongeval' voor de WIS een taak met omschrijving _Komt er een VOA-team ter plaatse?_.
* **opmaak summaryform incidenttree**: Het 'meldingkaartje' dat voor elk incident weergegeven wordt in de lijst aan de linkerzijde van het scherm is aangepast naar de wensen van PNH. Dit bevat nu de volgende informatie:
  * De naam van het incidenttype;
  * Het logo van de bijbehorende incidentcategorie;
  * De locatie van het incident bestaande uit: wegnummer, hectometerpaal en wegzijde/dvk letter;
  * De tijd en datum van de melding (datum wordt weggelaten als het een melding van de huidige dag betreft;
  * Het aantal openstaande (prio-)taken;
  * Aanduiding WIS indien een WIS geaccepteerd heeft via MIR3, of handmatig is toegewezen door de WVL
  * Aanduiding Geen WIS als er via de automatische alermering geen beschikbare WIS'en zijn, of alle beschikbare WIS'en geweigerd hebben. Als er geen van beide indicaties 'WIS' of 'Geen WIS' te zien is betekent dit dat de automatische alarmering van de WIS nog gaande is.
* **configuratie iconen per incidenttype**: De correcte incidentsymbolen worden nu ook getoond in de incidentlijst in de webclient.
* **schatting aankomsttijd WIS registreren (ETA)**: De verwachte aankomsttijd van de WIS wordt automatisch ingevuld op het totaalbeeld nadat de WIS geaccepteerd heeft.
* **WVL wil handmatig een WIS toevoegen aan het incident**: Wanneer alle WIS'en geweigerd hebben in de automatische alarmering (of er geen WIS'en beschikbaar zijn) kan de WVL handmatig een WIS aan het incident koppelen via het taakformulier: _De gealarmeerde WIS'en hebben geweigerd of zijn niet beschikbaar_.
* **OVD-er erbij vragen**: WIS ziet altijd een taak "Incident opschalen? Schakel OVD in".
* **OVD taak om bevindingen en acties vast te leggen**: WIS ziet een taak “OVD: leg bevindingen vast” wanneer de OVD is ingeschakeld
* **VCNL kunnen bellen**: Als de status beschikbaarheid infrastructuur wijzigt van 'onbekend' of 'open' naar 'hinder' of 'afgesloten', ziet WVL een taak "Bel VCNL om de details van het incident te bespreken?"

#### 1.0 Fixes

* **prognose flow**: De prognosetaken met formulier zijn vervangen door één afvinktaak met de volgende tekst: 'Wijzig de initiële prognose in het tabblad: Prognose'. Het wijzigen van de prognose kan alleen nog maar gedaan worden in dit tabblad.
* **geen beschikbare WIS**: 'Belangrijke Wijziging' wordt nu ook in het geval van geen beschikbare WIS getoond of als de enige beschikbare WIS weigert.

#### 1.0 Known issues

* **iconen per incidenttype**: Soms blijft het symbool een vraagteken en is het nodig te verversen.
* **milieuvervuiling inventariseren**: In een volgende oplevering zal in de omschrijving van deze taak automatisch de naam en het telefoonnummer ingevuld worden van het waterschap dat het bevoegd gezag is voor de incidentlocatie.
* **incident afsluiten voor verwerken**: De taak Taak '_Kan het dossier worden afgesloten_' verdwijnt niet altijd na verwerken. Dit is verbeterd maar treedt helaas nog steeds soms op. Hiervoor is er een upgrade van het basisproduct nodig.
* **logging vanuit Rollen ter plaatse-formulier**: Vanuit dit formulier (gebruikt in de taken 'De gealarmeerde WIS'en hebben geweigerd of zijn niet beschikbaar, alarmeer handmatig een andere WIS' ,'OVD: leg bevindingen vast' 'Geef uw verwachte tijd ter plaatse aan' en 'Geef uw tijd ter plaatse aan') worden na iedere wijziging ALLE velden met een waarde gelogd in het logboek, ipv. alleen de velden die gewijzigd zijn.
* **wis kaartlaag**: Heel af en toe wordt de WIS status in de kaart niet geüpdatet ook al is dit wel goed doorgevoerd in trafficFleet. Dit komt omdat de Sensorbroker onderdeel een herstart nodig heeft. Dit wordt verbeterd in het basisproduct.
* **wis alarmeren**: Er gebeurt soms dat een WIS gealarmeerd wordt maar ontvangt geen berichten. Dit probleem wordt nu geanalyseerd en zo snel mogelijk opgelost.
