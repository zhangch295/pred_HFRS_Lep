# pred_HFRS_Lep

Multi-source data-driven prediction models for **Hemorrhagic fever with renal syndrome (HFRS)** and **Leptospirosis**.

本项目用于整理和展示 Hemorrhagic fever with renal syndrome (HFRS) 与 Leptospirosis 发病趋势预测研究的主要分析流程，包括多源数据整合、时间序列特征构建、趋势与季节性分析、预测建模、模型评估和结果解释等内容。

## 1. Background

Hemorrhagic fever with renal syndrome (HFRS) and Leptospirosis are important zoonotic infectious diseases that remain public health concerns in many regions. Their occurrence and transmission are influenced by climatic conditions, ecological environment, population-related factors, socioeconomic development and seasonal variation.

Accurate prediction of HFRS and Leptospirosis incidence can support early warning, risk assessment and targeted prevention strategies. However, the nonlinear relationships between disease incidence and multiple external drivers make prediction challenging.

In this study, we developed a multi-source data-driven modelling framework to characterize the temporal dynamics of HFRS and Leptospirosis and predict their future incidence trends.

## 2. Study Objectives

This project aims to:

1. Describe long-term trends and seasonal patterns of HFRS and Leptospirosis.
2. Integrate disease surveillance data with climatic, environmental and socioeconomic predictors.
3. Develop prediction models for monthly disease incidence.
4. Compare the predictive performance of different modelling strategies.
5. Identify key predictors associated with disease dynamics.
6. Provide a reproducible analytical framework for zoonotic disease prediction and early warning.

## 3. Data Sources

The analysis was based on monthly disease surveillance data and multi-source covariates.

### 3.1 Disease Surveillance Data

- Monthly reported cases of HFRS
- Monthly reported cases of Leptospirosis
- Study period: January 2010 to December 2025
- Temporal resolution: monthly

### 3.2 Multi-source Predictors

Candidate predictors included:

- Temporal and seasonal indicators
- Lagged disease incidence
- Meteorological variables
- Environmental and ecological indicators
- Remote sensing-derived variables
- Socioeconomic indicators
- Population-related indicators

Due to restrictions on surveillance data sharing, raw case data may not be publicly available. Where possible, example data or processed templates can be provided to illustrate the expected data format.

## 4. Methodological Framework

The overall workflow consisted of the following steps:

```text
Disease surveillance data
        +
Multi-source predictors
        ↓
Data cleaning and monthly aggregation
        ↓
Feature engineering
        ↓
Exploratory temporal analysis
        ↓
Trend and seasonal decomposition
        ↓
Prediction model development
        ↓
Model evaluation and comparison
        ↓
Model interpretation
        ↓
Visualization and result reporting
```

## 5. Feature Engineering

Feature construction included:

- Time variables, such as year, month and seasonal indicators
- Lagged incidence features
- Lagged climatic and environmental variables
- Rolling-window statistics
- Long-term trend indicators
- Seasonal cycle indicators
- Disease-specific feature sets for HFRS and Leptospirosis

These features were used to capture autocorrelation, delayed environmental effects, seasonality and nonlinear associations between predictors and disease incidence.

## 6. Modelling Strategy

Several modelling strategies were considered and compared.

### 6.1 Baseline Models

Baseline models were used to capture historical temporal patterns and provide reference performance.

### 6.2 Statistical Time-series Models

Time-series models were used to account for autocorrelation, trend and seasonality in monthly disease incidence.

### 6.3 Machine Learning Models

Machine learning models were used to capture nonlinear associations and interactions among multi-source predictors.

### 6.4 Model Interpretation

Feature importance and interpretable machine learning approaches were used to identify major predictors contributing to disease prediction.

## 7. Model Evaluation

Model performance was evaluated using commonly used prediction metrics, including:

- Root Mean Squared Error, RMSE
- Mean Absolute Error, MAE
- Mean Absolute Percentage Error, MAPE
- Coefficient of determination, R²

Observed and predicted incidence curves were compared visually to assess model fit, prediction accuracy and temporal consistency.

## 8. Main Outputs

The project generates the following types of outputs:

- Monthly incidence trend plots
- Seasonal pattern visualizations
- Time-series decomposition results
- Observed versus predicted incidence curves
- Model performance comparison tables
- Feature importance results
- Model interpretation plots
- Disease-specific prediction results for HFRS and Leptospirosis

## 9. Results Summary

The analysis showed that HFRS and Leptospirosis exhibited distinct temporal patterns, including long-term changes and seasonal fluctuations. Models incorporating lagged disease incidence and multi-source external predictors generally achieved better prediction performance than simple baseline approaches.

Environmental, climatic and temporal features contributed to disease prediction, suggesting that multi-source data integration can improve the understanding and forecasting of zoonotic disease dynamics.

The proposed framework may provide methodological support for disease surveillance, early warning and public health decision-making.

## 10. Reproducibility

To reproduce the analytical workflow, users should prepare monthly disease data and covariates in a standardized format.

Example data structure:

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

A typical reproduction process includes:

1. Preparing monthly disease surveillance data.
2. Preparing corresponding multi-source predictors.
3. Conducting data cleaning and feature engineering.
4. Performing descriptive and seasonal analyses.
5. Developing and evaluating prediction models.
6. Generating figures and summary tables.

## 11. Citation

If you use or adapt this project, please cite the related study:

```text
Zhang C, et al. Multi-source data-driven prediction of Hemorrhagic fever with renal syndrome and Leptospirosis. Manuscript in preparation.
```

The formal citation will be updated after publication.

## 12. License

This project is intended for academic research and non-commercial use. Please refer to the license information in this repository for details.

## 13. Contact

For questions, suggestions or collaboration, please contact:

```text
Zhang Chi
Changsha Center for Disease Control and Prevention
Email: [your-email@example.com]
```

## 14. Disclaimer

This repository is intended for scientific research and methodological reference. Prediction results should not be used as the sole basis for public health decision-making. Any operational application should be combined with routine surveillance, field epidemiological investigation, expert assessment and local public health context.
