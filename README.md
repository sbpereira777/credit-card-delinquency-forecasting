# Credit Card Delinquency Forecasting using Time Series Analysis

## Overview
This project analyzes and forecasts the **US Credit Card Delinquency Rate** using time series techniques.  
The objective is to understand historical patterns and build a model for predicting future credit risk.

---

## Dataset
- Source: FRED (Federal Reserve Economic Data)  
- Series: DRCCLACBS (Delinquency Rate on Credit Card Loans)  
- Time Period: 1991 – 2025  
- Frequency: Quarterly  

---

## Methodology

### 1. Data Preprocessing
- Converted date column into time index  
- Checked for missing values and consistency  

### 2. Stationarity Testing
- Applied **Augmented Dickey-Fuller (ADF) Test**  
- Observed non-stationarity (p-value > 0.05)  
- Applied **first differencing**  
- Achieved stationarity (p-value < 0.05)  

### 3. Time Series Analysis
- Visualized trend and patterns  
- Used **ACF and PACF plots** to identify model structure  

### 4. Model Building
- Built an **ARIMA model**  
- Selected optimal parameters using AIC  
- Verified residuals behave like white noise  

### 5. Forecasting
- Generated future delinquency rate forecasts  
- Interpreted results for risk analysis  

---

## Key Insights
- Clear spike observed during the **2008 financial crisis**  
- Original series was non-stationary and required differencing  
- ARIMA captured temporal dependence effectively  
- Forecasting helps in **credit risk monitoring and stress analysis**  

---

## Tools & Libraries
- Python  
- Pandas  
- NumPy  
- Statsmodels  
- Matplotlib  

---

