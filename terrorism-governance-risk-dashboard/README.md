# Risk Dashboard — Terrorism, Governance & Macroeconomics (WDI/WGI/GTD)


## Overview
This project combines terrorism incidents, governance quality, and macro indicators into **interactive Tableau dashboards** and a final report to explore **risk concentration**, **time trends**, and **governance–risk patterns**.

## Quick links
- **Final report (PDF):** [Open](https://github.com/antonioncmsantos-hue/projects/blob/main/data-visualization-terrorism/docs/G17-DV4BA-Final-Report.pdf)
- **EDA / preprocessing notebook:** [Open](https://github.com/antonioncmsantos-hue/projects/blob/main/terrorism-governance-risk-dashboard/notebooks/Datasets_EDA.ipynb)
- **Dashboards (Tableau):** [AQ1](https://github.com/antonioncmsantos-hue/projects/blob/main/terrorism-governance-risk-dashboard/tableau/Data%20Visualization%20G17_AQ1.twbx) · [AQ2](https://github.com/antonioncmsantos-hue/projects/blob/main/terrorism-governance-risk-dashboard/tableau/Data%20Visualization%20G17_AQ2.twbx) · [AQ3](https://github.com/antonioncmsantos-hue/projects/blob/main/terrorism-governance-risk-dashboard/tableau/Data%20Visualization%20G17_AQ3.twbx)

## Problem
**Is terrorism risk increasing over time, where is it concentrated, and does stronger governance correlate with lower terrorism intensity?**  
Context: macro risk analysis and country benchmarking.

## Data
- **Sources**
  - Global Terrorism Database (GTD)
  - Worldwide Governance Indicators (WGI)
  - World Development Indicators (WDI)
- **Scope**
  - GTD aggregated to **country-year**
  - Focused on the period with consistent cross-source coverage (e.g., late 1990s–2017)
- **Key variables**
  - Terrorism: attacks, casualties, per-capita metrics
  - Governance: composite index from WGI dimensions
  - Macro: population (WDI) + selected indicators for comparisons

## Method
1. Clean GTD events and aggregate to **country-year**
2. Merge population (WDI) to compute **per-capita** metrics
3. Build a composite governance index (WGI) and merge into one panel
4. Build dashboards answering three analysis questions (AQ1–AQ3)

## Results (Key Findings)
- Risk is **not a smooth global upward trend**; it is driven by regional spikes and outliers.
- Terrorism is **geographically concentrated**; macro indicators explain variation only partially.
- Higher governance quality is generally associated with lower terrorism risk, with **heterogeneity** across countries and periods.

## Outputs
- **Final report (PDF):** `reports/G17-DV4BA-Final-Report.pdf`
- **Notebook:** `notebooks/Datasets_EDA.ipynb`
- **Tableau workbooks:** `dashboards/*.twbx`
- **Preview image:** `assets/preview.png`

## Repo structure
- `data/` — raw extracts / cleaned panels (optional)
- `notebooks/` — preprocessing + EDA
- `dashboards/` — Tableau `.twbx/.twbx`
- `reports/` — PDF outputs
- `assets/` — screenshots for previews

## Notes & limitations
- GTD has known data quality variation by region/time (and a missing year in the early 1990s).
- Per-capita normalization is essential for cross-country comparability.
- Next steps: add formal models (panel regression / fixed effects) to quantify governance–risk links beyond visualization.

