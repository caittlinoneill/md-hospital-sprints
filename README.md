# md-hospital-sprints
Maryland hospital star ratings for INST 414 project


readme_text = """# Maryland Hospital Star Ratings (QSSR Capstone)

## Project Overview
This project analyzes CMS Overall Hospital Quality Star Ratings for hospitals in Maryland. The goal is to examine whether hospital ownership, emergency service availability, and county location help explain variation in star ratings. The project follows the Quantitative Social Science Research (QSSR) track and emphasizes interpretation, statistical modeling, and policy-relevant insights rather than prediction.

Sprint 3 focuses on model development, evaluation, and interpretation.


## Data
Primary dataset:
Hospital General Information (2016–2020), sourced from Kaggle and originally published by the Centers for Medicare & Medicaid Services (CMS).

File used in this repository:
data/Hospital_General_Information_2016_2020.csv

The dataset is filtered to Maryland hospitals and the 2020 reporting year.

## Repository Structure
md-hospital-sprints/
│
├── data/
│   └── Hospital_General_Information_2016_2020.csv
│
├── notebooks/
│   └── Sprint3_Modeling.ipynb
│
├── results/
│   ├── figures/
│   │   ├── fig1_residuals_vs_fitted.png
│   │   └── fig2_coefficient_plot.png
│   │
│   └── tables/
│       ├── table1_main_regression_results.csv
│       └── table2_model_comparison.csv
│
└── README.md


## Modeling and Analysis
The primary analysis uses an ordinary least squares (OLS) regression to estimate the relationship between hospital star ratings and institutional and geographic characteristics. The main model includes hospital ownership type, emergency service availability, and county indicator variables.

A baseline mean-only model is estimated for comparison. Model evaluation focuses on explanatory power, coefficient interpretation, and regression diagnostics rather than prediction accuracy.


## Model Artifacts
Because this project emphasizes interpretability over deployment, model artifacts are not saved as serialized objects. Instead:
- Full model specifications and results are documented in the notebook
- Regression tables are exported as CSV files in results/tables/
- Diagnostic and interpretive figures are stored in results/figures/

This approach aligns with standard QSSR practices for transparency and reproducibility.


## Results and Figures
Figures used in the Sprint 3 report are stored in results/figures/ and include:
- Residuals vs fitted values plot for model diagnostics
- Coefficient plot visualizing estimated effects of hospital ownership and county location

Regression result tables and model comparison summaries are stored in results/tables/.

## How to Reproduce the Analysis
1. Open notebooks/Sprint3_Modeling.ipynb
2. Run cells top-to-bottom
3. The notebook reproduces all models, tables, and figures discussed in the Sprint 3 report

Figures included in results/figures/ correspond to outputs shown in the notebook.


## Sprint 3 Status
Sprint 3 is complete. The repository includes documented modeling code, reproducible results, regression tables, and figures suitable for policy and equity-focused interpretation.

Sprint 4 will focus on refining interpretation and communicating findings to a non-technical audience.
"""

with open("README.md", "w") as f:
    f.write(readme_text)

print("README.md created successfully.")
