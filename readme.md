# DataCatalog

.. admonition:: Wat is het...

    DataCatalog is een metadata registratie systeem dat bedrijfsdata en dataproducten beschrijft in termen van wat is het, wie erover gaat, waar het te vinden is en tot welke informatieproducten het leidt.

Alle in DataCatalog beschreven bedrijfsdata is op- of via Datahub beschikbaar.
DataCatalog biedt naast metadata beschrijvingen ook:

* een baseline die inzicht geeft in *verleden, heden en toekomst* van de beschreven data,
* een systematiek voor het aggregeren en specialiseren van attributen -> dataobjecten -> datasets -> informatieproducten (UML model),
* informatie over de diverse webservices die attribuutgroepen bij bronsystemen ophalen,
* het modelleren van dataobjecten op basis van vrij te definieren relaties,
* een (BIV) dataclassificatie,
* een beperkte harmonisatie op gegevenstypen (geometrieën, datum, datumtijd, eenheden),
* het aan/uit kunnen zetten van attributen in datasets,
* veranderdetectie op belangrijke data,
* een optie om bepaalde data te vlaggen als onbetrouwbaar,
* veel data kwaliteit metrics (rapportage op data)

.. toctree::
   :maxdepth: 1

   Concept/Outline
   BasisMetadata/Basismetadata
   Concept/Data lifecycle management
   Concept/Metadata baseline
   Concept/Domeinwaarden
   Concept/Samenstellen dataobjecten
   Concept/Modelleren dataobjecten
   Functies/Functies
   Concept/Standaarden
   Requirements/Requirements
   Datakwaliteit/Indicatoren.rst
   Functies/MetadataRecords.rst


# Datahub

.. admonition:: Wat is het...

    Datahub is de centrale Azure omgeving waarin de organisatie haar data onafhankelijk verzamelt, bewerkt en ontsluit

In Datahub wordt:

    * data centraal verzameld,
    * data centraal beschikbaar gesteld,
    * data verrijkt en geanalyseerd,
    * Informatieproducten gerealiseerd,
    * Data en Informatieproducten gedistribueerd.

Zie ook de `architectuur <../html/_static/archi_datahub/archi_datahub.html>`_ van DataHub
