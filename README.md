# Workforce Intelligence & Attrition Analytics Dashboard

**Portfolio Project | HR Analytics | Excel BI**

---

## Project Overview

End-to-end HR analytics solution built in Microsoft Excel using the **IBM HR Analytics Employee Attrition** dataset (1,470 employees, 35 variables). This project demonstrates data cleaning, KPI engineering, risk modeling, pivot-based analysis, executive dashboard design, and consulting-style reporting—skills directly applicable to HR Analytics and People Analytics roles.

**Dataset source:** [IBM HR Analytics Employee Attrition (Kaggle)](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)

---

## Business Problem

Employee attrition creates significant cost and operational risk. Leadership needs a single source of truth to understand *who* is leaving, *why* patterns differ across departments and roles, and *which employees* are at highest risk—so HR can act before turnover occurs.

---

## Key Results

| Metric | Value |
|--------|-------|
| Total Employees | 1,470 |
| Attrition Rate | 16.1% |
| Avg Monthly Salary | $6,503 |
| Avg Tenure | 7.0 years |
| Overtime Rate | 28.3% |
| Overtime Attrition | 30.5% vs 10.4% (non-OT) |

---

## Workbook Structure

| Sheet | Purpose |
|-------|---------|
| `01_Raw_Data` | Unmodified source import |
| `02_Clean_Data` | Power Query cleaned table |
| `03_Helper_Calculations` | Segments, flags, risk scores |
| `04_KPI_Engine` | Single source of truth for KPIs |
| `05_Attrition_Analysis` | Attrition pivot tables & charts |
| `06_Salary_Analysis` | Compensation pivots & charts |
| `07_Risk_Model` | Risk distribution & action lists |
| `08_Dashboard` | Executive visual dashboard |
| `09_Executive_Report` | Consulting-style narrative report |

---

## Technical Skills Demonstrated

- Microsoft Excel (Advanced formulas, Tables, PivotTables, Slicers, Charts)
- Power Query (ETL, data types, deduplication)
- HR Metrics & KPI Design
- Segmentation & Cohort Analysis
- Weighted Risk Scoring Model
- Executive Dashboard Design
- Data Storytelling & Business Recommendations

---

## Tools Used

- Microsoft Excel 365 / Excel 2021
- Power Query
- Python (optional workbook generator: `build_workbook.py`)

---

## Files in This Repository

```
workforce_intelligence/
├── Raw Dataset.csv                          # Source dataset
├── Workforce_Attrition_Dashboard.xlsx     # Built workbook
├── Images                     # Screenshots
└── README.md                              # This file
```

---

## How to Use

1. Open `Workforce_Attrition_Dashboard.xlsx` in Excel.
2. Enable automatic calculation: **Formulas → Calculation Options → Automatic**.
3. Refresh Power Query if you re-import from CSV (Data → Queries & Connections → Refresh).
4. Build pivot tables on sheets 05–07 following the implementation guide in the project documentation.
5. Connect dashboard charts and slicers to pivots on sheet `08_Dashboard`.

---

## Risk Model (Summary)

Composite score (0–100) based on:

- **Age** — younger cohorts weighted higher
- **Salary** — low-income band weighted higher
- **Overtime** — Yes = +25 points
- **Job Satisfaction** — inverse scale
- **Tenure** — 0–2 years weighted highest

**Categories:** Low Risk (&lt;35) | Medium Risk (35–54) | High Risk (≥55)

---


## License

Dataset: IBM HR Analytics (Kaggle). Project code and workbook structure: MIT License.
