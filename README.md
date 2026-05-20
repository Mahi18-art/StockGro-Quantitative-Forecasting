# StockGro-Quantitative-Forecasting
# Quantitative Forecasting & Multi-Factor Portfolio Optimization

This repository contains the complete end-to-end framework for asset evaluation, forecasting, and deployment validation on StockGro with a capital footprint of ₹10,00,000.

##  Technical Architecture Overview
The underlying pipeline executes data harvesting dynamically via `yfinance`, performs structural signal separation using Robust STL decomposition, and optimizes capital risk matching via an automated inverse-variance weighting schema.

##  Submission Deliverables Mapping
The final analysis is structurally organized across the 8 core evaluation pillars as presented in the comprehensive project report:

* **Task 1: Stock Selection Rationale** — Strategic baseline asset universe targeting high-liquidity choices.
* **Task 2: Data Preprocessing Steps** — Stationarity transformations, outlier filtering, and feature normalization.
* **Task 3: Production Forecast Funnel** — Out-of-sample forward targets wrapped in 95% confidence intervals.
* **Task 4: Volatility & Trend Analysis Findings** — Structural trend stability tracking and EWMA risk matrices.
* **Task 5: Portfolio Composition & Sizing** — Multi-strategy execution rules scaling return targets against risk limits.
* **Task 6: Model Evaluation Metrics** — Cross-validation analysis and historical backtest performance parsing.
* **Task 7: StockGro Execution Summary** — Live position deployments, order fills, and asset deployment summaries.
* **Task 8: Predicted vs. Actual Outcomes** — The core performance validation matching model projections to actual spot rates.
* **Task 9: Operational Reflections** — Algorithmic adjustments, constraint modifications, and future execution enhancements.

## How to Execute the Pipeline Local Environment Setup
1. Clone this repository to your local machine.
2. Install the system dependencies directly using the frozen manifest:
   ```bash
   pip install -r requirements.txt
3. Launch your Jupyter interface and execute the tracking workflow sequentially
