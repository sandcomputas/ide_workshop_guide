---
title: Oppgaver
#toc: true
weight: 995
---

> _Her er noen oppgaver for å øve seg på ulike verktøy i PyCharm._

*❗❗❗️Husk at det er lov å bruke cheatsheetet her: [cheatsheet](/ide_workshop_guide/chapters/04_ide_walkthrough)❗❗❗*

## Oppgave 1 - "Grave dypt" 🪨 ⛏ (15min)

[BRANCH: xxxxx]

> *Mål: Bli kjent med å navigere med debuggeren.*

1. Åpne filen `tests/resources/test_calculation_resource.py` i PyCharm
2. Sett et breakpoint på første linje i første testen `test_calculation_add`
3. Sett et breakpoint i `app/resources/calculation_resource.py` på linje 14
4. Starte testen i debug mode  
5. Bruk følgende kommandoer for å **"grave"** dere igjennom koden, prøv å kom helt ned til 
   `app/repositories/calculation_repository.py`.
- Step into: `F7`
- Step over: `F8`
- Next breakpoint: `F9`

*Kommentarer:*
- Det er natulig at man må starte debuggeren om igjen og om igjen (`ctrl + d`) 
- Dersom man "stepper into" `F7` innebyde funksjoner eller andre bibliotek funksjoner er det lett å gå seg litt vill.
- Lurt å lukke alle åpne tabs før vi begynner på ny oppgave - lett å gå seg bort!

## Oppgave 2 - "Dårlig kalkulator" 🧮 (15min)

[BRANCH: xxxx]

> *Mål: Bruke debuggeren til å finne og fikse feil i kalkulatoren som gjør at testen vår feiler* 

1. Kjøre alle testene (ikke debug), se hvilken som feiler 
2. Kjøre den spesifikke testen som feiler i debug mode 
3. Bruk breakpoints og step over `F8`, step into `F7` funksjonene for å finne og rette feilen. 
4. Målet er å få alle testene til å passere (skal bare være behov for å endre en!)

*Tips:*
- Bruk debuggeren til å utforske og inspiser variabler underveis for å prøve å finne hvor det går galt. 
- (Prøv å bruke debuggeren i stedet for å lese koden nøye for å finne feilen, det er litt av poenget 😉 )

## Oppgave 3 - "Kalkulatoren kan bare regne det samme en gang!?" (15min)

[BRANCH: xxxxx]

1. Kalkulatoren vår har også en vakker frontend (`localhost:8080/calculator.html`)
2. Noen brukere har rapportert at dersom de prøver å regne ut det samme regnestykket mer enn en gang så går ting galt
3. Bruk debuggeren, sammen med frontend applikasjonen til å finne ut hvorfor og fiks gjerne feilen og se at det 
   fungerer. 

*Kommentarer:*
- Start applikasjonen i debug mode 
- Set breakpoint i ressursen `app/resources/calculation_resource.py` og gå innover derifra. 
- OBS: Feilen ligger *ikke* i frontend-koden som ligger i `static` mappen.

## Oppgave 4 - Conditional breakpoint (5min - kun felles gjennomgang)

[BRANCH: xxxxx]

> Mål: Vise hvordan man kan bruke "conditional breakpoints"

- Få applikasjonen til å stoppe når vi har kommet til det punktet der `hazardous_asteroids` listen i 
  `app/services/near_earth_asteroids_service` har fått 4 elementer. 


## Oppgave 5 "No response from NASA API" (15min) 

[BRANCH: xxxxx]

> Mål: Få litt mer trening i å bruke debuggeren til å finne bugs






## Oppgave 3 - "Første bug" 🪲 (15min)

[BRANCH: xxxxx]

> Mål: 


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




