This project was developed as an applied statistical exercise in survival analysis, focusing on:

- real-world medical data modeling  
- handling of non-proportional hazards  
- model selection and interpretation in clinical contexts  
- integration of statistical analysis and data # Breast Cancer Survival Analysis 📊

## Project Overview
This project focuses on the survival analysis of breast cancer patients using the SEER (Surveillance, Epidemiology, and End Results) database.

The objective is to identify key clinical, pathological, and biological factors associated with patient survival and to evaluate how their effects evolve over time using both classical and extended survival models.

The analysis combines statistical modeling in R.

---

## 📊 Report

👉 View the report here:  
https://danielemonteverdi02.github.io/breast-cancer-survival-analysis/

---

## 🎯 Objectives
- To analyze survival patterns in breast cancer patients
- To identify significant prognostic factors affecting survival
- To compare non-parametric and semi-parametric survival methods
- To assess the validity of the proportional hazards assumption
- To model time-dependent effects when necessary
- To provide an interactive tool for data exploration

---

## 📁 Dataset
The dataset is derived from the SEER program (National Cancer Institute, USA) and includes 4024 patients diagnosed with invasive breast cancer between 2006 and 2010.

It contains:

- **Demographic variables**: age at diagnosis, ethnicity, marital status  
- **Clinical variables**: tumor size, TNM staging, AJCC stage  
- **Pathological variables**: tumor grade, lymph node involvement  
- **Biomarkers**: estrogen and progesterone receptor status  
- **Survival outcome**: survival time (months) and event indicator  

A derived variable, **LODDS (log-odds of positive lymph nodes)**, is introduced to better capture lymph node involvement.

---

## 🧪 Methods

### Exploratory Analysis
- Summary statistics  
- Correlation analysis  
- Group comparisons (event vs. non-event)

### Survival Analysis
- Kaplan-Meier estimator  
- Log-rank tests for group comparisons  

### Regression Modeling
- Univariate Cox proportional hazards models  
- Multivariate Cox regression  
- Hierarchical model building strategy  

### Model Extensions
- Cox stratified models (for non-proportional hazards)  
- Time-varying covariate effects (for progesterone receptor)  
- Assessment of proportional hazards assumption (Schoenfeld residuals)

### Feature Engineering
- LODDS: log-odds transformation of lymph node status  

---

## 📈 Key Findings
- Lymph node involvement (LODDS) is one of the strongest independent prognostic factors for survival.  
- Tumor stage, histological grade, and tumor size are strongly associated with increased mortality risk.  
- Hormonal receptors (estrogen and progesterone) are associated with significantly better prognosis.  
- The proportional hazards assumption is violated for hormonal receptors, indicating time-dependent effects.  
- Modeling time-varying effects improves interpretability and clinical realism of the Cox model.  
- Stratification and extended Cox models provide a better representation of survival dynamics compared to the standard model.  

---

## 🛠 Tools & Technologies
- R (survival, survminer, tidyverse, gtsummary, pheatmap)  
- Statistical methods: Kaplan-Meier, Cox models, time-dependent Cox models  
