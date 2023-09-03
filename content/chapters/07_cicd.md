---
title: CI/CD Pipelines ♻️
weight: 994
---

## Hva er en CICD pipeline? 

> **CI = Continuous integration:** Frequent merging of several small changes into a main branch.


> **CD = Continuous delivery:** Levere i små bolker, hyppig, på en slik måte at teamet trygt kan release ny 
> software/funksjonaltet til enhver tid. For å få til dette kreves en enkel deployment prosess. 

- Fokus på automatisering i bygging, testing og deployment av applikasjoner. 
- Forsøk på å eliminere gapet mellom utvikling og drift. 

Avgjørende for å lykkes:
- Automatisert testing med god test-dekning
- Små og hyggige leveringer 

Tools:
- Github Action 
- Azure DevOps / Cloud Build (GCP)
- Artifact Registry / Azure Container Registry (Hosting av docker images og andre pakker for bygge prosessen)
- ArgoCD (GitOps for Kubernetes)


## I praksis 👨‍🔧

Vi skal vise kort hvordan en Github Actions deployment prosess kan fungere. 

- Hugo build
- Arkivverket 

