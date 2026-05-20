# StockGro-Quantitative-Forecasting
# Multi-Factor Financial Forecasting & Risk-Aware Portfolio Optimization

An end-to-end quantitative trading and pipeline framework built to forecast equity price action and optimize asset allocation parameters using a virtual capital footprint of ₹10,00,000 deployed on StockGro.

## Project Architecture
The underlying pipeline runs entirely on live market data fetched dynamically via the `yfinance` API. The technical workflow is structured into three main engineering blocks:
1. **Signal Decomposition:** Isolating underlying trends and structural noise using Robust STL decomposition.
2. **Forecasting Funnel:** Generating out-of-sample forward projections wrapped in 95% confidence intervals utilizing a blended multi-model consensus (ARIMA, Prophet, LSTM).
3. **Portfolio Construction:** Allocating capital dynamically via custom inverse-variance weights and forecast-guided momentum scoring, validated using a 5,000-pass Monte Carlo Efficient Frontier simulation.

---

## 🗺️ Execution Framework Matrix
The core asset scaling strategy follows a structured 2x2 cross-reference matrix to manage portfolio risk parameters against varying market regimes:

                        TASK 4 METRIC CROSS-REFERENCE
                                      │
                 High Strength                  Low Strength
        ┌──────────────────────────────┬──────────────────────────────┐
        │ STRATEGY A: FORECAST GUIDED  │ HIGH NOISE REGIME            │
  High  │ - High conviction direction  │ - Avoid or heavily reduce    │
  Trend │ - Allocate larger weights    │   capital allocation         │
  Score │ - e.g., Britannia (Upward)   │ - Unpredictable price action │
        ├──────────────────────────────┼──────────────────────────────┤
        │ STRATEGY B: VOLATILITY AWARE │ DEEP CONSOLIDATION           │
  Low   │ - Feed directly into inverse │ - Sideways trend pattern     │
  Trend │   variance matrix (1/Var)    │ - Wait for explicit volume   │
  Score │ - Protect capital in Kotak   │   breakout confirmation      │
        └──────────────────────────────┴──────────────────────────────┘

---

## 📁 Repository Deliverables Directory
The structure of this project is organized strictly according to evaluation guidelines:

* 📂 **`notebooks/`**
  * `capstoneProject.ipynb`: The complete executable pipeline containing live data-harvesting, processing transformations, model implementations, and interactive Plotly optimization visualizations.
* 📂 **`reports/`**
  * `Projectreport_timeseriesanalysis.pdf`: The comprehensive 10-page analytical dossier diving into methodology justifications, historical performance backtests, StockGro fill executions, and final model calibration critiques.

---

## ⚙️ Local Environment & Installation
To reproduce the modeling environment and run the pipeline locally, execute the following steps in your local terminal:

1. Clone the repository:
   ```bash
   git clone [https://github.com/Mahi18-art/YOUR_REPOSITORY_NAME.git](https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git)
   cd YOUR_REPOSITORY_NAME
