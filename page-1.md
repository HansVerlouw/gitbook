# Page 1

```mermaid
    flowchart BT
        materieel -- aggregates_to --> bedrijfsobject
        immaterieel -- aggregates_to --> bedrijfsobject
        verzorgingsgebied -- aggregates_to --> immaterieel
        district -- aggregates_to --> immaterieel
        kunstwerk -- aggregates_to --> materieel
        stuw -- specializes --> kunstwerk
        waterlichaam -- aggregates_to --> materieel
        transportleiding -- aggregates_to --> materieel
        meetreeks -- part_of --> stuw
```
