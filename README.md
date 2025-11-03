# FUTURE_ML_01 - AI Powered Sales Forecasting System

## 🎯 Projecy Overview
This project delivers an end-to-end workflow for monthly retail sales forecasting and dashboarding.
It uses Python (Prophet) for time series modeling and Power BI for interactive visualizations, enabling actionable insights for business decisions.

## Features
- Automated data cleaning and aggregation in Python
- Prophet-based time series forecasting
- Export of forecast and actuals to CSV for BI usage
- Power BI dashboard with:
- Actual vs. forecasted sales trend line
- Monthly and yearly comparison charts

## Data Source: 
-Sample Superstore/retail sales CSV (columns used: Order Date, Sales, [Category/Region/Store, ...])

After cleaning: aggregated as monthly sales for model building and dashboarding

Workflow
1. Python Data Preparation
Load CSV and handle encoding issues

Clean data, drop duplicates, handle missing values

Group and aggregate sales by month using pd.resample('ME')

Export to monthly_actuals.csv
