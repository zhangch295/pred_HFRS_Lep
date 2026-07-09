# pred_HFRS_Lep

**pred_HFRS_Lep** provides the analytical framework and documentation for the study of multi-source data-driven prediction of:  

*Hemorrhagic fever with renal syndrome (HFRS) and Leptospirosis.*

---

## 🧩 Overview

This repository is designed to support the prediction and interpretation of the temporal dynamics of **Hemorrhagic fever with renal syndrome (HFRS)** and **Leptospirosis**.

The study integrates disease surveillance data with multi-source predictors, including meteorological, environmental, ecological, socioeconomic and temporal features. The overall aim is to characterize long-term trends, seasonal patterns and potential drivers of HFRS and Leptospirosis, and to develop predictive models for disease risk assessment and early warning.

The repository currently focuses on the methodological framework, data structure description, modelling strategy and result interpretation. Detailed code files are not displayed at this stage and will be updated in future releases.

---

## 📂 Data Availability

The analysis is based on monthly disease surveillance data and multi-source covariates from January 2010 to December 2025.

Due to restrictions on surveillance data sharing, the original case-level or raw surveillance data are not publicly distributed in this repository. Processed templates or example data structures may be provided where appropriate to illustrate the required input format.

The data used or considered in this project include:

- Monthly reported cases of **Hemorrhagic fever with renal syndrome (HFRS)**
- Monthly reported cases of **Leptospirosis**
- Meteorological variables
- Environmental and ecological indicators
- Remote sensing-derived indicators
- Socioeconomic indicators
- Population-related variables
- Temporal and seasonal features
- Lagged disease and environmental features

Example data format:

```text
date,disease,cases,incidence
2010-01,HFRS,xx,xx
2010-02,HFRS,xx,xx
2010-03,HFRS,xx,xx
2010-01,Leptospirosis,xx,xx
2010-02,Leptospirosis,xx,xx
2010-03,Leptospirosis,xx,xx
```

Recommended date format:

```text
YYYY-MM
```

---

## ⚙️ Methodological Framework

The analytical framework consists of the following major components.

### Data preprocessing and integration

The study first harmonizes monthly disease surveillance data and multi-source predictors into a unified time-series dataset. Data preprocessing includes date formatting, missing value handling, monthly aggregation, feature matching and disease-specific dataset construction.

### Exploratory temporal analysis

Temporal analyses are conducted to describe the monthly incidence patterns of HFRS and Leptospirosis. These analyses are used to examine long-term trends, seasonal fluctuations and differences in temporal dynamics between the two diseases.

### Trend and seasonal decomposition

Time-series decomposition methods are used to separate observed disease incidence into trend, seasonal and residual components. This step helps reveal the underlying temporal structure of HFRS and Leptospirosis and supports subsequent predictive modelling.

### Feature engineering

Feature construction includes temporal variables, seasonal indicators, lagged incidence terms, lagged meteorological and environmental variables, rolling-window statistics and disease-specific predictors. These features are designed to capture autocorrelation, delayed environmental effects, seasonality and nonlinear associations.

### Prediction modelling

Multiple modelling strategies are considered, including baseline models, statistical time-series models and machine learning models. The modelling framework aims to compare the predictive value of historical incidence, temporal features and multi-source external predictors.

### Model evaluation

Model performance is evaluated using standard prediction metrics, including:

- Root Mean Squared Error, RMSE
- Mean Absolute Error, MAE
- Mean Absolute Percentage Error, MAPE
- Coefficient of determination, R²

Observed and predicted incidence curves are also compared to assess prediction accuracy and temporal consistency.

### Model interpretation

Interpretable modelling approaches are used to identify important predictors associated with disease dynamics. Feature importance and related interpretation methods help evaluate the contribution of climatic, environmental, temporal and socioeconomic factors to disease prediction.

---

## 📊 Main Outputs

The project generates the following types of outputs:

- Monthly incidence trend plots
- Seasonal pattern visualizations
- Time-series decomposition results
- Observed versus predicted incidence curves
- Model performance comparison tables
- Feature importance results
- Model interpretation plots
- Disease-specific prediction results for HFRS
- Disease-specific prediction results for Leptospirosis

---

## 📌 Results Summary

The analysis suggests that HFRS and Leptospirosis show distinct temporal patterns, including long-term changes and seasonal fluctuations. Models incorporating lagged disease incidence and multi-source predictors generally provide improved prediction performance compared with simple baseline approaches.

Meteorological, environmental, ecological and temporal features may contribute to disease prediction, indicating that multi-source data integration can improve the understanding and forecasting of zoonotic disease dynamics.

The proposed framework may provide methodological support for disease surveillance, risk assessment, early warning and targeted public health interventions.

---

## 🔁 Reproducibility

To reproduce the analytical workflow, users should prepare monthly disease data and corresponding predictors in a standardized format.

A typical reproduction process includes:

1. Preparing monthly disease surveillance data.
2. Preparing corresponding multi-source predictors.
3. Conducting data cleaning and feature engineering.
4. Performing descriptive temporal analysis.
5. Conducting trend and seasonal decomposition.
6. Developing and evaluating prediction models.
7. Generating figures and summary tables.
8. Interpreting key predictors and disease-specific results.

Detailed code files are not displayed at this stage. Future updates may include reproducible scripts, example datasets, figure-generation workflows and additional documentation.

---

## 📖 Citation

If you use this project or adapt the analytical framework in your research, please cite the related article:

> Upcoming update

---

## 📜 License

This project is intended for academic research and non-commercial use.  
License information will be updated in future releases.

---

## 📬 Contact

For questions, suggestions or collaboration, please contact:

```text
Zhang Chi
Changsha Center for Disease Control and Prevention
Email: [Upcoming update]
```

---

## ⚠️ Disclaimer

This repository is intended for scientific research and methodological reference. Prediction results should not be used as the sole basis for public health decision-making. Any operational application should be combined with routine surveillance, field epidemiological investigation, expert assessment and local public health context.

---
