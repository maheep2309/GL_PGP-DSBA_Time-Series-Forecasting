# GL_PGP-DSBA_Time-Series-Forecasting
This project forecasts monthly sales of Rose and Sparkling wines using time-series models. It analyzes historical trends, seasonality, and patterns, evaluates multiple forecasting methods, identifies the best models, and generates 12-month forecasts to help ABC Estate Wines improve sales planning and strategy.

# Project Summary
This project analyzes 15 years of monthly Rose and Sparkling wine sales (1980–1995) to uncover long-term trends, seasonal behavior, and demand patterns for ABC Estate Wines. It begins with extensive exploratory data analysis, revealing a strong annual seasonality in both wines, a declining long-term trend for Rosé, and stable yet sharply seasonal year-end demand for Sparkling wine. Missing values (only in Rosé) are treated using spline interpolation.

The time series is decomposed using additive and multiplicative methods to separate trend, seasonality, and residual components. A full suite of forecasting models is then built on both original and stationary data, including Linear Regression, Naïve and Simple Average models, Moving Average (2-point trailing), Single/Double/Triple Exponential Smoothing (manual & autofit), Auto-ARIMA, Manual ARIMA, Auto-SARIMA, and Manual SARIMA.

Model performances are compared using RMSE. For Rosé wine, Triple Exponential Smoothing with additive trend and seasonality achieves one of the best results but is closely matched by the 2-point trailing Moving Average model. For Sparkling wine, Triple Exponential Smoothing with no trend and multiplicative seasonality delivers the strongest performance.

The best models are rebuilt on the full dataset and used to forecast the next 12 months, producing stable, seasonally aligned forecasts. Key insights highlight declining Rosé popularity, strong and predictable holiday-driven Sparkling wine demand, and clear opportunities for inventory planning, promotional timing, and targeted marketing. These forecasts equip ABC Estate Wines with actionable, data-driven guidance to optimize future sales and maintain competitive advantage.
