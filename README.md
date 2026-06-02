# Auracelle Charlie — Workshop Portal

**An Asynchronous War Game for AI Governance — without needing to be an expert.**

> *Auracelle Charlie puts you in the room where AI policy gets vetted.*

[![License: Proprietary](https://img.shields.io/badge/License-Proprietary-red.svg)](./LICENSE)
[![Framework: E-AGPO-HT](https://img.shields.io/badge/Framework-E--AGPO--HT-teal.svg)](./docs/FRAMEWORK.md)
[![Doctoral Research](https://img.shields.io/badge/Research-Bath%20Spa%20University-blue.svg)](./docs/RESEARCH.md)

---

## Overview

Auracelle Charlie is an AI governance wargame simulation instrument built on the **E-AGPO-HT framework** (Experimental AI Governance Policy Optimisation — Human Terrain). It places participants in the roles of real stakeholder groups — states, institutions, civil society, and industry — negotiating live AI governance scenarios with other actors.

The Workshop Portal is a single-file HTML application that requires no installation, no server, and no prior knowledge of AI governance. It launches directly in any modern browser.

---

## Quick Start

### Option A — GitHub Pages (recommended for workshops)
```
https://<your-org>.github.io/<repo-name>/
```

### Option B — Local
1. Download `index.html`
2. Open in any modern browser (Chrome, Firefox, Edge, Safari)
3. No dependencies, no installation required

---

## Repository Structure

```
.
├── index.html                  # Auracelle Charlie Workshop Portal (self-contained)
├── README.md                   # This file
├── LICENSE                     # Proprietary licence with E-AGPO-HT IP carve-out
├── CHANGELOG.md                # Version history
├── docs/
│   ├── FACILITATOR_GUIDE.md    # Step-by-step workshop facilitation guide
│   ├── PARTICIPANT_GUIDE.md    # Participant quick-start card
│   ├── FRAMEWORK.md            # E-AGPO-HT framework overview
│   └── RESEARCH.md             # Doctoral research context and citation
└── assets/
    └── .gitkeep
```

---

## The Simulation

### Login — Participant Composition
Participants select two independent dimensions at login:

| Dimension | What it captures | Options |
|-----------|-----------------|---------|
| **Sector** | Professional background | Cross-Sector · Military/Defence · Civil Society · Technical/Industry · Academic |
| **Gender Composition** | Demographic makeup of the group today | Mixed · All-Female · All-Male |

These two selections are the **primary independent variables** in the research design. They are independent of each other — a female military officer in an all-female group selects **Military/Defence** + **All-Female** → research code **ML-AF**.

---

### Session Design — Tab ①
Configure your session before launching:

| Field | Purpose |
|-------|---------|
| **Participant Composition Group** | Maps to actor pool (Cross-Sector, Military, Civil Society, Technical) |
| **Scenario Domain Pack** | AI Weapons · Cyber Norms · Nuclear-AI · Autonomous Systems · Data Sovereignty · Privacy · Frontier AI |
| **Workshop Use-Case** | Specific stress-test objective for the session |
| **Round Arc** | Structured narrative arc for the 6 rounds |
| **Information Regime** | Partial / Complete / Adversarial |

Press **▶ Initialise Session** to move to the Facilitator tab.

---

### Facilitator Mode — Tab ②
The core turn-logging interface. For each actor move:

1. **Select Actor** — one of the five session actors
2. **BGC Domain** — what governance capability does this move engage?

| Code | Plain meaning |
|------|--------------|
| STI | Sensing & Intelligence (spotting threats) |
| SAD | Building the Rules (designing governance) |
| ESI | Testing & Modelling (running scenarios) |
| NDM | Negotiating (forming agreements) |
| SRA | Judging Intent (assessing actor behaviour) |
| IIC | Implementing (putting rules into practice) |
| ASI | Adapting (keeping governance flexible) |

3. **Move Type** — what did the actor do?

| Move | Plain meaning | Best rounds |
|------|--------------|-------------|
| Propose | Put a new idea on the table | 1–2 |
| Coalition | Formally join another actor | 1–3 |
| Counter | Push back with an alternative | 2–4 |
| Verify | Demand proof before agreeing | 2–4 |
| Comply | Accept what is on the table | 4–6 |
| Escalate | Raise the stakes / invoke a red line | 4–6 |
| Defect | Withdraw or refuse to cooperate | Any |
| Delay | Stall for time | Any |

4. **Rationale Captured** — record what the actor said
5. **Governance Action Taken** — select the specific action matching the rationale
6. Press **⊕ Log Move** → **Advance Round** when all actors have moved

**💡 Suggest My Move button**: generates a structured, scenario-grounded suggestion for the selected actor and round. Works without an API key (Path A — static heuristic) or with an Anthropic API key (Path B — AI reasoning).

---

### Governance Indicators — Tab ③
Live dashboard tracking seven indicators updated after every move:
- Coalition Stability · Compliance Signal · Legitimacy Index
- Fragmentation Score · Decision Latency · Escalation Index · Public Trust

---

### Additional Tabs
| Tab | Purpose |
|-----|---------|
| ④ Foresight Validation | Compare session outcomes to historical governance cases |
| ⑤ After-Action Review | Auto-generated debrief with PSTOA scores |
| ⑥ SIPRI Data | Live arms transfer and military expenditure context |
| ⑦ MARL Engine | Multi-Agent Reinforcement Learning simulation |
| ⑧ Autonomous Sim | Fully AI-driven session for baseline generation |
| ⑨ Red Team | Shock injection and adversarial stress-testing |
| ⑩ Agentic AI | Policy Owner + Agentic Red Team (requires Anthropic API key) |
| ⑪ Archive | Cross-session tracking and PSTOA score history |

---

### API Key (Optional — Tab ⑩)
An Anthropic API key activates:
- **Policy Owner Agent** — always-on governance monitor with live challenge prompts
- **Agentic Red Team** — APT-attributed adversarial reasoning (APT41, Sandworm, APT29, XENOTIME)
- **Suggest My Move (Path B)** — AI-powered turn suggestions using live session state

Without a key, all core simulation features operate normally using structured heuristic logic.

---

## Scenarios

| Domain | Stress-test focus |
|--------|------------------|
| AI Weapons Governance | Autonomous lethal systems — LOAC compliance, human oversight thresholds |
| Cyber Norms & Standards | Critical infrastructure — attribution, private sector compliance |
| Nuclear-AI Nexus | C2 governance — AI in nuclear command and control |
| Autonomous Systems | LOAC compliance under autonomous decision-making |
| Data Sovereignty | AI training governance — cross-border data flows |
| Privacy Compliance | Algorithmic accountability — enforcement and deterrence |
| **Frontier AI** *(default)* | Catastrophic risk and safeguards — SB-53 stress-test |

---

## Research Context

Auracelle Charlie is a doctoral research instrument developed at **Bath Spa University** under the supervision of Dr. John Curry. It is the primary simulation platform for the thesis:

> *"Testing Public Policy Outcomes through War Gaming Methodologies for Strengthening AI Governance"*

The E-AGPO-HT framework underpinning this instrument is proprietary. See [LICENSE](./LICENSE) and [docs/FRAMEWORK.md](./docs/FRAMEWORK.md).

**Academic affiliation:** Auracelle AI Governance Labs · UC Berkeley CLTC (Non-Resident Senior Fellow) · NATO STO SAS-219 (Technical Role Member, R4/R5/R7)

**Public platform:** [https://auracelle.github.io/Auracelle-AI-Governance-Labs-Platform-Comms-Public](https://auracelle.github.io/Auracelle-AI-Governance-Labs-Platform-Comms-Public)

---

## Citation

If you use Auracelle Charlie in research or workshops, please cite:

```
Evans, G-A. (2025). Auracelle Charlie: An AI Governance War Game Simulation Instrument.
Auracelle AI Governance Labs. Bath Spa University Doctoral Research Programme.
https://github.com/<your-org>/<repo-name>
```

---

## Contact

**Grace-Alice Evans**
Founder & Principal Investigator, Auracelle AI Governance Labs
LinkedIn: [https://www.linkedin.com/in/grace-alice-evans-5a9632a3](https://www.linkedin.com/in/grace-alice-evans-5a9632a3)

---

*© 2025 Auracelle AI Governance Labs. All rights reserved. E-AGPO-HT framework, BGC taxonomy, and NOF specifications are proprietary. See LICENSE.*
