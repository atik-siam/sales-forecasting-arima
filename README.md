# Sales Forecasting Using ARIMA

## Overview
This project focuses on forecasting monthly retail sales using time series modeling.
The goal is to build an interpretable model that can support short-term business planning.

## Dataset
- Supermarket sales data
- Aggregated into monthly time series

## Methodology
- Time series aggregation and visualization
- Log transformation for variance stabilization
- Stationarity testing using Augmented Dickey-Fuller (ADF)
- ARIMA(1,1,0) model implementation
- Residual diagnostics (ACF, Ljung-Box)
- Forecasting on original scale

## Results
- Forecast horizon: 6 months
- MAPE: ~36%
- sMAPE: ~47%

## Business Insight
The model captures the overall sales trend and provides a reasonable estimate
for short-term demand. It can support planning decisions such as inventory
management and sales forecasting.

## Limitations
- Limited historical data reduces long-term accuracy
- External factors (promotions, seasonality, economic changes) are not included
- Forecast uncertainty increases over time

## Tools
Python, Pandas, NumPy, Statsmodels, Matplotlib
