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
 
- Clone Github-repo: https://github.com/sandcomputas/ide_workshop  🌐


## Kjøre koden 👩‍💻

1. Gå til `app/main.py`. 
2. Øverst i editoren vil det dukke opp en gul linje med en ⚠️som sier at "No Python interpreter configured for the 
   project". Trykk på "Configure Python Interpreter" -> "Add new interpreter" -> "Add local interpreter".
3. In the pop-up, select "Poetry Environment" from the left side-bar -> choose "Existing environment".
4. Then press the buttun with tree dots on the right "...". Locate the place on your computer where you stored this 
   python project. Choose the `<your path>/ide_workshop/.venv/bin/python3.10` file. Press OK. 
5. Nå skal du kunne kjøre koden ved å trykke den grønne "play" knappen i `main.py` 🤞

## Problemer? 🤨

Dersom du får problemer, ta kontakt med Sondre Andersen eller Kristian Roa Gran på Slack! 🤓