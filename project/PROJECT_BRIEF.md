# Project Brief

## Engagement Details
| Field | Detail |
|---|---|
| Project ID | MTL-XF-019 |
| Project Title | Road Network Demand, Traffic Pressure & Infrastructure Investment Intelligence |
| Client | Confidential Regional Transport Infrastructure Authority |
| Sector | Transport / Highways / Infrastructure Investment |
| Duration | 8 weeks |
| Recommended Team Size | 6–8 |
| Primary Sponsor | Director of Transport Strategy |
| Senior Stakeholders | Head of Highways, Network Planning Lead, Capital Programme Lead, Transport Modelling Lead, GIS Lead, Data Governance Lead, Finance Business Partner |
| Primary Dataset | Department for Transport Road Traffic Statistics — Count Points and Annual Average Daily Flow datasets |

## 1. Client Situation
The authority receives more requests for road improvements than it can fund. Current evidence does not consistently distinguish long-term traffic demand, temporary variation, vehicle mix, estimated counts and count-point coverage, so investment priorities are difficult to defend.

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
