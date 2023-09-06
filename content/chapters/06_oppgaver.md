---
title: Oppgaver
#toc: true
weight: 995
---

> _Her er noen oppgaver for å øve seg på ulike verktøy i PyCharm._

*Husk at det er lov å bruke cheatsheetet her: [gfdg](/chapters/04_ide_walkthrough)*

## Oppgave 1 - "Grave dypt" 

> Mål: Bli kjent med å navigere med debuggeren.

1. Åpne filen `tests/resources/test_calculation_resource.py` i PyCharm
2. Sett et breakpoint på første linje i første test (`test_calculation_add`)
3. Sett et breakpoint i `app/resources/calculation_resource.py` på linje 14
4. Starte opp debuggeren 
5. Bruk følgende kommandoer for å "grave" dere igjennom koden, prøv å kom helt ned til `app/models/calculation.py`.
- Step into: `F7`
- Step over: `F8`
- Next breakpoint: `F9`


## Oppgave 2


---

## Drafts

### Struktur på oppgave del 

Bør kanskje starte med a debugge unit tests - er kanskje endel enklere en resource tests?

### Calculator 

Fix bugs... mer kommer her 

### Calculator 2 

Litt mer avansert bug kanskje. Vi legger aldri verdien til i cache? Må kanskje være en enhets test og ikke en 
resource. Eller vi kan ha en methode som henter ut hele cahcen også? 

### NASA Near Earth Asteriods feed API

> *Fix the test!*

Når vi kaller endepunktet (/????) så vil APIet vårt gjøre et kall til NASAs API. Svaret vi får er ganske stort, 
derfor cacher vi svaret, så å starte og kjøre APIet mange ganger vil være lite effektivt. I tillegg har APIet en 
limit på hvor mange requests vi kan sende hver time, så vi må være smarte her. 

En løsning for å komme rundt dette problemet og likevel kunne kjøre appen vår mange ganger og undersøke responsen er 
ved å gjøre debuggingen ved å kjøre testen `/tests/connectors/test_feed`. Denne testen har mocket ut requesten - 
slik at vi kan kjøre "kall" til APIet så mange ganger vi ønsker uten verken ventetid eller bekymringer for å nå 
request limiten. 




