# 📈 Superstore Sales Forecasting and Time Series Analysis

## Overview

This project performs **Exploratory Data Analysis (EDA)** and **Time Series Forecasting** on retail sales data from a Superstore dataset. The objective is to analyze historical sales patterns across different product categories and forecast future sales using **SARIMA (Seasonal ARIMA)** models.

The project covers the complete workflow from data preprocessing and visualization to model building, forecasting, and performance evaluation.

---

## Features

- Data cleaning and preprocessing
- Date feature engineering
- Exploratory Data Analysis (EDA)
- Regional and geographical sales analysis
- Monthly sales trend analysis
- Time series decomposition
- Stationarity testing using ADF Test
- Autocorrelation (ACF) and Partial Autocorrelation (PACF) analysis
- SARIMA/SARIMAX forecasting models
- Six-month sales forecasting
- Model performance evaluation using MAPE

---

## Dataset

The project uses the Superstore retail dataset containing:

- Order information
- Sales data
- Product categories
- Customer locations
- Regions and states

Dataset source:

https://confrecordings.ams3.digitaloceanspaces.com/JDS/EXPL2/Chp11/superstore.csv

---

## Product Categories Analyzed

The forecasting models are built separately for:

- 🪑 Furniture
- 🏢 Office Supplies
- 💻 Technology

---

## Project Workflow

### 1. Data Preprocessing

- Load dataset using Pandas
- Convert order dates to datetime format
- Create additional date-based features:
  - Year
  - Month
  - Day
  - Day of Week
  - Year-Month

### 2. Exploratory Data Analysis

Visualizations include:

- Orders by State
- Orders by Region
- Top 20 Cities by Order Count
- Monthly Order Trends
- Category-wise Sales Trends

### 3. Time Series Preparation

For each category:

- Aggregate daily sales
- Convert to monthly average sales
- Create category-specific time series

### 4. Time Series Diagnostics

- Augmented Dickey-Fuller (ADF) Test
- Seasonal Differencing
- Seasonal Decomposition
- Trend Analysis
- ACF and PACF plots

### 5. Forecasting

SARIMAX models are trained for:

| Category | Model Parameters |
|-----------|------------------|
| Technology | SARIMAX(1,1,1)(1,1,2,12) |
| Office Supplies | SARIMAX(1,1,1)(1,1,2,12) |
| Furniture | SARIMAX(5,1,10)(1,0,0,12) |

### 6. Evaluation

Models are evaluated using:

- Mean Absolute Percentage Error (MAPE)
- Forecast Accuracy

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Statsmodels

                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  
