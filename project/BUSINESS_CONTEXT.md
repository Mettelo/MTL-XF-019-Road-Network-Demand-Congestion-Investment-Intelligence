# Business Context

## Business Problem

The transport authority receives more requests for highway improvements than its capital budget can support. Traffic-count data provides useful evidence about vehicle volumes and long-term change, but current decision-making can over-rely on single-year counts or headline traffic growth without considering whether counts are observed or estimated, whether count-point coverage has changed, or whether high volume actually represents congestion.

This creates an infrastructure-prioritisation problem. Leadership needs a defensible way to identify corridors or count points that genuinely warrant further investigation, while also identifying where the available traffic data is too weak to support a capital case.

The business problem is therefore to create a longitudinal network-demand intelligence product that separates persistent traffic pressure from temporary variation and makes evidence quality visible before investment decisions are considered.

## Required Delivery Response

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

## How the Client Will Use the Output

The finished product should support a transport investment gateway meeting. A planning lead should be able to identify a corridor where multi-year demand is growing, understand the vehicle mix and quality of the underlying counts, and decide whether the corridor should move to a deeper congestion/economic assessment.

The product should not claim that high AADF automatically means congestion or that a high-priority analytical flag justifies capital expenditure.

## Client
**Confidential Regional Transport Infrastructure Authority**

## Problem
The authority receives more requests for road improvements than it can fund. Current evidence does not consistently distinguish long-term traffic demand, temporary variation, vehicle mix, estimated counts and count-point coverage, so investment priorities are difficult to defend.

## Decision Owner
**Director of Transport Strategy**

## Stakeholders
Head of Highways, Network Planning Lead, Capital Programme Lead, Transport Modelling Lead, GIS Lead, Data Governance Lead, Finance Business Partner

## Decision
**Which corridors and count-point areas warrant the earliest investigation or capital intervention, and where is the evidence insufficient to justify investment?**

## Role Responsibilities
| Role | Required contribution |
|---|---|
| Business Analyst | Define capital-investment decision, stakeholder requirements and acceptance criteria. |
| Data Governance Analyst | Govern count-point IDs, road classes, estimation flags, geography and lineage. |
| Data Engineer | Build reproducible count-point/AADF ingestion and longitudinal model. |
| Transport/Data Analyst | Own demand, vehicle-mix, persistence and count-quality analysis. |
| GIS Analyst | Map count points/corridors and validate spatial interpretation. |
| BI Developer | Build network-investment decision support and drill-down. |
| Data Scientist | Develop transparent demand scenarios/forecasting where justified. |
| AI/Model Governance Analyst | Assure validation, uncertainty, explainability and human oversight. |

## Evidence Chain
**Requirement → governed definition → transformation → quality control → metric/analysis → decision insight → recommendation → UAT**
