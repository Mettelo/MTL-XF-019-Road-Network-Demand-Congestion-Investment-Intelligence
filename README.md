# MTL-XF-019 — Road Network Demand, Traffic Pressure & Infrastructure Investment Intelligence

**Mettelo Project Studio**  
**Project ID:** MTL-XF-019  
**Project Type:** Cross-Functional Transport Analytics & Responsible Forecasting · Team project · Production-style portfolio project  
**Client:** Confidential Regional Transport Infrastructure Authority  
**Sector:** Transport / Highways / Infrastructure Investment  
**Engagement Type:** Simulated confidential-client engagement  
**Status:** Pre-launch  
**Recommended Team Size:** 6–8  
**Delivery Window:** 8 weeks  
**Master Repository:** Mettelo-controlled

> **Confidentiality Notice**  
> The client identity is intentionally withheld. This is a simulated Mettelo Project Studio engagement built around official public/open data. Participants must not represent the simulated client as a real external Mettelo customer.

## Challenge

A transport authority receives more requests for road improvements than its capital programme can fund. Traffic data can show demand patterns, but leadership needs a defensible way to distinguish persistent traffic pressure from temporary variation, estimated counts and incomplete evidence.

Your team will work as a multidisciplinary delivery team rather than as a group of people independently producing charts.

The engagement combines business analysis, data governance, data engineering, analytics, BI/decision support, assurance and specialist roles relevant to the project.

## Commissioned Decision

> **Which corridors and count-point areas warrant the earliest investigation or capital intervention, and where is the evidence insufficient to justify investment?**

A successful submission must help structure or support this decision. A dashboard without governed definitions, reproducible data, analytical evidence and a defensible decision framework is not sufficient.

## Official Data Source

**Department for Transport Road Traffic Statistics — Count Points and Annual Average Daily Flow datasets**

Official publisher/source:

https://roadtraffic.dft.gov.uk/downloads

The project uses a frozen Mettelo cohort copy/reference of the approved source wherever licensing and file-size rules permit. Teams should not depend on a live website or API remaining unchanged.

See:
- [Data workspace](data/README.md)
- [Source register](data/SOURCE_REGISTER.md)
- [Raw data folder](data/raw/)

## Core Objective

Build a reproducible cross-functional solution that:

1. build a longitudinal count-point and AADF analytical model;
2. preserve observed-versus-estimated count status;
3. analyse multi-year traffic demand;
4. assess vehicle-mix change;
5. identify count-point anomalies and discontinuities;
6. develop transparent investigation/investment scenarios;
7. optionally compare simple forecasting approaches with time-aware validation;
8. build GIS-enabled decision-support BI;
9. complete model governance, assurance and UAT;

## Key Business Questions

- Which count points or corridors show persistent demand growth?
- Where does vehicle mix materially change the network picture?
- Which apparent changes are driven by estimated counts or sparse coverage?
- Which locations deserve further investigation rather than immediate investment?
- What additional congestion, safety or economic evidence is needed for a full business case?

## Required Delivery Flow

```text
Discovery & stakeholder understanding
        ↓
Business requirements & acceptance criteria
        ↓
Data governance & source control
        ↓
Data ingestion & analytical modelling
        ↓
Data quality, reconciliation & exceptions
        ↓
KPI definition
        ↓
Core analysis
        ↓
Decision / prioritisation framework
        ↓
BI / decision-support product
        ↓
Assurance & UAT
        ↓
Executive recommendation
        ↓
Technical & operational handover
```

## Cross-Functional Team Model

The exact allocation can vary by team, but the project should demonstrate meaningful contribution across:

- Business Analysis;
- Data Governance;
- Data Engineering;
- Data Analysis / Domain Analysis;
- BI Development;
- Risk, Assurance or QA;
- specialist roles defined in the project brief;
- Data Science / AI or Model Governance where applicable.

One person may cover more than one function in a smaller team, but ownership and evidence must remain explicit.

## Minimum Delivery Standard

The final repository must demonstrate:

- traceable stakeholder requirements;
- governed metric and field definitions;
- frozen source/version documentation;
- reproducible data preparation;
- row/value reconciliation;
- explicit data-quality exceptions;
- project-specific analysis;
- transparent decision/prioritisation logic;
- governed BI measures;
- user acceptance testing;
- technical handover;
- visible GitHub collaboration;
- clear individual contribution evidence.

## Important Interpretation Rules

- Traffic volume is not automatically congestion.
- Keep observed and estimated counts distinguishable.
- Document count-point discontinuities and road-network changes.
- Do not infer economic or safety benefit from traffic volume alone.
- Any forecast or scenario must show uncertainty and validation.

## Agreed Success Standard

The engagement is considered successful only when:

- the approved frozen source can be identified and obtained;
- curated outputs can be regenerated from code/instructions;
- material exclusions and data-quality issues are quantified;
- headline KPIs reconcile to the curated analytical model;
- analytical conclusions answer the commissioned business questions;
- decision rules and thresholds are visible and challengeable;
- at least five headline dashboard measures reconcile to underlying data;
- UAT and assurance evidence is present;
- each member's contribution can be evidenced;
- a reviewer can reproduce the team's core outputs without undocumented manual changes.

Detailed sign-off tests are defined in:

- [Acceptance Criteria](project/ACCEPTANCE_CRITERIA.md)
- [Deliverables](project/DELIVERABLES.md)

## Repository Purpose

This master repository is the official Mettelo source of truth for:

- project scope and challenge;
- business context;
- approved data/source information;
- governance requirements;
- deliverables;
- acceptance criteria;
- team repository standards;
- final submission instructions.

Teams use this repository as the specification. Their delivery work is completed in their own team repository under the Mettelo GitHub organisation.

## Repository Structure

```text
.
├── README.md
├── project/
│   ├── README.md
│   ├── PROJECT_BRIEF.md
│   ├── BUSINESS_CONTEXT.md
│   ├── DELIVERABLES.md
│   ├── ACCEPTANCE_CRITERIA.md
│   └── GOVERNANCE.md
├── data/
│   ├── README.md
│   ├── SOURCE_REGISTER.md
│   ├── raw/
│   ├── reference/
│   └── metadata/
└── submission/
    ├── README.md
    ├── TEAM_REPOSITORY_STANDARD.md
    ├── SUBMISSION_GUIDE.md
    └── FINAL_SUBMISSION_TEMPLATE.md
```

## Start Here

### 1. Understand the engagement
- [Project Brief](project/PROJECT_BRIEF.md)
- [Business Context](project/BUSINESS_CONTEXT.md)

### 2. Understand what must be delivered
- [Deliverables](project/DELIVERABLES.md)
- [Acceptance Criteria](project/ACCEPTANCE_CRITERIA.md)

### 3. Understand governance and data
- [Governance](project/GOVERNANCE.md)
- [Data Workspace](data/README.md)
- [Source Register](data/SOURCE_REGISTER.md)

### 4. Create the team delivery repository
- [Team Repository Standard](submission/TEAM_REPOSITORY_STANDARD.md)
- [Submission Guide](submission/SUBMISSION_GUIDE.md)
- [Final Submission Template](submission/FINAL_SUBMISSION_TEMPLATE.md)

## Team Submission Model

Each project team creates its delivery repository **under the Mettelo GitHub organisation**.

Recommended naming:

`MTL-XF-019-<team-name>`

The Team Lead adds every team member using their individual GitHub account.

Teams should use issues, branches, meaningful commits, pull requests and reviews where practical as evidence of collaborative delivery.

The team repository is the official delivery artefact. The master Mettelo repository remains the source of truth for the challenge specification.

## Final Review

The team presents to a Mettelo review panel acting as the simulated senior stakeholder group.

The panel may challenge:

- problem framing;
- requirements;
- data provenance;
- quality rules;
- metric definitions;
- analytical logic;
- thresholds;
- modelling assumptions;
- decision framework;
- dashboard usability;
- recommendations;
- limitations;
- reproducibility;
- contribution evidence.

A polished presentation does not compensate for weak evidence, unreproducible analysis or unclear ownership.

---
**Mettelo — Built for What’s Next**
