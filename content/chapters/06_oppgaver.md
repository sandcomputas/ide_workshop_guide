---
title: Oppgaver
#toc: true
weight: 995
---

> _Her er noen oppgaver for å øve seg på ulike verktøy i PyCharm._

## Oppgave 1

## Oppgave 2


---

## Drafts

### NASA Near Earth Asteriods feed API

> *Fix the test!*

Når vi kaller endepunktet (/????) så vil APIet vårt gjøre et kall til NASAs API. Svaret vi får er ganske stort, 
derfor cacher vi svaret, så å starte og kjøre APIet mange ganger vil være lite effektivt. I tillegg har APIet en 
limit på hvor mange requests vi kan sende hver time, så vi må være smarte her. 

En løsning for å komme rundt dette problemet og likevel kunne kjøre appen vår mange ganger og undersøke responsen er 
ved å gjøre debuggingen ved å kjøre testen `/tests/connectors/test_feed`. Denne testen har mocket ut requesten - 
slik at vi kan kjøre "kall" til APIet så mange ganger vi ønsker uten verken ventetid eller bekymringer for å nå 
request limiten. 




