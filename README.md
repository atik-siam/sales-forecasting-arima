# Sales Forecasting for Retail Demand using ARIMA

## Overview
This project develops a time series forecasting model to predict monthly retail sales, with the goal of supporting short-term business decision-making such as inventory planning and demand estimation.

## Dataset
- Supermarket sales dataset
- Aggregated into monthly time series
- Time span: [ADD THIS — e.g., Jan 2018 – Dec 2020]
- Total observations: [ADD NUMBER]

## Methodology
- Aggregated daily sales into monthly totals
- Performed exploratory data analysis (trend and variability)
- Applied log transformation to stabilize variance
- Conducted stationarity testing using Augmented Dickey-Fuller (ADF)
- Built ARIMA(1,1,0) model for forecasting
- Performed residual diagnostics (ACF plots, Ljung-Box test)
- Generated forecasts and converted back to original scale

## Model Evaluation
- Forecast horizon: 6 months
- Mean Absolute Percentage Error (MAPE): ~36%
- Symmetric MAPE (sMAPE): ~47%

## Key Insights
- The model captures the overall sales trend but struggles with sudden fluctuations
- Forecast uncertainty increases significantly for longer horizons
- Model performance suggests that additional variables (e.g., promotions, seasonal effects) could improve accuracy

## Business Implications
- Provides a baseline forecast for short-term inventory planning
- Helps identify expected demand trends over the next 6 months
- Can be used as a starting point for more advanced forecasting systems incorporating external factors

## Limitations
- Limited historical data reduces predictive performance
- No inclusion of external drivers such as promotions, holidays, or economic indicators
- Seasonal patterns are not explicitly modeled
- Moderate forecast error limits reliability for high-stakes decisions

## Tools & Technologies
- Python
- Pandas, NumPy
- Statsmodels
- Matplotlib

## Future Improvements
- Compare with baseline models (Naïve, Moving Average, SARIMA)
- Incorporate seasonality and external variables
- Improve model selection and hyperparameter tuning
- Explore machine learning approaches for forecasting
