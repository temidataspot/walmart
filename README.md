# Walmart Stock Price Analysis & Forecasting (2020–2025)

**Tools Used:** Python, Power BI, XGBoost, statsmodels, pandas, matplotlib, seaborn

---

## Overview

This project presents an end-to-end analysis and forecasting of **Walmart’s stock price**, combining historical analysis, technical indicators, volatility modelling, machine learning, and portfolio simulation.

It includes an interactive **Power BI dashboard**, in-depth **time series analysis**, and **XGBoost forecasts** for daily and monthly price trends in **2025**.

🔗 **[Power BI Dashboard](https://app.powerbi.com/view?r=eyJrIjoiMmNlNjdkZjQtYTJkNC00MWVmLWEwNjktZGFlM2I4NWQ5MTk2IiwidCI6IjVhYjI0MzA0LWY3NWItNDlkZS04Y2RkLTAyZGMyOGNkNDU5YiJ9)**  
📁 **[Raw Dataset (CSV)](https://github.com/temidataspot/walmart/blob/main/WMT.csv)**
**[Jupyter Notebook (Python)](https://github.com/temidataspot/walmart/blob/main/walmart.ipynb)

---

## Part 1: Historical Data Analysis & EDA

- **Adjusted Close Price Over Time** — to visualise long-term stock trends
- **Daily Returns Analysis** — for volatility and outlier detection
- **Rolling Mean & Moving Averages** — smoothed price signals
- **30-Day Rolling Volatility** — volatility over time
- **Volatility vs. Price Comparison**
- **Monthly & Yearly Seasonality Checks**
- **Correlation Analysis** — between volume, price and returns
- **Bullish vs. Bearish Days** — open vs close price comparison
- **Time Series Decomposition** — trend, seasonality, residuals using `statsmodels`

---

## Part 2: Strategy Backtesting

Implemented and tested a **moving average crossover strategy**:

- **MA7 & MA30 Strategy**
- Compared to Buy-and-Hold
- Evaluated performance over time

---

## Part 3: Price Movement Classification (XGBoost)

Built an **XGBoost classifier** to predict the next day’s price movement (up/down):

**Features:**
- RSI (Relative Strength Index)
- MACD (Moving Average Convergence Divergence)
- Lag features
- Volume
- Calendar variables

---

## Part 4: Volatility Modelling

Modelled and visualised market volatility:

- **Standardised Residuals**
- **Conditional Volatility Plots**
- Identified high-risk and calm periods

---

## Part 5: Portfolio Simulation

Simulated portfolio based on **moving average signals**:

- Capital tracking
- Buy/sell logic from strategy
- Compared strategy vs Buy & Hold

---

## Part 6: 2025 Forecasting (XGBoost)

Used an **XGBoost Regressor** to forecast **daily stock prices throughout 2025**, then aggregated into **monthly predictions**.

**Features Used:**
- Lag features (lag_1 to lag_5)
- RSI, MACD, Bollinger Bands
- Calendar features (Day, Month, Weekday)

**Forecast Outputs:**
- 📅 Daily prediction chart for 2025
- 🗓️ Monthly average price forecast

---

## Future Work

- Use Prophet or LSTM for deep time series forecasting
- Include economic indicators (e.g., CPI, Unemployment)
- Add model backtesting with walk-forward validation
- Build web dashboard with Streamlit or Flask

---
