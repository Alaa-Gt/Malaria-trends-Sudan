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
