# Project Brief

## Client Commission
The authority receives more requests for road improvements than it can fund. Current evidence does not consistently separate long-term traffic pressure, vehicle mix, count-point coverage, temporary variation and data-estimation limitations.

> **Decision to support:** Which corridors and locations warrant the earliest investigation or capital intervention, and where is the evidence insufficient to justify investment?

## Primary Dataset
**Department for Transport Road Traffic Statistics — Count Points and Annual Average Daily Flow datasets**  
Publisher: Department for Transport  
Official source: https://roadtraffic.dft.gov.uk/downloads

## Delivery Lifecycle
**Discovery → Requirements → Governance → Acquisition → Engineering → Data Quality → Analysis → Decision Framework → BI/Product → Assurance/UAT → Executive Recommendation → Handover**

## Cross-Functional Roles
| Role | Expected contribution |
|---|---|
| Business Analyst | Define capital decision process, requirements and intervention criteria. |
| Data Governance Analyst | Govern count-point identifiers, road classes, estimation flags, lineage and quality. |
| Data Engineer | Ingest and model count points and AADF history reproducibly. |
| Transport/Data Analyst | Analyse demand, vehicle mix, trends and corridor pressure. |
| GIS Analyst | Map count points/corridors and validate spatial interpretation. |
| BI Developer | Build transport-investment decision support. |
| Data Scientist | Develop transparent demand scenarios/forecasts where justified. |
| AI/Model Governance Analyst | Assure forecast validation, uncertainty, explainability and human oversight. |

## Business Questions
1. What is the current baseline and where is material variation concentrated?
2. Which data-quality, coverage or definition issues could materially alter the decision?
3. Which segments, areas, assets, recipients or corridors require deeper investigation?
4. Which indicators are suitable for prioritisation, and which should not be used that way?
5. What intervention choices are genuinely supported by evidence?
6. What should management monitor after handover?

## Success Criteria
Traceable requirements; governed definitions/lineage/quality; reproducible transformations; defensible traffic demand, AADF trends, vehicle mix, count-point coverage, corridor pressure, regional variation and investment-prioritisation scenarios; transparent decision logic; useful BI/product; UAT evidence; executive recommendation; maintainable handover; visible collaborative contribution.

## Panel Challenge
The review panel may challenge assumptions, denominators, definitions, data quality, thresholds, models, spatial interpretation, governance, recommendations and maintainability.
