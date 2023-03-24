# kaartlagen

### Standaard zichtbaarheid kaartlagen

In de configuratie van de applicatie kan (door het ontwikkelteam) worden ingesteld welke kaartlagen standaard zichtbaar zijn. Momenteel is standaard zichtbaarheid alleen ingesteld voor de WIS-laag.

### Arcgis server Kaartlagen in kaartbeeld van ICMS:

| Naam                   | type | legenda                                                                                                         |
| ---------------------- | ---- | --------------------------------------------------------------------------------------------------------------- |
| Hectometrering         | punt | https://gisservices.noord-holland.nl/ags/rest/services/extern/pnh\_ic\_weghectometrering/MapServer/Legend       |
| IM wegen PNH           | lijn | https://gisservices.noord-holland.nl/ags/rest/services/extern/pnh\_ic\_wegen\_pnh/MapServer/Legend              |
| IM wegen RWS           | lijn | https://gisservices.noord-holland.nl/ags/rest/services/extern/pnh\_ic\_wegen\_rws/MapServer/Legend              |
| Wegnummering           | punt | https://gisservices.noord-holland.nl/ags/rest/services/extern/pnh\_ic\_wegnummering/MapServer/Legend            |
| OV verzorgingsgebieden | vlak | https://gisservices.noord-holland.nl/ags/rest/services/extern/pnh\_ic\_ov\_verzorgingsgebieden/MapServer/Legend |
| Gemeentegrenzen        | vlak | https://gisservices.noord-holland.nl/ags/rest/services/extern/pnh\_ic\_gemeentegrenzen/MapServer/Legend         |
| Waterschappen          | vlak | https://gisservices.noord-holland.nl/ags/rest/services/extern/pnh\_ic\_waterschappen/MapServer/Legend           |
| Gebiedscontractregio's | vlak | https://gisservices.noord-holland.nl/ags/rest/services/extern/pnh\_ic\_gebiedscontractregios/MapServer/Legend   |
| Veiligheidsregio's     | vlak | https://gisservices.noord-holland.nl/ags/rest/services/extern/pnh\_ic\_veiligheidsregios/MapServer/Legend       |

De displayvolgorde is zo dat op de kaart de vlakken 'onderop' liggen, daarboven de lijnen, en daarboven de punten.

Sommige lagen zoals Weghectometrering en Wegnummering worden alleen weergegeven als je inzoomt

### Be-mobile Kaartlagen in kaartbeeld van ICMS:

| Naam                      | symbool |
| ------------------------- | ------- |
| stilstaand voertuig       |         |
| ongeval                   |         |
| obstakel                  |         |
| werkzaamheden (punt)      |         |
| werkzaamheden (lijn)      |         |
| verkeersvertraging (file) |         |
