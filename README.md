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
- **Data Visualization:** `matplotlib`, `seaborn`

---

## Installation & Setup

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/YOUR-USERNAME/your-repo-name.git](https://github.com/YOUR-USERNAME/your-repo-name.git)
   cd your-repo-name
2. **Install required dependencies:**
   ```bash
   pip install yfinance pandas numpy matplotlib seaborn

## Usage

Run the script from your terminal or execute the Jupyter Notebook:
   ```bash
   python main.py
   ```

When prompted, enter the required parameters:

1. **Ticker Symbol:** e.g., `TSLA`, `AAPL`, `MSFT`
   
2. **Start Date:** Format `YYYY-MM-DD` (e.g., `2021-01-01`)

---

## Generated Output & Visualizations

After execution, the tool automatically saves the following files to your project directory:

| Filename / Type | Description |
| --- | --- |
| `[TICKER]_01_kursverlauf.png` | Historical closing price chart

 |
| `[TICKER]_02_taegliche_renditen.png` | Daily percentage return dynamics

 |
| `[TICKER]_03_renditen_histogramm.png` | Statistical distribution of daily returns

 |
| `[TICKER]_kurs_trends.png` | Closing price with SMA 50, SMA 200 & Golden/Death Crosses

 |
| `[TICKER]_risikoanalyse.png` | Rolling 21-day annualized volatility chart

 |
| `[TICKER]_04_drawdowns.png` | Underwater chart highlighting Maximum Drawdown

 |
| `[TICKER]_analysiert_[DATE].csv` | Complete dataset exported to CSV

 |

---

## Academic Context

This project was developed as part of a university module. It demonstrates practical applications of data wrangling, quantitative risk analysis, and automated data visualization in Python.

```

```
