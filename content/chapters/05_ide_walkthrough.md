---
title: IDE gjennomgang 🚶‍♂️ 👩‍🏫
#toc: true
weight: 996
---

> Vi starter med en liten gjennomgang av nyttige triks, deretter skal dere få prøve dere selv.

- Generelle IDE verktøy:

| Operation                                         | MacOS Hotkey                                            | Windows hotkeys                  | 
|---------------------------------------------------|---------------------------------------------------------|----------------------------------|
| *TODO* (nyttig som "notat-verktøy" i koden)       | `I venstre meny`                                        | <--                              |
| *Søk*                                             | `shift shift`                                           | `shift shift`                    |
| *Finne klasser / files*                           | `cmd + (shift) + o`                                     | `ctrl + (shift) + n`             |
| *Find (text) in files*                            | `shift + cmd + f`                                       | `ctrl + shift + r`               |
| *Go to* definition / usages                       | `cmd + b / scroll click`                                | `ctrl + b`                       |
| *Go back and forth*                               | `option + cmd + høyre/venstre pil` / `mus frem/tilbake` | `ctrl + alt + høyre/venstre pil` |
| *Rename* - variable / function / class            | `shift + F6`                                            | `shift + F6`                     |
| *Move* - / function / class                       | `F6`                                                    | `F6`                             |
| *Move file into folder and auto refactor.*        | `flytt i menyen`                                        | <--                              |
| *Optimize imports*                                | `ctrl + option + o`                                     | `ctrl + alt + o`                 |
| *Format file / prettify*                          | `option + cmd + l`                                      | `ctrl + alt + l`                 |
| *Context Actions*                                 | `option + enter`                                        | `alt + enter`                    |
| -> *Create* - function / class                    | `option + enter og velg create ...`                     | `alt + enter og velge create`    |
| -> *Auto import missing class/function/...*       | `option + enter og velge import`                        | `alt + enter og velge import`    |
| *Navigate* to project structure                   | `cmd + 1`                                               | `alt + 1` (?)                    |
| -> Inside project structre create new file/folder | `cmd + n`                                               | `ctrl + n` (?)                   |
| *Generate...* test / code                         | `høyre click -> generate `                              | <--                              |

- Git verktøy:
    - Git blame 🙈
    - Compare branch / revision
    - Commit
    - Bytte branch
    - Resolve merge conflicts
    - Commit historie

- Plugins:
    - Git toolbox
    - Atom material icons
    - Databaser / s3 / osv. (betalt versjon - se Intellij Ultimate)

- Scratch files (to, f.example prettify json) `shift + cmd + n`

- Debugging:
    1. Starte applikasjon i debug mode
    2. (Legge til environment variabler i run-config)
    3. Breakpoints
    4. Conditional breakpoints
    5. *Run program or test* `ctrl + r`
    6. *Run in debug mode* `ctrl + d`
    7. Step over / step into / jump to next breakpoint
    8. Call stack - se hvilke funksjoner funksjonen du står i nå ble kalt fra.
    9. Teste å kjøre kode `option + F8`
    10. Kjøre kode i console

Hotkeys for debugging:

| Operation             | Hotkey             |                     |
|-----------------------|--------------------|---------------------|
| Set/remove breakpoint | `cmd + F8`         | `ctrl + F8`         |
| See all breakpoints   | `cmd + shift + F8` | `ctrl + shift + F8` |

- Mulighet for å opprette nytt prosjekt fra Intellij / PyCharm.

Hotkeys fullstending
cheatsheet: https://resources.jetbrains.com/storage/products/intellij-idea/docs/IntelliJIDEA_ReferenceCard.pdf

