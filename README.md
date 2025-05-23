# PROPHET-IIT_GUWAHATI-Stock-Predictor

**Overview:**
This repository contains my solution for the IIT Guwahati Prophet Contest on StockGro, focused on developing a data-driven approach for short-term stock price prediction and portfolio allocation. The project leverages time series forecasting models to guide stock selection and capital deployment within a virtual ₹10,00,000 budget, simulating real-world trading using live NSE/BSE data.

**Problem Statement:**
Participants are tasked with using time series analysis and forecasting models (e.g., ARIMA, Prophet, LSTM) to:
  *Predict stock prices for the next 2 trading days for a selected set of NSE-listed stocks.
  *Use these predictions to inform stock selection and capital allocation decisions within StockGro’s virtual trading environment.
  *Manage risk and optimize returns over a 2-day trading window (May 12–13, 2025), reporting performance and strategy outcomes1.

**Data:**
  *Source: Live NSE/BSE data via StockGro and Python libraries (e.g., yfinance).
  *Period: 1st January 2020 – 31st December 2024.
  *Testing: Minimum of the last 6 months’ data reserved for validation.
  *Features: Open, close, high, low, volume, and derived indicators.

**Project Workflow:**

1. Stock Universe Selection:
   *Selected 5–10 NSE-listed stocks based on:
      -Historical volatility (using rolling standard deviation)
      -Trend strength (via seasonal decomposition)
      -Sectoral diversity for risk mitigation1
   *Rationale for each stock choice is documented in the report.

2. Data Preprocessing:
   *Handled missing values (forward/backward fill).
   *Checked and enforced stationarity (ADF test, differencing).
   *Scaled data for ML models (e.g., MinMaxScaler for LSTM).
   *Performed train-test split (last 6 months for validation).

3. Time Series Forecasting:
   *Implemented and compared models:
     -ARIMA/SARIMA (tuned via AIC/BIC)
     -Facebook Prophet
     -LSTM/GRU
     -Transformer-based models
   *Forecasted prices for the next 2 trading days.
   *Evaluated using MAPE, RMSE, and hit rate (directional accuracy).

4. Volatility & Trend Analysis:
   *Estimated short-term volatility (log returns, GARCH/ARCH models).
   *Decomposed price series (trend, seasonality, noise).
   *Interpreted trends and volatility to inform allocation.

5. Stock Selection & Allocation Strategies:
   *Forecast-Guided Allocation: Allocated more capital to stocks with higher predicted gains and model confidence.
   *Volatility-Aware Sizing: Reduced exposure to stocks with high expected volatility to manage risk.
   *Diversification by sector and correlation analysis.
