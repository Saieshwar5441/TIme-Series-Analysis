# Time Series Forecasting Projects – Seasonal & Non-Seasonal Analysis

This project applies time series analysis techniques to two real-world domains: **stock price forecasting (seasonal data)** and **public safety analysis (non-seasonal data)**. The goal is to uncover patterns and generate accurate forecasts using ARIMA and SARIMA models.

---

## Project Overview

- **Course:** MA-641 Time Series Analysis  
- **Timeline:** Spring 2024  
- **Author:** Sai Eshwar Gaddipati  
- **Topics:**
  - **Seasonal:** Costco Stock Price Prediction (2021–2024)
  - **Non-Seasonal:** NYPD Daily Shooting Incident Forecasting (Jan–Sep 2024)

---

## Problem Statements

### 1. Costco Stock Price Forecasting
- Analyze seasonal fluctuations in daily closing prices of Costco stock
- Apply SARIMA to capture trend + seasonality
- Help investors and analysts anticipate market behavior

### 2. NYPD Shooting Incident Forecasting
- Examine daily incident trends in New York City
- Use ARIMA to forecast near-future public safety concerns
- Enable law enforcement to allocate resources effectively

---

## Techniques Used

- Time Series Decomposition
- Augmented Dickey-Fuller (ADF) & KPSS Tests
- Differencing & Log Transformation
- ACF and PACF analysis
- ARIMA & SARIMA Modeling
- Model Selection via AIC
- Forecast Accuracy Metrics: RMSE, MAE, MAPE

---

## Files & Structure

- `Seasonal.ipynb` – Costco Stock SARIMA modeling
- `Non_seasonal.ipynb` – NYPD Shooting ARIMA modeling

---

## Key Findings

### Costco Stock Prediction (Seasonal)
- Trend: Strong upward trajectory from 2021 to 2024
- SARIMA captured seasonal patterns effectively
- Forecasts align with market cycles, enabling better decision-making for:
  - Investors (buy/sell timing)
  - Businesses (inventory planning, budget alignment)

### NYPD Shooting Forecasting (Non-Seasonal)
- Daily incidents show no strong seasonality but visible volatility
- ARIMA(1,1,1) chosen for simplicity + strong performance (AIC: 458.4)
- Forecasts showed stable incident counts → helpful for:
  - Law enforcement planning
  - Citywide safety strategy

---

## Evaluation Metrics

| Model         | RMSE  | MAPE (%) | AIC     |
|---------------|-------|----------|---------|
| ARIMA(1,1,1) – NYPD | 0.5964 | 17.88   | 458.4   |
| SARIMA – Costco     | 0.0208 | 0.28    | -4872.99 |

---

## Conclusion

- ARIMA and SARIMA effectively modeled real-world time series data.
- Stock trends benefitted from seasonal decomposition.
- Public safety trends, while volatile, were forecasted reliably with ARIMA.
- Demonstrates the value of statistical modeling in financial and civic applications.

---

## Data Sources

- Costco Stock Data: [Kaggle – Costco Performance](https://www.kaggle.com/datasets/nitirajkulkarni/cost-stock-performance)
- NYPD Shooting Data: [NYC Open Data](https://data.cityofnewyork.us/Public-Safety/NYPD-Shooting-Incident-Data-Year-To-Date-/5ucz-vwe8)

---

## Tools Used

- R (for SARIMA, forecast, tseries, ACF/PACF plots)
- Colab
- Libraries: `forecast`, `tseries`, `ggplot2`, `auto.arima`, `stats`, `Box.test`



