# meldingen importeren

## Meldingen importeren

Het is mogelijk om nieuwe incidenten aan te maken via de _Import_ endpoint van icms-webapi. Dit is een POST request met als Body een JSON string die een array van incidenten bevat met een minimaal aantal gegevens.

Om de Import endpoint te kunnen aanroepen zijn er twee headers vereist:

* Authorization header (basic authentication): Dit bevat de geodanMaps gebruikersnaam en wachtwoord (gescheiden door een puntcomma) en versleuteld as base64 string.
* Token (jwt string met een geldigheid van 24 uur). Dit kan worden opgehaald via de token endpoint van de multi-tenant icms-webapi

### Voorbeeld JSON for the import (array)

```json
[
    {
        "properties": {
            "name": "Pechgeval",
            "incidentTypeName": "Intake",
            "severity": "Normal"
        },
        "ieps": {
            "IncidentSource": "Facman"
        },
        "childIncidents": [
            {
                "properties": {
                    "name": "Pechgeval",
                    "incidentTypeName": "Pechgeval",
                    "severity": "Normal"
                },
                "ieps": {
                    "ConceptLocation": "A9 67.1 Li"
                }
            }
        ]
    }
]
```

## Beschrijving bericht

### Hoofdincident

#### Properties:

* **name**: De naam van het incident (gelijk aan het incidentTypeName van het sub)
* **incidentTypeName**: Altijd "Intake" voor productie en "DEV\_Intake" voor test/ontwikkel
* **severity**: Een van de waarden: "Low", "Normal", "Medium", "High", "Urgent"
* **x**: x-coordinaat (WGS84), mag leeg blijven
* **y**: y-coordinaat (WGS84), mag leeg blijven

#### Ieps

* **IncidentSource**: altijd "Facman"
* **DateTimeIncident**: datumtijd incident in Zulu tijd, ISO 8601 formaat

De informatie van belang voor het terugbericht naar Facman:

* **FacmanAccountCode**
* **FacmanEvent**

Indien bekend informatie over de melder:

* **NotifierLabel**: "Politie", "Be-mobile", "RWS", "WIS", "Overig"
* **NotifierName**: De naam van de melder

### Subincident

#### Properties

* **name**: De naam van het incident (Gelijk aan het incidentTypeName van het sub)
* **incidentTypeName**: Een van de volgende waarden: "Ongeval", "Pechgeval", "Wateroverlast", "Hinder in de omgeving", "Installatie in storing", "Obstakel op de weg", "Verlaten voertuig", "Verontreiniging wegdek"
* **severity**: Een van de waarden: "Low", "Normal", "Medium", "High", "Urgent" (gelijk aan het hoofdincident)
* **x**: mag leeg blijven
* **y**: mag leeg blijven

#### Ieps

* **ConceptLocation**: spatiegescheiden informatie over de locatie: wegnummer, kilometrering, wegzijde (indien bekend)
* Zie [ieplijst](http://docs.geodan.nl/icms-docs/pnh-customer/iep-lijst-pnh.html)
