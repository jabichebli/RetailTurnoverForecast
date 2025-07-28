# RetailTurnoverForecast
Created by Jason Abi Chebli
© 2025 Jason Abi Chebli. All rights reserved.

## Description
This project forecasts monthly turnover (in $Million AUD) for the Northern Territory's electrical and electronic goods retailing industry (Series ID: A3349598V) using classical time series techniques—ETS and ARIMA. The project is based on data from the Australian Bureau of Statistics (ABS) spanning April 1998 to December 2022 and aims to produce accurate and interpretable forecasts supported by statistical diagnostics and validation using updated real-world data.

## Dataset
- Source: Australian Bureau of Statistics (ABS)
- Time Period: April 1998 – December 2022
- Region: Northern Territory, Australia
- Industry: Electrical and electronic goods retailing
- Series ID: A3349598V
- Unit: $Million AUD
- Access Method: Programmatically retrieved using fpp3 R package

## Objectives
- Explore statistical features of the retail turnover series
- Apply appropriate transformations and decomposition
- Identify and fit ETS and ARIMA models
- Perform model selection using AIC and test-set validation
- Diagnose residuals and validate assumptions
- Generate 2-year forecasts and compare with actual ABS updates
- Evaluate model accuracy and discuss their suitability

## Key Methods
- Transformation: Box-Cox (λ estimated via Guerrero method)
- Decomposition: STL for trend, seasonality, and residuals
- Stationarity Testing: Unit-root tests and differencing
- Model Selection: AIC-based shortlisting and test set validation (last 24 months)

## Model Fitting:
- ETS (Exponential Smoothing State Space Models)
- ARIMA (AutoRegressive Integrated Moving Average)
- Validation: ACF plots, Ljung-Box test, and comparison to up-to-date ABS data
- Forecasting: Out-of-sample predictions with 80% prediction intervals through to December 2024

## Files
- RetailTurnoverForecast.qmd — Quarto file containing full analysis, diagnostics, and forecasts
- RetailTurnoverForecast.html — Rendered output for easy viewing
- abs_forecast_comparison.csv — Actual ABS data from Table 11 used for validating forecast accuracy

## Visual Highlights
- Seasonally adjusted line plots highlighting COVID-19 impacts
- STL decomposition to isolate components
- AIC-ranked model comparison
- Residual ACF plots and Ljung-Box test outputs
- Forecast visualisations with 80% prediction intervals
- Forecast accuracy comparison against latest ABS values

## Feedback
If you have questions, suggestions, or feedback on this analysis, feel free to contact me. Your input is welcome and appreciated.

