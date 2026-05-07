# HIV County-Level Need vs Access Gap Analysis

**End-to-End Data Analytics Portfolio Project**

## Project Overview
A county-level screening model that identifies areas with **high HIV burden + high access barriers** using public data from CDC AtlasPlus and ACS.

**Gap Score** = (HIV Prevalence Percentile + Access Risk Score Percentile) / 2

## Key Deliverables

### Visualizations
![Need vs Access Gap Map](outputs/figures/gap_score_hiv_prevalence_access_barriers.png)
**Need vs Access Gap Score** (National County Map)

![HIV Prevalence](outputs/figures/hiv_prevalence_map.png)
**HIV Prevalence Rate (per 100,000)**

![Access Risk Score](outputs/figures/access_risk_score_map.png)
**Access Risk Score** (Uninsured % + Poverty %)

![Scatter Plot](outputs/figures/hiv_need_vs_access_scatter.png)
**HIV Need vs Access Barriers** (colored by Viral Suppression %)

### Data Files
- [`full_merged_dataset.csv`](outputs/full_merged_dataset.csv) — Complete dataset with all metrics
- [`top15_gap_counties.csv`](outputs/top15_gap_counties.csv) — Top 15 priority counties

## Key Findings
- Several counties show **compounding risk** (high HIV prevalence + very high uninsured + poverty rates).
- Viral suppression provides important context on care outcomes in high-gap areas.
- Clear geographic patterns visible on the national maps.

## Limitations
- CDC suppresses HIV data in counties with small case counts (privacy/statistical reliability). Gap score calculated only on available data.
- This is a **screening tool** for prioritization, not a causal analysis.

## Use Case
Helps public health teams, nonprofits, and policymakers quickly identify counties that warrant deeper investigation into clinic capacity, outreach programs, and care navigation.

## Tech Stack
- Python, pandas, plotly.express, censusdata
- GeoJSON county boundaries
- ACS 2022 5-year estimates + CDC AtlasPlus

## How to Reproduce
1. Clone the repo
2. Open `notebooks/04_county_map_uninsured_%.ipynb`
3. Run all cells (requires Census API key for fresh ACS data)

**Data Sources**:
- ACS 2022: Uninsured and Poverty percentages
- CDC AtlasPlus: HIV Prevalence & Viral Suppression

---

Made as part of my Data Analytics portfolio.