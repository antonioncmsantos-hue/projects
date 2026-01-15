# Data Visualization – Terrorism, Economics & Governance 

Interactive visual analytics study on global terrorism patterns (1997–2017) and how terrorism risk relates to economic development and governance quality.

**Course:** Data Visualization (NOVA SBE)  
**Group:** António Marques dos Santos, Simon Anthofer, Vanessa Weiss

---

## Analytical Questions (AQ)
- **AQ1:** Is the world really becoming increasingly dangerous?
- **AQ2:** Where is terrorism risk concentrated, and how does it relate to economic measures?
- **AQ3:** Does better governance quality go hand in hand with less terrorism?

---
## Key results (summary)
- **AQ1 (Global trend):** Terrorism intensity shows notable **spikes (e.g., around 2007 and 2014)** rather than a steady upward trend. After **2014**, the overall pattern suggests a **decline**, which challenges the idea that the world is continuously becoming more dangerous.
- **AQ2 (Economics):** Most economic indicators show **weak or inconsistent global relationships** with terrorism intensity. **GDP per capita** is not systematically predictive, while **military expenditure** shows a **moderate positive association**. **R&D expenditure** is **weakly associated with fewer attacks**, but effects vary substantially by country.
- **AQ3 (Governance):** There is a **clear (but imperfect) negative association** between governance quality and terrorism risk: higher-governance countries tend to cluster in lower-risk areas. However, the relationship is **context-dependent**, and governance improvements do not guarantee lower terrorism without broader conflict and institutional dynamics improving as well.

---

## Tableau Public dashboards (no Tableau Desktop needed)
If you don’t have Tableau Desktop/Reader, you can view the dashboards here:

- **AQ1 Dashboard:** https://public.tableau.com/app/profile/vanessa.weiss/viz/DataVisualizationG17_AQ1/AQ1-Dashboardtobegraded  
- **AQ2 Dashboard:** https://public.tableau.com/app/profile/simon.a5880/viz/shared/GSSZ42FFD  
- **AQ3 Dashboard:** https://public.tableau.com/app/profile/ant.nio.santos/viz/DataVisualizationG17_AQ3/DataVisualizationG17_AQ3  

---

## Repository structure
- `docs/`
  - `final-report.pdf` – final written report
  - `eda-report.pdf` – preprocessing + EDA documentation
- `notebooks/`
  - `datasets_eda.ipynb` – EDA / dataset preparation notebook
- `tableau/`
  - `AQ1.twbx`, `AQ2.twbx`, `AQ3.twbx` – packaged Tableau workbooks

---

## How to open locally (optional)
- Open `.twbx` files using **Tableau Desktop** or **Tableau Reader** (free).
- If you don’t have Tableau installed, use the Tableau Public links above.

---

## Data sources (high-level)
This project uses:
- Global Terrorism Database (GTD)
- World Bank World Development Indicators (WDI)
- Corruption Perceptions Index (CPI)

> Note: raw datasets may not be included in this repository depending on licensing/size.
