# PROPHET-IIT_GUWAHATI-Stock-Predictor

# 📈 Consulting & Analytics Club - IIT Guwahati Prophet Contest on StockGro

Welcome to my solution for the **IIT Guwahati Prophet Contest on StockGro**!  
This project focuses on developing a **data-driven approach** for short-term **stock price prediction** and **portfolio allocation**. Utilizing advanced time series forecasting models, the aim is to simulate real-world trading with a virtual ₹10,00,000 budget using live **NSE/BSE data**.

---

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; ![Image Alt](https://github.com/Adityabaan/PROPHET-IIT_GUWAHATI-Stock-Predictor/blob/dc4f4980a29b7527e93876a38994961011e45699/profile.png) &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; ![Image Alt](https://github.com/Adityabaan/PROPHET-IIT_GUWAHATI-Stock-Predictor/blob/dc4f4980a29b7527e93876a38994961011e45699/images.png)

&nbsp; &nbsp; &nbsp; ![Image Alt](https://github.com/Adityabaan/PROPHET-IIT_GUWAHATI-Stock-Predictor/blob/ab7a9c184562f6e6ce5e2c8c719530e6ceb94aac/stockgrow.PR_.jpg)

## 📝 Overview

This repository contains:
- 🗂 **Solutions**: Time series forecasting for stock price prediction.
- 💹 **Portfolio Allocation Strategies**: Optimal capital deployment.
- 📊 **Risk Management**: Focused on volatility analysis and trend interpretation.

### 🌟 Objectives:
1. Predict stock prices for the next **2 trading days** (May 12–13, 2025).  
2. Optimize **stock selection** and **capital allocation**.  
3. Report **performance and strategy outcomes** within a virtual trading environment.

---

## 📜 Problem Statement

Participants are required to:
1. **Predict stock prices** for a selected set of NSE-listed stocks using **time series forecasting models** (e.g., ARIMA, Prophet, LSTM).  
2. Utilize predictions for **stock selection** and **capital allocation** in **StockGro's trading environment**.  
3. Manage risk and optimize returns during the **2-day trading window**.  

---

## 📂 Data

- **Source**: Live NSE/BSE data via StockGro and Python libraries like `yfinance`.  
- **Period**: January 1, 2020 – December 31, 2024.  
- **Validation**: Reserved the last 6 months for testing and validation.  
- **Features**: Open, close, high, low, volume, and derived indicators.

---

## 🚀 Project Workflow

### 1. **Stock Universe Selection**  
- Selected **5–10 NSE-listed stocks** based on:  
  - Historical volatility (using rolling standard deviation).  
  - Trend strength (via seasonal decomposition).  
  - Sectoral diversity for risk mitigation.  
- Documented rationale for each stock choice.

---

### 2. **Data Preprocessing**  
- 📥 Handled missing values (forward/backward fill).  
- 📈 Checked and enforced stationarity (ADF test, differencing).  
- 🔄 Scaled data for ML models (e.g., `MinMaxScaler` for LSTM).  
- 🧪 Performed train-test split (last 6 months for validation).

---

### 3. **Time Series Forecasting**  
Implemented and compared the following models:  
- **ARIMA/SARIMA** (tuned via AIC/BIC).  
- **Facebook Prophet**.  
- **LSTM/GRU**.  
- **Transformer-based models**.  

📅 **Forecast Horizon**: 2 trading days.  
📊 **Evaluation Metrics**:  
- MAPE (Mean Absolute Percentage Error).  
- RMSE (Root Mean Squared Error).  
- Hit rate (directional accuracy).  

---

### 4. **Volatility & Trend Analysis**  
- Estimated short-term volatility (log returns, GARCH/ARCH models).  
- Decomposed price series (trend, seasonality, noise).  
- Interpreted trends and volatility to guide capital allocation.  

---

### 5. **Stock Selection & Allocation Strategies**  
- **Forecast-Guided Allocation**:  
  Allocated more capital to stocks with higher predicted gains and model confidence.  
- **Volatility-Aware Sizing**:  
  Reduced exposure to stocks with high expected volatility to manage risk.  
- **Diversification**:  
  Ensured sectoral diversity and analyzed correlation to minimize portfolio risk.

---

## 🛠️ Prerequisites

Before running the project, ensure you have the following installed:
- Python 3.8+  
- Jupyter Notebook or Jupyter Lab  
- Libraries: `numpy`, `pandas`, `matplotlib`, `statsmodels`, `yfinance`, `fbprophet`, `tensorflow`, `arch`  

---

## 🧑‍💻 Contributor

- **Adityabaan Tripathy**: [GitHub Profile](https://github.com/Adityabaan)  
Feel free to connect for queries, suggestions, or collaborations!

---

## 📬 Contact

For any questions or feedback:  
📧 Email: [adityabaantripathy@gmail.com](mailto:adityabaantripathy@gmail.com)  
🌐 LinkedIn: [Adityabaan Tripathy](https://www.linkedin.com/in/adityabaan-tripathy-6b245323b/)  

---

## 🔗 Resources

- 📄 Blog on ARIMA & SARIMA  
- 📄 Facebook Prophet Documentation  
- 📄 LSTM/GRU Time Series Tutorials  

---

## 🌟 Acknowledgments

Special thanks to **IIT Guwahati** and **StockGro** for organizing this exciting contest.  
Happy forecasting! 🚀

