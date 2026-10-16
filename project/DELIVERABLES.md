# Required Deliverables

## D1 — Discovery, Decision & Requirements Pack
**Due:** Week 1  
**Location:** `docs/01-discovery/`

Decision statement; stakeholder map; as-is/to-be process; minimum 8 prioritised functional/user requirements; non-functional requirements; assumptions/dependencies; mapped acceptance criteria.

**Acceptance:** every planned feature/analysis maps to an approved requirement.

## D2 — Data Governance & Source Control Pack
**Due:** Week 2  
**Location:** `docs/02-data-governance/`, `data/SOURCE_REGISTER.md`

Frozen-source inventory; glossary; critical data elements; owner/steward assumptions; lineage; DQ rules; reuse notes; governance risks.

**Acceptance:** every headline KPI traces to governed source fields.

## D3 — Reproducible Ingestion & Analytical Model
**Due:** Week 3  
**Location:** `src/`, `sql/`, `docs/03-data-model/`

Load process; raw preservation; schema/type checks; standardisation; keys/grain; curated tables; rerun instructions; exception handling.

**Acceptance:** same frozen input produces equivalent curated output on clean rerun.

## D4 — Data Quality, Reconciliation & Exceptions
**Due:** Week 3  
**Location:** `docs/04-data-quality/`, `tests/`

Row/value reconciliation; duplicates; missingness; accepted values/ranges; exception log; inclusion/exclusion rules.

**Acceptance:** material exclusions/adjustments are quantified and explained.

## D5 — KPI & Metric Catalogue
**Due:** Week 4  
**Location:** `docs/05-kpi-catalogue/`

Minimum metrics:
- AADF by count point/year;
- total motor vehicles;
- car/taxi share;
- LGV share;
- HGV share;
- multi-year demand growth;
- persistent-growth flag;
- observed-versus-estimated count indicator;
- count-point coverage/completeness;
- priority-investigation score components;

Each metric requires purpose, definition, formula, grain, source, exclusions, owner, refresh expectation and limitation.

## D6 — Core Analytical Assessment I
**Due:** Week 5  
**Location:** `analysis/`, `docs/06-analysis/`

- multi-year demand trends;
- vehicle-mix change;
- observed/estimated count comparison;
- count-point coverage and anomalies;

Each major finding states comparison basis, materiality and limitation.

## D7 — Core Analytical Assessment II & Decision Framework
**Due:** Week 6  
**Location:** `docs/07-decision-framework/`

- corridor/count-point investigation segmentation;
- look-back/threshold sensitivity;
- optional forecast/scenario comparison;
- evidence-gap classification;
- explicit factors/thresholds;
- rationale;
- at least one sensitivity test;
- manual-review triggers;
- evidence insufficient for action.

## D8 — BI / Decision-Support Product
**Due:** Draft Week 6; final Week 7  
**Location:** `dashboard/`

Executive view; diagnostic drill-down; governed measures; source/reporting period; definitions/quality notes; filters; accessibility; reproducible build/access instructions.

**Acceptance:** at least five headline measures reconcile to curated data.

## D9 — Assurance & UAT
**Due:** Week 7  
**Location:** `docs/08-assurance-uat/`

Minimum 10 scenarios; calculation/filter/edge checks; reconciliation; defect log; requirement-to-test traceability; UAT feedback; final status.

## D10 — Technical & Operational Handover
**Due:** Week 8  
**Location:** `docs/09-technical-handover/`

Setup; run/refresh; architecture/data flow; transformations; metric logic; tests; troubleshooting; limitations; maintenance/change guidance.

## D11 — Executive Briefing & Presentation
**Due:** Week 8  
**Location:** `deliverables/`

Maximum two-page briefing plus 15–20 minute presentation covering decision, evidence, recommendation/investigation, limitations and next steps.

## D12 — Contribution & Delivery Evidence
**Due:** Final submission  
**Location:** `CONTRIBUTIONS.md`

Role, work packages, artefacts, linked issues/PRs/commits, review contribution and presentation contribution. Commit count alone is insufficient.
