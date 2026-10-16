# Project Brief

## 1. Business Problem

The transport authority receives more requests for highway improvements than its capital budget can support. Traffic-count data provides useful evidence about vehicle volumes and long-term change, but current decision-making can over-rely on single-year counts or headline traffic growth without considering whether counts are observed or estimated, whether count-point coverage has changed, or whether high volume actually represents congestion.

This creates an infrastructure-prioritisation problem. Leadership needs a defensible way to identify corridors or count points that genuinely warrant further investigation, while also identifying where the available traffic data is too weak to support a capital case.

The business problem is therefore to create a longitudinal network-demand intelligence product that separates persistent traffic pressure from temporary variation and makes evidence quality visible before investment decisions are considered.

## What the Team Needs to Do

The team is expected to build a road-network demand and investment-investigation solution.

The work should include:
- defining the capital-investment questions and decision users;
- building a governed count-point/AADF longitudinal model;
- validating count-point identifiers across years;
- preserving observed-versus-estimated count status;
- analysing multi-year traffic demand and vehicle mix;
- identifying anomalies, discontinuities and coverage gaps;
- distinguishing persistent demand from one-year spikes;
- developing transparent investigation-priority rules;
- optionally building simple forecasts only with time-aware validation and a baseline;
- creating GIS-enabled decision-support views;
- documenting what congestion, safety, economic or scheme-cost evidence would still be required for a full business case;
- completing assurance, UAT and handover.

## Practical Use Case

The finished product should support a transport investment gateway meeting. A planning lead should be able to identify a corridor where multi-year demand is growing, understand the vehicle mix and quality of the underlying counts, and decide whether the corridor should move to a deeper congestion/economic assessment.

The product should not claim that high AADF automatically means congestion or that a high-priority analytical flag justifies capital expenditure.

## 2. Business Decision
> **Which corridors and count-point areas warrant the earliest investigation or capital intervention, and where is the evidence insufficient to justify investment?**

## 3. Agreed Objectives
1. Build a governed count-point/AADF analytical model with clear road, geography and year definitions.
2. Separate observed and estimated traffic measures and make coverage limitations visible.
3. Identify persistent traffic-demand pressure and vehicle-mix change without calling traffic volume congestion by default.
4. Develop transparent investigation/investment prioritisation scenarios.
5. Provide a decision-support product that allows leadership to move from portfolio view to count-point/corridor evidence.

## 4. Key Business Questions
1. Which count points or corridors show persistent demand growth over multiple years?
2. Where do heavy-goods, light-goods or car mix changes materially alter the network picture?
3. Which apparent changes are driven by estimation, sparse coverage or one-year anomalies?
4. Which areas combine high demand, growth and strategic vehicle mix in a way that merits further investigation?
5. What evidence is missing for a true congestion, economic or safety investment case?
6. How sensitive are priorities to alternative thresholds and look-back windows?

## 5. Cross-Functional Roles
| Role | Minimum expected output |
|---|---|
| Business Analyst | Define capital-investment decision, stakeholder requirements and acceptance criteria. |
| Data Governance Analyst | Govern count-point IDs, road classes, estimation flags, geography and lineage. |
| Data Engineer | Build reproducible count-point/AADF ingestion and longitudinal model. |
| Transport/Data Analyst | Own demand, vehicle-mix, persistence and count-quality analysis. |
| GIS Analyst | Map count points/corridors and validate spatial interpretation. |
| BI Developer | Build network-investment decision support and drill-down. |
| Data Scientist | Develop transparent demand scenarios/forecasting where justified. |
| AI/Model Governance Analyst | Assure validation, uncertainty, explainability and human oversight. |

## 6. Minimum Delivery Standard
Traceable requirements; governed definitions/lineage; preserved raw data; reproducible transformation; reconciliation; project-specific analysis; transparent decision logic; governed BI; UAT; handover; collaborative evidence.

## 7. Constraints
- AADF and traffic counts are not direct congestion measures.
- Estimated counts must be distinguishable from observed counts.
- Count-point coverage and road-network changes can distort longitudinal comparisons.
- Traffic volume alone does not prove economic benefit, safety need or investment value.
- Forecasts/scenarios are planning support and must show uncertainty.

## 8. Agreed Success Criteria
- Observed and estimated traffic records are distinguishable in the curated model and dashboard.
- Count-point identifiers are validated for longitudinal use and discontinuities are logged.
- At least five count-point/year values reconcile to the DfT source data.
- No output labels high traffic volume as congestion unless a separate justified congestion measure is introduced.
- Priority logic uses a documented multi-year rule rather than one-year volume alone.
- If forecasting is used, a simple baseline and time-aware validation are included.

## 9. Out of Scope
Core delivery excludes confidential personal data, paid production infrastructure, automated operational decisions and unsupported causal inference.

## 10. Reproducibility Definition
A reviewer should be able to clone the team repository, obtain the approved source data, execute the workflow and reproduce curated outputs and validation evidence without undocumented manual changes.
