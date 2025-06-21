# COVID-19 Rehabilitation and Outcomes Analysis

This document provides an overview of the scripts and notebooks in the `cv19_statistics` folder, relevant to thesis Chapters 4 and 5. These include the analysis of COVID-19 patient data, rehabilitation pathways, and outcomes. The scripts were used for cohort extraction, propensity matching, survival and regression analysis, and the generation of synthetic (dummy) datasets for evaluation. This also includes the statistical analyses from Chapter 4 based on the data acquired from the [COCHRANE REH-COVER](https://rehabilitation.cochrane.org/special-projects/completed-special-projects/REH-COVER) systematic review series.

Relevant to published work:
> Georgiev, K., et al. "Understanding hospital rehabilitation using electronic health records in patients with and without COVID-19." *BMC Health Serv Res* 24, 1245 (2024). https://doi.org/10.1186/s12913-024-11665-x

---

## Main Notebooks and Scripts

### `LitReview_Exploration.ipynb`
- Jupyter notebook for loading, processing, and visualizing REH-COVER literature review data related to COVID-19 rehabilitation and outcomes.

---

## `rehab_analytics` Subfolder

### `01_EDA.Rmd`
- R Markdown notebook for exploratory data analysis (EDA) of COVID-19 rehabilitation data in NHS Lothian, including data loading, summary statistics, and visualization.

### `02_COVID_pts_extraction.Rmd`
- R Markdown notebook for extracting the COVID-19 patient cohort from raw data sources, including data cleaning and preparation steps.

### `03_COVID_propensity_matching.Rmd`
- R Markdown notebook for performing propensity score matching to balance covariates between COVID-19 patient groups.

### `04_COVID_groups_exploration.Rmd`
- R Markdown notebook for exploring matched patient groups, including group-wise comparisons and descriptive statistics.

### `05_COVID_pts_survival_analysis.Rmd`
- R Markdown notebook for survival analysis among COVID-19 hospitalised patients.

### `06_COVID_regression_analysis.Rmd`
- R Markdown notebook for regression analysis of rehabilitation outcomes, including multivariate modeling and mixed-effects estimation.

---

## `synthetic_pathways` Subfolder

### `dateUtils.R`
- R script providing utility functions for generating and manipulating synthetic date data for simulated patient pathways.

### `generateData.R`
- R script for generating dummy data to support COVID-19 rehabilitation analysis, including basic synthetic episodes, lab tests, and care pathways.

### `generateEvalCohort.R`
- R script for generating evaluation cohorts from synthetic datasets, including cohort selection and adjustment procedures.

### `processMapping.R`
- R script for processing and summarising metadata for process mapping in bupaR.

---