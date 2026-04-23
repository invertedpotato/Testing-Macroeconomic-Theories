# Testing-Macroeconomic-Theory
Empirically testing macroeconomic theories using real world data
# Empirical Testing of Macroeconomic Theory

**Python | Pandas | Statsmodels | FRED API**

## Overview

This project tests standard macroeconomic theories (IS-LM model, labor market dynamics, Keynesian GDP) using historical U.S. data from 1980–2024. All data was retrieved via the FRED API.

## Key Empirical Results

### 1. IS Curve Validation
- **Finding:** Real private investment has a statistically significant negative relationship with the federal funds rate
- **Interpretation:** Empirically confirms the downward slope of the IS curve

### 2. Labor Market Dynamics
- **Finding:** Industrial Production and Nonfarm Employment show a robust positive relationship
- **Interpretation:** Validates standard labor demand theory

### 3. Money Demand (LM Curve)
- **Finding:** Income elasticity of money demand = 1.13
- **Finding:** Inverse relationship between interest rates and real money balances confirmed

### 4. Recession Forecasting
- **Finding:** 10yr-2yr Treasury yield curve predicts NBER recessions with **~78% accuracy**
- **Method:** Historical analysis of yield curve inversions preceding recessions

### 5. GDP Determinants
- **Finding:** Consumption, investment, government spending, and unemployment explain **>96% of GDP variation** (R² = 0.96+)
- **Method:** Stepwise multiple regression
- **Interpretation:** Largely confirms the Keynesian expenditure approach

## Data Sources

- **FRED API (Federal Reserve Economic Data)**
  - Federal funds rate
  - Real private investment
  - Industrial production
  - Nonfarm employment
  - Money supply measures
  - Treasury yields (10yr, 2yr)
  - GDP and components
  - Unemployment rate

## Methods Used

- Linear regression
- Multiple regression (stepwise selection)
- Log-log models (elasticity estimation)
- Time series analysis
- Hypothesis testing

## How to Run

1. Clone this repository
2. Install requirements: `pip install -r requirements.txt`
3. Obtain a free FRED API key [here](https://fred.stlouisfed.org/docs/api/api_key.html)
4. Add your API key to the notebook (or use environment variable)
5. Run `macroeconomics_analysis.ipynb`

## Requirements

- Python 3.8+
- pandas
- numpy
- statsmodels
- matplotlib
- fredapi (for FRED API access)

## Author

Ashvin Budhiraja | ashvinbudhiraja9@gmail.com | 
