# Melbourne Housing — Capstone Project

**Student:** naif ali ayed bin dair  
**Course:** ML Foundations Bootcamp  
**Dataset:** Melbourne Housing Snapshot  

---

## Project Overview

This project builds a complete data analysis pipeline on the Melbourne Housing dataset, covering data cleaning, feature engineering, exploratory data analysis, and foundational mathematics.

## Repository Structure

```
my-capstone/
├── 01_cleaning.ipynb       # Phase 1 — Load, Explore & Clean
├── 02_features.ipynb       # Phase 2 — Feature Engineering
├── 03_eda.ipynb            # Phase 3 — EDA & Visualisation
├── 04_math.ipynb           # Phase 3 (cont.) — Math Basics
├── report.md               # Written report (2-3 pages)
├── README.md               # This file
├── requirements.txt        # Python dependencies
├── data/
│   ├── raw/
│   │   └── melb_data.csv   # Original dataset
│   └── cleaned/
│       ├── melb_cleaned.csv    # Output of 01_cleaning.ipynb
│       └── melb_features.csv   # Output of 02_features.ipynb
└── report_assets/          # Charts saved by notebooks
```

## How to Run

1. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

2. **Run notebooks in order** (each one depends on the output of the previous):
   ```
   01_cleaning.ipynb  →  02_features.ipynb  →  03_eda.ipynb  →  04_math.ipynb
   ```

3. Use **Kernel → Restart & Run All** in Jupyter to verify each notebook runs clean from top to bottom.

## Key Results

- **Strongest predictor:** Region (Southern Metropolitan properties sell for ~2× the price of Western Metropolitan)
- **Price driver:** Rooms and building area are the top numeric correlates with price
- **Data quality:** ~47% of `BuildingArea` values were missing; filled using group-median by property type
- **Outliers:** Price capped at 99th percentile (~AUD 3.8M) to reduce leverage of ultra-luxury sales

## Notes

- All file paths are **relative** — the project can be run from any machine.
- All charts are saved to `report_assets/` automatically when notebooks are run.
- AI assistance was used for code structuring and debugging. All analysis decisions and explanations are the student's own work.
