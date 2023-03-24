---
description: 5e test - na sync github
---

# GitBook\_test\_mermaid

Mermaid voorbeelden

```mermaid
graph TD;
  A-->B;
  A-->C;
  B-->D;
  C-->D;
```

```mermaid
sequenceDiagram
    autonumber
    Alice->>+John: Hello John, how are you?
    Alice->>+John: John, can you hear me?
    John-->>-Alice: Hi Alice, I can hear you!
    John-->>-Alice: I feel great!
```

```mermaid

flowchart BT;
   materieel -- aggregates_to --> bedrijfsobject;
   immaterieel -- aggregates_to --> bedrijfsobject;
   verzorgingsgebied -- aggregates_to --> immaterieel;
   district -- aggregates_to --> immaterieel;
   kunstwerk -- aggregates_to --> materieel;
   stuw -- specializes --> kunstwerk;
   waterlichaam -- aggregates_to --> materieel;
   transportleiding -- aggregates_to --> materieel;
   meetreeks -- part_of --> stuw;
```

```mermaid

    flowchart BT;
        foto -- relates_to --> stuw;
        datum_foto -- part_of --> foto;
        onderhoudshistorie -- part_of --> stuw;
        TT[technische tekening] -- part_of --> stuw;
        tekenaar -- relates_to --> TT;
        datum_tekening -- part_of --> TT;
        locatie -- relates_to --> stuw;
        meetlocatie -- specializes --> locatie;
        meetreeks -- relates_to --> meetlocatie;
        validatiegrens -- part_of --> meetreeks;
        meetdoel -- part_of --> meetreeks;
```

```mermaid

    flowchart BT
       eigenaar -- relates_to --> peilbuis
       onderhoudshistorie -- part_of --> peilbuis
       F[filter] -- part_of \n1:n --> peilbuis
       bovenkant -- part_of --> F[filter]
       materiaal -- part_of --> F[filter];
       onderkant -- part_of --> F[filter]
       locatie -- relates_to --> peilbuis
       maaiveldhoogte -- relates_to --> locatie
       ML[meetlocatie] -- specializes --> locatie

       MR[meetreeks] -- relates_to --> ML

       HMR[handmatige meetreeks] -- specializes --> MR
       AMR[automatische meetreeks] -- specializes --> MR

       HM[handmeting] -- part_of --> HMR
       HMD[meetdoel] -- part_of --> HMR
       HVG[validatiegrens] -- part_of --> HMR
       HMW[meetwaarde] -- part_of --> HM
       HT[tijdstip] -- part_of --> HM

       AM[automatische meting] -- part_of --> AMR
       AMD[meetdoel] -- part_of --> AMR
       AVG[validatiegrens] -- part_of --> AMR
       AMW[meetwaarde] -- part_of --> AM
       AT[tijdstip] -- part_of --> AM
```

```mermaid

    flowchart BT;
        eigenaar -- relates_to --> boring;
        tijdstip_boring -- part_of --> boring;
        locatie -- relates_to --> boring;
        maaiveldhoogte -- relates_to --> locatie;
        laag -- relates_to \n1:n --> locatie;
        bovenkant -- part_of --> laag;
        grondsoort -- part_of --> laag;
        onderkant -- part_of --> laag;
        boorlocatie -- specializes --> locatie;
```

In de tabel `md_synonym` zijn vertalingen van de relatienamen beschikbaar die o.a. voor im/exports (Excel) gebuikt kunnen worden. De namen zijn dan:

* relatie
* specialisatie
* afhankelijk
* erft
* instantie
* onderdeel
* aggregatie

Door andere (nieuwe) relaties te definieren kunnen andere modellen vastgelegd worden.
