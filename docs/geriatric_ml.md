# Geriatric Machine Learning (CIPR - Care Intensity PRediction) Analytics

This document provides an overview of the notebooks in the `geriatric_ml` folder used to generate the analyses in Chapter 8. These notebooks cover the workflow for machine learning analysis, including cohort definition, feature engineering, model development, evaluation, and interpretation. The workflow is relevant to the development and validation of predictive models for healthcare needs and hospital outcomes in older patients.

Relevant to published and upcoming work:
> Georgiev, K., McPeake, J., Shenkin, S.D. et al. "Understanding hospital activity and outcomes for people with multimorbidity using electronic health records". *Sci Rep* 15, 8522 (2025). https://doi.org/10.1038/s41598-025-92940-7

---

## Main Notebooks and Scripts

### `01 CIPR Outcome Definition.ipynb`
- Defines the NHSL-specific cohort for care contacts prediction.
- Loads and explores input data and care contact groupings.

### `02 CIPR Feature Extraction.ipynb`
- Generates features from RCHD for ML predictions of hospital outcomes and healthcare contacts.
- Loads routine data, cohort, comorbidities, and geriatric risk assessments data.

### `03 CIPR Feature Selection.ipynb`
- Implements feature selection and train/validation split pipeline.
- Includes helper-functions for visualising patient characteristics.

### `04 CIPR Classification.ipynb`
- Develops and evaluates classification models for all secondary hospital endpoints.
- Loads features, sets up file paths, and manages data types.

### `05 CIPR Regression.ipynb`
- Implements regression models for healthcare contacts and related outcomes.
- Loads training data and relevant features.

### `06 CIPR Competing Risks.ipynb`
- Analyses competing risks using survival analysis methods.
- Loads validation data, sets target groups, and merges with outcome data.

### `07 CIPR Cross-validation.ipynb`
- Performs K-fold cross-validation (SKCV) for regression and classification models.

### `08 CIPR Trajectory Plotting.ipynb`
- Plots model performance trajectories across outcomes and admission timepoints.
- Loads results tables and visualizes ROC-AUC and other metrics.

### `09 CIPR Model Comparison.ipynb`
- Compares discrimination across various regression models.

### `10 CIPR Patient Characteristics.ipynb`
- Explores relationships between hospital outcomes, rehabilitation activity, and demographic history.
- Loads cohort for the summary of baseline characteristics, risk assessments and care contacts data.

### `11 CIPR Missingness.ipynb`
- Analyses missing data by outcome groups.
- Explores the impact of missingness on model development and evaluation.

---
