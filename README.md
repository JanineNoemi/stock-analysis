# Automated Stock & Financial Risk Analyzer

A Python-based financial data analysis and visualization tool for historical stock data. The script fetches market data, performs data cleaning, calculates quantitative financial risk metrics and trend indicators, and automatically exports structured reports and charts.

---

## Features

- **Automated Data Retrieval:** Dynamically fetches historical price data via the `yfinance` API.
- **Data Cleaning & Normalization:** Removes missing values, handles timezone conflicts, and prepares time series data.
- **Financial & Quantitative Metrics:**
  - Daily percentage returns & gain/loss in USD
  - Simple Moving Averages (SMA 50 & SMA 200) for trend identification
  - Automated signal detection for **Golden Cross** (buy signal) and **Death Cross** (sell signal)
  - Rolling 21-day annualized volatility
  - **Maximum Drawdown** (maximum historical loss from peak)
- **Visualization & Report Export:**
  - Automatically generates 6 high-resolution charts (PNG)
  - Exports cleaned data and calculated metrics to a CSV file

---

## Tech Stack & Libraries

- **Language:** Python 3.x
- **Data Processing:** `pandas`, `numpy`
- **Financial Data:** `yfinance`
- **Data Visualization:** `matplotlib`, `seaborn`[cite: 4]

---

## Installation & Setup

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/YOUR-USERNAME/your-repo-name.git](https://github.com/YOUR-USERNAME/your-repo-name.git)
   cd your-repo-name
