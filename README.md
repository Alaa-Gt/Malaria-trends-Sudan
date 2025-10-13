# Malaria-trends-Sudan
Malaria burden (DALYs) in Sudan, 2011–2021 — IHME GBD data. Excel analysis &amp; visualization.
# Malaria Trends in Sudan (2011–2021)

**Short description**
This small project explores trends in malaria burden in Sudan using IHME Global Burden of Disease (GBD) estimates (DALYs, 2011–2021). It is an early portfolio piece created using Microsoft Excel to clean and visualize the data.

---

## Files in this repo

* data/malaria_dalys_rate_sudan_2011_2021.csv` — cleaned CSV (year, DALYs_rate).
* images/malaria_trend_sudan_2011_2021.png` — line chart image (DALYs rate over 2011–2021).
* raw_data_note.txt` — instructions and link to original IHME GBD tool to download raw data.

---

## Data source & license

* Source: IHME — Global Burden of Disease results (GBD). Data downloaded and processed for analysis.
* Note: I have included cleaned aggregated results here. If you need the original IHME files, follow the instructions in `raw_data_note.txt` and check IHME’s terms before redistributing.

---

## What I did (methods)

1. Downloaded GBD data for **Malaria — Sudan** (2011–2021).
2. Filtered to **DALYs** (both sexes, all ages).
3. Kept `year` and `value` (DALYs rate), cleaned column names, saved CSV.
4. Created line chart (Excel) to visualize trends.

---

## Key observations (brief)

* DALYs were relatively stable (2011–2013), increased notably between 2014–2017 (peak around 2016), fell in 2018, then rose again from 2019 onward.
* The post-2019 rise may relate to political instability, floods, or health system disruptions. The mid-decade spike (2014–2017) requires further investigation.

---

## Next steps (what I will add)

* Compare DALYs vs Death rates (side-by-side chart).
* Compute percentage change (2011→2021) and year-to-year % changes.
* Add annotations for major events (e.g., floods, political events) on the time series.
* (Future) Reproduce analysis in a Jupyter notebook or R script for reproducibility.

---

## How to reproduce / run

1. Download raw GBD malaria data for Sudan from the IHME GBD Results tool: `https://vizhub.healthdata.org/gbd-results/`.
2. Filter by cause = Malaria, measure = DALYs (rate), location = Sudan, years = 2011–2021.
3. Save CSV and follow the cleaning steps in `analysis/analysis_notes.xlsx`.

---

## Contact

If you have feedback, ideas, or collaboration suggestions, please open an issue here or contact me on LinkedIn.

---

*This project is part of my transition from clinical dentistry to public health analytics and epidemiology. I am building my portfolio openly — learning in public.*

### Update —12 Oct 2025: Period analysis & summary statistics

I added a short period analysis and a compact summary table to the workbook:

- **Period Analysis** — the 2011–2021 series is described as three periods:
  - **2011–2016:** Rising (466.15 → 652.61) → **+40.0%**
  - **2016–2018:** Declining (652.61 → 569.20) → **−12.8%**
  - **2019–2021:** Rising again (567.00 → 659.47) → **+16.3%**

- **Analysis Summary** — quick statistics for the whole period:
  - Mean DALYs rate (2011–2021): **552.69** (per 100,000)
  - Min: **459.7** (2012) | Max: **659.47** (2021)
  - Change 2011→2021: **+41.47%**
  - Linear trend (slope): **+19.1 DALYs per 100,000 per year** (R² ≈ 0.70)
  - CAGR: **≈ 3.53% per year**

These additions are in the Excel workbook (`Malaria burden DALYs.xlsx`) on the new sheet named **Period Analysis**. They provide a concise, interpretable summary of the trend and the distinct sub-periods observed in the data. The analysis is descriptive and does not test causal explanations — potential drivers (e.g., interventions, floods, surveillance changes) are noted as hypotheses to explore in future work.

### Update —12 Oct 2025: Trendline, Regression Added

This update improves both the visualization and statistical interpretation of the data:

**1. Chart improvements**
- Added a **linear trendline** with equation and R² displayed on the chart.
- Added a **mean DALYs rate line** for easy visual comparison with yearly fluctuations.
- Updated the Y-axis title to **“DALYs rate — per 100,000 population”**.

**2. Regression analysis**
- Performed a **linear regression (2011–2021)** using Excel’s Data Analysis ToolPak.
- Results show a **positive slope of +19.1 DALYs per year** and **R² = 0.696**, indicating a moderately strong upward trend.
- Regression output is included in the workbook under the “Data Analysis” section.


These additions make the workbook both visually informative and analytically sound, providing a clear picture of malaria DALY trends in Sudan from 2011 to 2021.

### Update —13 Oct 2025: Malaria Death Rate analysis (Sudan, 2011–2021)

I added a second indicator and extended the workbook to include malaria **death rate** analysis alongside the DALYs analysis.

**Files added / updated**
- `Malaria Death Rate.xlsx` — full workbook with three sheets:
  1. **Clean data** (year, rate)
  2. **Chart & regression** (scatter/line chart with trendline, mean line, and Excel Data Analysis regression output)
  3. **Period Analysis & Analysis Summary** (three-period change and concise statistics)


**What I did (methods)**
- Downloaded IHME GBD data for Malaria — Deaths (rate) for Sudan (2011–2021).
- Cleaned and organized the yearly series (CSV).
- Created a time-series chart (Excel) and added a linear trendline (equation + R²) and mean reference line.
- Performed a simple linear regression (Excel Data Analysis ToolPak) to quantify the time trend.
- Divided the series into three sub-periods for interpretable change analysis.

**Key results (short)**
- Mean death rate (2011–2021): **7.68 per 100,000**  
- Min: **6.22 (2012)** — Max: **9.09 (2021)**  
- % Change (2011→2021): **+46.0%**  
- Linear trend (slope): **+0.282 per 100,000 per year** (R² ≈ 0.688, p ≈ 0.0016)  
- CAGR ≈ **3.84%** per year

**Period analysis**
- 2011–2016: rising → **+44.6%**
- 2016–2018: declining → **−14.1%**
- 2019–2021: rising again → **+18.0%**

**Interpretation & limitations**
- The death rate shows a statistically significant upward trend over 2011–2021, with mid-decade fluctuation and renewed increase after 2019. Possible hypotheses include reporting changes, health system disruptions, or environmental factors these require additional data to test.  
- Limitations: only yearly aggregated data, no subnational breakdown or covariates (rainfall, conflict, interventions). Results are descriptive and not causal.



If you have feedback or data suggestions, please open an issue.

