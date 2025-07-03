# CO2-Research-Report

## Abstract
As global CO₂ emissions reach record highs, predictive modeling has become a critical tool for informing climate policy and sustainability planning. In this project, we use country-level data from the Our World in Data (OWID) dataset to forecast future CO₂ emissions based on historical emissions trends and key economic and energy indicators. We implement and compare multiple machine learning models—including Linear Regression, XGBoost, and ARIMAX—evaluating performance using RMSE and MAPE metrics. To improve transparency and interpretability, we apply SHAP to identify the most influential features driving emissions predictions. Our results show that autoregressive models such as ARIMAX outperform other approaches by effectively capturing temporal dependencies in national emission trends. These findings highlight the value of integrating time series analysis with interpretable ML to support evidence-based environmental decision-making.

## Methodology
Data Preprocessing
- Utilized Our World in Data (OWID)'s dataset recording annual emissions per individual country
- Excluded aggregate regions to retain degrees of freedom within data
- Filtered by time period of 1990-2023 to contain consistently reported data
- Standardized numeric features via StandardScaler
- Performed a chronological train/test split of training set (1990-2014) and testing set (2015-2023), testing for temporal generalization (2020-2021 via covid-19)

<br>Models Implemented
- Linear Regression (baseline)
- XGBoost (baseline)
- ARIMAX (time-series)

<br>Metrics Measured
- Root Mean Square Error (RMSE)
- Mean Absolute Percentage Error (MAPE)
- Explainability (feature coefficients / SHAP)

## Results
