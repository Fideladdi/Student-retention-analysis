# student-retention-analysis

> CRISP-DM pipeline for predicting and understanding student retention at a post-secondary institution.

## Overview

This project applies the **CRISP-DM** (Cross-Industry Standard Process for Data Mining) framework to analyze and model student retention across **9 cohorts** (Fall 2016 – Fall 2024) at a hypothetical Alberta post-secondary institution.

| Scope | Detail |
|---|---|
| Students | 25,414 |
| Schools | 7 (anonymized: A–G) |
| Programs | 61 |
| Dataset rows | 1,522 aggregated groups |
| Source file | `RetentionData_Final.csv` |

Each row in the dataset represents a **group of students** sharing the same school, program, national status, admission pathway, and admit term — not an individual student.

## Project Structure

```
student-retention-analysis/
├── RetentionAnalysis_CRISPDM.ipynb   # Main analysis notebook
├── RetentionData_Final.csv           # Source dataset
└── README.md
```

## CRISP-DM Workflow

The notebook follows the full CRISP-DM pipeline:

1. **Business Understanding** — Define retention goals and institutional context
2. **Data Understanding** — Inspect data types, completeness, and distributions
3. **Data Preparation** — Clean, transform, and engineer features
4. **Modelling** — Build and tune predictive models
5. **Evaluation** — Assess model performance and interpret results
6. **Deployment** — Summarize findings and recommendations

## Key Variables

- `AdmitTerm` — Fall cohort year (e.g. Fall 2016)
- `School` — One of 7 anonymized schools
- `Program` — One of 61 academic programs
- `NationalStatus` — Domestic / International
- `AdmissionPathway` — How students were admitted
- Retention metrics — Year-over-year continuation rates

## Tech Stack

- **Python** — pandas, NumPy, scikit-learn, matplotlib / seaborn
- **Jupyter Notebook**
- Framework: **CRISP-DM**

## Getting Started

```bash
git clone https://github.com/<your-username>/student-retention-analysis.git
cd student-retention-analysis
pip install pandas numpy scikit-learn matplotlib seaborn jupyter
jupyter notebook RetentionAnalysis_CRISPDM.ipynb
```


## License

For academic and research use only. Dataset is hypothetical.
