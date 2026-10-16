# Data Guidance

## Approved Core Datasets

Use Department for Transport Road Traffic Statistics:

1. **Count Points**
2. **Annual Average Daily Flow (AADF)**

Official download page:
https://roadtraffic.dft.gov.uk/downloads

These are the core datasets for the project.

## What to Put in `data/raw/`

Prefer to store the original ZIP files unchanged where practical:

```text
data/raw/
├── dft-count-points.zip
└── dft-traffic-counts-aadf.zip
```

Do not edit the ZIPs.

Extract working CSVs through reproducible code or to a working/processed area.

## Recommended Time Scope

The source covers a long period.

Do **not** analyse the full history by default.

Recommended core window:
- latest **5 complete years** available in the frozen dataset.

Optional:
- extend to 10 years for long-term trend analysis after the 5-year model is working.

## Recommended Geographic Scope

Choose a manageable scope, for example:
- one region;
- one local authority plus neighbouring areas;
- selected strategic roads/corridors;
- a defined set of count points.

Document why that scope was chosen.

Do not attempt every count point in Great Britain for the core project unless the team has a justified technical reason.

## Required Join Logic

Count Points provide location/reference information.

AADF provides annual traffic-flow measures.

Before joining:
- confirm the count-point key;
- validate year coverage;
- retain road class and location fields;
- preserve observed/estimated or estimation-related flags where available;
- log count-point discontinuities.

## Recommended Analytical Grain

Use:
**count point × year** for the main longitudinal fact table.

Vehicle-type measures should remain columns or a documented long-format structure.

## Large-Data Strategy

The DfT raw-count dataset is substantially larger and is **optional**.

Do not use the raw-count ZIP for the core project unless the team specifically needs:
- time-of-day analysis;
- count-event analysis;
- deeper validation.

If an optional file is too large for GitHub:
- do not commit it;
- document exact URL;
- filename;
- file size;
- checksum;
- extraction instructions.

## GIS Extension

The DfT major-roads spatial file may be added for GIS analysis, but it is optional.

Keep reference shapefiles outside the core model unless they materially support the agreed use case.

## Forecasting Extension

If forecasting is attempted:
- use the documented 5+ year series;
- use time-aware validation;
- compare against a simple baseline;
- do not forecast count points with insufficient or discontinuous history.

## Assessment Baseline

The project must be reproducible using Count Points + AADF alone.
