---
title: IDE walkthrough 🚶‍♂️ 👩‍🏫
#toc: true
weight: 997
---

> Vi starter med en liten gjennomgang av nyttige triks, deretter skal dere få prøve dere selv.

- IDE refactoring tool:

| Operation                                         | Hotkey                              |
|---------------------------------------------------|-------------------------------------|
| *TODO* (nyttig som "notat-verktøy" i koden)       | `I venstre meny`                    |
| *Go to* definition / usages                       | `cmd + b / scroll click`            |
| *Go back and forth*                               | `option + cmd + høyre/venstre pil`  |
| *Generate...* test                                | `høyre click -> generate `          |
| *Rename* - variable / function / class            | `shift + F6`                        |
| *Move* - / function / class                       | `?`                                 |
| *Move file into folder and auto refactor.*        |                                     |
| *Optimize imports*                                | `ctrl + option + o`                 |
| *Format file / prettify*                          | `option + cmd + l`                  |
| *Intellij suggestion*                             | `option + enter`                    |
| -> *Create* - function / class                    | `option + enter og velg create ...` |
| -> *Auto import missing class/function/...*       | `option + enter og velge import`    |
| *Navigate* to project structure                   | `F1`                                |
| -> Inside project structre create new file/folder | `cmd + n`                           |
| *Finne klasser / functioner*                      | `cmd + (shift) + o`                 |
| *Find (text) in files*                            | `shift + cmd + f`                   |

- Git tools:
    - Git blame 🙈
    - Compare branch / revision
    - Commit
    - Bytte branch
    - Resolve merge conflicts 

- Plugins:
    - Databaser / s3 / osv. (betalt versjon - se Intellij Ultimate)

- Scratch files (to, f.example prettify json)

- Debugging:
    1. Starte applikasjon i debug mode
    2. (Legge til environment variabler i run-config)
    3. Breakpoints
    4. Conditional breakpoints
    5. *Run program or test* `ctrl + r`
    6. *Run in debug mode* `ctrl + d`
    7. Step over / step into / jump to next breakpoint
    8. Teste å kjøre kode `option + F8`
    9. Kjøre kode i console

Hotkeys for debugging:

| Operation             | Hotkey             |
|-----------------------|--------------------|
| Set/remove breakpoint | `cmd + F8`         |
| See all breakpoints   | `shift + cmd + F8` |

- Mulighet for å opprette nytt prosjekt fra Intellij / PyCharm.
