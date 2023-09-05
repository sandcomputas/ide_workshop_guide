---
title: Prerequisites 📝
#toc: true
weight: 999
---

> Denne NXT-dagen blir det en workshop som handler om utviklingsverktøy. Vi vil benytte Python for å holde ting enkelt - slik at fokus blir på verktøy og ikke språk. 

![Test](/toolbox_illustration.png)

## Ting å installere 💾

*Nå er det snart tid for første NXT-dag!* **Før** NXT dagen 8. september er det fint om dere har følgende på plass:

- PyCharm Community Edition installert.

  - Vi anbefaler å installere JetBrains Toolbox: https://www.jetbrains.com/toolbox-app/ og bruke denne til å installere PyCharm. Det gjør det lettere å håndtere ulike installasjoner av JetBrains programmer.

- Sjekk at dere har Python 3 (helst minst 3.10) installert. Hvis nei, installer.

- Installere Poetry (package manager for Python).

  - Poetry gjør det (relativt) enkelt å håndtere ulike pakker og miljøer i Python.
  - Installer med:
    - macOS / Linux / WSL: `curl -sSL https://install.python-poetry.org | python3 -`
    - Windows (Powershell): `(Invoke-WebRequest -Uri https://install.python-poetry.org -UseBasicParsing).Content | py -`
    - If all else fails: https://python-poetry.org/docs/
  - Etter installasjon:
    - Mac/Linux: legg `export PATH="/Users/<your username>/.local/bin:$PATH"` til i din shell configurasjon 
      fil. For mac/linux: `.bashrc` / `.zshrc`.
    - Windows: idk 🤷‍ (burde stå skrevet i terminalen rett etter dere har installert)
  

- Konfigurer Poetry ❗❗️❗️️:

  - Kjør: `poetry config virtualenvs.in-project true` i terminalen.
 
  
## Kjøre koden 👩‍💻

> Her er det to muligheter. Prøv den første først, hvis ikke det fungerer, prøv den andre.

### Clone via PyCharm 

1. Åpne PyCharm
2. Øverst til høyre i det lille vinduet som dukker opp står det "Get from VCS"
3. Lim inn urlen til Github repoet https://github.com/sandcomputas/ide_workshop
4. Trykk "clone"
5. Nå skal PyCharm klare å konfigurere prosjektet selv - vent med å gjøre noe til loading baren nederst i høyre 
   hjørne er ferdig å spinne. 
6. Nå skal du kunne kjøre koden ved å trykke den grønne "play" knappen i `main.py` 🤞
   7. Du vil sannsynligvis få en feilmelding som sier: `Please add api key for NASA to configuration 
      (IDE_WORKSHOP__NASA_KEY)`. Det er sånn det skal være :) 
7. Nice! Da er du klar for workshop!

### Manuell cloning og installering

1. Clone repoet: https://github.com/sandcomputas/ide_workshop
2. Gå til prosjektet i terminalen og kjør: `poetry install`
3. Gå til `app/main.py`. 
4. Øverst i editoren vil det dukke opp en gul linje med en ⚠️som sier at "No Python interpreter configured for the 
   project". Trykk på "Configure Python Interpreter" -> "Add new interpreter" -> "Add local interpreter".
5. I pop-up-vinduet, velg "Poetry Environment" fra venstre side meny -> velg "Existing environment".
6. Trykk så på knappen med tre prikker (...) på høyre side. Finn stedet du har lagret prosjektet på maskinen din. 
   Velg filen som ligger på `<your path>/ide_workshop/.venv/bin/python3.10`. Klikk "OK". 
7. Nå skal du kunne kjøre koden ved å trykke den grønne "play" knappen i `main.py` 🤞
8. Nice! Da er du klar for workshop!


## Problemer? 🤨

Dersom du får problemer, ta kontakt med Sondre Andersen eller Kristian Roa Gran på Slack! 🤓