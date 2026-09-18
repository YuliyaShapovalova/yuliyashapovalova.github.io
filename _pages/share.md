---
layout: archive
title: "SHARE: Synthetic Harmonized Access to Renewable Energy data"
permalink: /share/
author_profile: true
redirect_from:
  - /share
---

{% include base_path %}

**Funder:** NWO, Knowledge and Innovation Covenant (KIC) call *Data sharing for the energy transition*  
**Duration:** February 2027 to January 2031 (48 months)

SHARE develops methods to generate synthetic energy data that is realistic, privacy-safe, and consistent with the physics of the electricity network, together with the privacy guarantees and governance frameworks needed for organisations to trust and use it.

## We are hiring

**[PhD position: Physics-Informed Generative AI for Synthetic Energy Data](https://www.ru.nl/en/working-at/job-opportunities/phd-position-physics-informed-generative-ai-for-synthetic-energy-data)** at Radboud University. Start February 2027. Application deadline 25 October 2026.
{: .notice--info}

The project starts in February 2027 and I am recruiting one **PhD candidate** at Radboud University (iCIS) on physics-informed generative models for synthetic energy data. The PhD will develop deep generative models (VAEs, GANs, diffusion models, Gaussian processes) for energy time series that respect the physics of the network, working with real operational data from Alliander. Supervision by Dr. Yuliya Shapovalova and Prof. Tom Heskes. Expected start: February 2027. Full details and the application form are on the [Radboud University vacancy page](https://www.ru.nl/en/working-at/job-opportunities/phd-position-physics-informed-generative-ai-for-synthetic-energy-data).

## The problem

The Dutch energy transition depends on data that almost no one is allowed to see. Distribution system operators (DSOs), municipalities, and energy communities need high-resolution grid and consumption data to plan grid reinforcements, heat networks, and local flexibility. Privacy law, commercial sensitivity, and regulatory uncertainty keep most of this data locked away. As a result, critical infrastructure decisions are being made with incomplete information.

Synthetic data offers a way out: artificial datasets that preserve the statistical, temporal, and physical structure of real energy data while revealing nothing about any real household or company. But energy data is not like images or text. It consists of time series living on a physical network, governed by power-flow equations. Off-the-shelf generative models produce data that looks plausible but violates physics, which makes it of limited use for grid planning. And no synthetic dataset will be adopted unless its privacy properties can be verified and its use is legally and institutionally trusted.

## Our approach

SHARE combines machine learning, privacy engineering, energy law, and energy planning in the following work packages:

- **Use cases and requirements.** Together with DSOs, municipalities, and energy communities, we define which data needs to be shared, between whom, and for what decisions, and translate this into quantifiable requirements for synthetic datasets. Led by Dr. Henk-Jan Kooij with Prof. Saskia Lavrijssen (Radboud University).
- **Synthetic data generation.** We develop and compare deep generative models (variational autoencoders, GANs, diffusion models, Gaussian processes) for load, generation, and voltage time series, and embed physical constraints such as power-flow consistency, operational bounds, and network topology directly into the generation process. Led by Dr. Yuliya Shapovalova with Prof. Tom Heskes (Radboud University).
- **Adaptive privacy and legal compliance.** We develop adaptive differential privacy mechanisms that allocate privacy budget according to the sensitivity of each data component, evaluate them against realistic privacy attacks, and build a verification framework aligned with the GDPR and the EU AI Act. Led by Dr. Mina Alishahi with Prof. Harald Vranken (Open Universiteit).
- **Adoption and dissemination.** Training, documentation, and a community of practice so that the methods are actually used by the Dutch energy sector.

The main outputs are an open-source synthetic data toolbox, a privacy-utility benchmarking and auditing toolkit, openly published benchmark datasets, and governance guidelines for privacy-compliant data sharing in the energy sector.

## Consortium

- [Radboud University](https://www.ru.nl/en) (coordinator): machine learning and AI, strategic energy planning, energy law and governance
- [Open Universiteit](https://www.ou.nl/en): privacy engineering, cybersecurity, and privacy law
- [Alliander](https://www.alliander.com/en/): distribution system operator, providing use cases and operational data
- [Gemeente Nijmegen](https://www.nijmegen.nl/): municipal spatial energy planning use cases
- [Zenmo](https://zenmo.com/): energy system modelling
- [VSL](https://www.vsl.nl/en/): national metrology institute, measurement quality and validation
- [Bronscode](https://bronscode.nl/): software engineering for the open-source toolbox
- [NPRES](https://www.regionale-energiestrategie.nl/) / VIVET: alignment with the national roadmap for energy data sharing
