# Melbourne Housing — Capstone Project

**Student:** naif ali ayed bin dair
**Dataset:** Melbourne Housing Snapshot  

---

## Project Overview

This project builds a complete data analysis pipeline on the Melbourne Housing dataset, covering data cleaning, feature engineering, exploratory data analysis, and foundational mathematics.

## Key Results

- **Strongest predictor:** Region (Southern Metropolitan properties sell for ~2× the price of Western Metropolitan)
- **Price driver:** Rooms and building area are the top numeric correlates with price
- **Data quality:** ~47% of `BuildingArea` values were missing; filled using group-median by property type
- **Outliers:** Price capped at 99th percentile (~AUD 3.8M) to reduce leverage of ultra-luxury sales

## Notes

- All file paths are **relative** — the project can be run from any machine.
- All charts are saved to `report_assets/` automatically when notebooks are run.
- AI assistance was used for code structuring and debugging. All analysis decisions and explanations are the student's own work.
