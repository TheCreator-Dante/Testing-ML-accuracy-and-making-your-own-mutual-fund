# Mutual Fund Optimization and Forecasting

**Institute:** ISI Kolkata, IdeasTIH Department

---

## 🔍 Project Overview

This project builds an AI-powered system to forecast mutual fund performance using the past three years of Nifty 100 company data. Data is sourced in real time via the Yahoo Finance (`yfinance`) API, enabling continuous model updates and live forecasting.

---

## 🎯 Objective

* Deliver accurate, real-time forecasts of mutual fund performance.
* Leverage machine learning to inform and optimize investment strategies.

---

## 🚀 Approach

1. **Baseline Modeling with ARIMA**

   * Implemented ARIMA to establish initial time series benchmarks.

2. **Advanced Prediction with XGBoost**

   * Transitioned to XGBoost regression for superior forecasting.
   * XGBoost handles nonlinear relationships, captures complex feature interactions, and reduces overfitting with built‑in regularization.
   * Achieved **91% accuracy** on validation, outperforming classical models in speed and predictive power.

3. **Real-Time Data Automation**

   * Automated data pipeline using `yfinance` API to pull daily price and volume data for Nifty 100 companies over the last three years.
   * Ensures models are retrained with the latest market information for live forecasting.

4. **Prototype AI Agents (Future Work)**

   * Integrate large language model (LLM) agents for dynamic forecasting, natural language alerts, and decision support.
   * Explore NLP-driven sentiment analysis to enrich feature sets.

---

## 📊 Data Source

* **Universe:** Nifty 100 companies
* **Timeframe:** Last three years
* **Extraction:** Yahoo Finance API via Python `yfinance`

---

## 🔧 Prerequisites

* Python 3.8+
* Key packages: `pandas`, `numpy`, `statsmodels`, `xgboost`, `scikit-learn`, `yfinance`, `requests`

---

## 🛠️ Installation & Setup

```bash
git clone https://github.com/TheCreator-Dante/mutual-fund-forecasting.git
cd mutual-fund-forecasting
python3 -m venv venv
source venv/bin/activate   # On Windows: venv\\Scripts\\activate
pip install -r requirements.txt
cp .env.example .env       # Configure API keys and endpoints
```

---

## ⚙️ Usage

* **Run Baseline (ARIMA):**
  `python src/arima_forecast.py --config config/arima.yaml`

* **Run XGBoost Forecast:**
  `python src/xgboost_forecast.py --config config/xgb.yaml`

* **Launch Real-Time Pipeline:**
  `python src/realtime_agent.py`

---

## 📈 Impact

* Simplifies stock forecasting and investing with high-accuracy, real-time mutual fund predictions.
* Highlights the advantages of XGBoost—speed, robustness, and superior handling of complex financial datasets—over traditional time series models.

---

## 📝 Future Work

* Incorporate sentiment analysis from news and social media.
* Extend forecasting to other asset classes (bonds, ETFs).
* Develop an interactive dashboard for visualization and user interaction.

---


## 📜 License

This project is licensed under the MIT License. See \[LICENSE] for details.

© 2025 ISI Kolkata, IdeasTIH Department.
