# Panel Econometric Analysis of Retail Discount Strategies

## Overview

This project investigates the dynamic impact of promotional discount strategies on retail beverage revenue using advanced panel econometric techniques and machine learning.

The dataset consists of approximately two years of daily observations across 37 retail stores, providing a rich panel structure for analysing both short-run and medium-run responses to promotional activity. A major econometric challenge arises from strong cross-sectional dependence, where nationwide demand shocks, holidays, seasonal effects, and macroeconomic conditions simultaneously influence all stores.

To address this issue, the study applies Common Correlated Effects Mean Group (CCEMG) estimation to explicitly model latent common factors and eliminate spurious cross-sectional relationships. The analysis then combines causal inference, panel Granger non-causality testing, and machine learning methods to identify genuine revenue responses attributable to discount interventions.

The project demonstrates how modern econometric methods can be integrated with predictive analytics to improve both causal interpretation and forecasting performance in large-scale retail systems.

---

## Research Questions

1. Do promotional discounts genuinely increase retail revenue?

2. Are observed causal relationships robust after correcting for cross-sectional dependence?

3. How persistent are the effects of promotional activity?

4. Can machine learning models improve prediction accuracy beyond traditional econometric approaches?

5. What implications do discount strategies have for long-term revenue optimisation?

---

## Dataset

| Feature | Description |
|----------|-------------|
| Stores | 37 retail stores |
| Frequency | Daily observations |
| Duration | Approximately 2 years |
| Target Variable | Beverage revenue |
| Key Explanatory Variable | Promotional discounts |
| Data Structure | Balanced panel dataset |

---

## Methodology

### Econometric Framework

- Panel Data Analysis
- Fixed Effects Models
- Cross-Sectional Dependence Testing
- Common Correlated Effects Mean Group (CCEMG)
- Panel Granger Non-Causality Testing
- Dynamic Lag Structure Analysis

### Machine Learning Framework

- LightGBM
- SHAP Explainability
- Residual Modelling
- Hybrid Econometric–Machine Learning Pipeline

### Statistical Validation

- Robustness Checks
- Residual Diagnostics
- Sensitivity Analysis
- Out-of-Sample Evaluation

---

## Key Findings

### Cross-Sectional Dependence Creates Spurious Causality

Initial Granger causality tests suggested widespread and highly significant relationships between discount activity and revenue performance.

However, dependence diagnostics revealed that much of this significance was driven by latent common factors affecting all stores simultaneously. Without correcting for these factors, causal conclusions would be severely overstated.

### CCEMG Removes Common-Factor Contamination

After applying Common Correlated Effects Mean Group estimation, the majority of previously identified causal relationships disappeared.

This demonstrates that controlling for cross-sectional dependence is essential when analysing retail panels exposed to shared economic shocks.

### Discounts Increase Revenue in the Short Run

Corrected causal estimates indicate that promotional discounts generate statistically significant short-run revenue gains.

The strongest effects occur immediately following promotional activity, supporting the effectiveness of temporary discount campaigns as a tactical sales mechanism.

### Evidence of Inter-Temporal Demand Substitution

Revenue gains were not fully permanent.

Higher sales during promotional periods were partially offset by reduced demand in subsequent periods, suggesting that discounts often shift future purchases forward rather than generating entirely new demand.

### Hybrid Models Improve Forecasting Performance

LightGBM models applied to the econometric residual structure captured nonlinear relationships not explained by traditional panel models.

The resulting hybrid framework achieved superior predictive performance while retaining interpretability through SHAP-based feature attribution.

---

## Technical Skills Demonstrated

### Econometrics

- Panel Data Econometrics
- Common Correlated Effects Mean Group (CCEMG)
- Fixed Effects Estimation
- Cross-Sectional Dependence Analysis
- Dynamic Causal Inference
- Panel Granger Non-Causality Testing

### Statistics

- Statistical Inference
- Hypothesis Testing
- Model Diagnostics
- Robustness Analysis
- Forecast Evaluation

### Machine Learning

- LightGBM
- Explainable AI (SHAP)
- Feature Importance Analysis
- Hybrid Statistical Learning Models

### Programming

- R
- Python
- Data Visualisation
- Reproducible Research Workflows

---

## Repository Structure

```text
panel-econometrics-discount-analysis/
│
├── README.md
├── report/
│   └── final_report.pdf
│
├── data/
│   ├── raw/
│   └── processed/
│
├── scripts/
│   ├── preprocessing.R
│   ├── panel_models.R
│   ├── ccemg_analysis.R
│   ├── granger_tests.R
│   ├── lightgbm_model.py
│   └── diagnostics.R
│
├── figures/
│   ├── revenue_trends.png
│   ├── causality_results.png
│   ├── shap_summary.png
│   └── model_comparison.png
│
└── presentation/
    └── slides.pdf
```

---

## Technologies Used

- R
- Python
- LightGBM
- SHAP
- tidyverse
- plm
- ggplot2

---

## Repository Topics

```text
econometrics
panel-econometrics
causal-inference
cross-sectional-dependence
ccemg
granger-causality
statistical-learning
lightgbm
machine-learning
rstats
```

---

## Author

Kan Kai Zheng

BSc (Hons) Mathematics and Data Science  
University of Nottingham Malaysia

Research Interests:
- Econometrics
- Statistical Finance
- Machine Learning
- Causal Inference
- Quantitative Research
