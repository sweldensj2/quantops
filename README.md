# QuantOps: ML-Powered Risk Analytics Dashboard for Multi-Asset Portfolios

**Author:** Johan Sweldens  
**Target Audience:** Trading Ops Engineers, Quant Developers, Risk Analysts  
**Status:** MVP in progress (June 2025)

---

## 🧠 Overview

QuantOps is a personal finance-tech project designed to simulate, analyze, and visualize the performance and risk of multi-asset portfolios using real financial data and modern machine learning.

Inspired by roles within Financial Engineering, this project bridges market-aware analytics with software engineering best practices.

---

## 🎯 Features

- Simulate and visualize portfolio allocations
- Compute key risk metrics (VaR, volatility, drawdown, etc.)
- Detect anomalies using ML (PCA, clustering, isolation forest)
- Streamlit-powered dashboard for interactive exploration
- Dockerized for reproducibility

---

## 🧱 Stack

- **Python** (Pandas, NumPy, Scikit-learn, yfinance, Matplotlib)
- **ML Models** (PCA, Isolation Forest, Rolling Z-score)
- **Web UI**: Streamlit
- **Infra**: Docker, GitHub Actions (CI/CD ready)
- **Optional Extension**: C++ backend for pricing / curve fitting

---

## 🚀 Getting Started

```bash
git clone https://github.com/jsweldens/quantops.git
cd quantops
pip install -r requirements.txt
streamlit run dashboard/app.py

### 📅 **Sprint: June 18–25, 2025**

#### ✅ Setup & Infra
- [X] Create private or public GitHub repo: `quantops`
- [ ] Set up project structure with folders: `src`, `dashboard`, `notebooks`
- [ ] Add virtual environment and `requirements.txt` with:
  - `pandas`, `numpy`, `yfinance`, `scikit-learn`, `streamlit`, `matplotlib`

#### ✅ Data & Portfolio Logic
- [ ] Write `data_ingestion.py` to fetch daily stock prices (e.g., `AAPL`, `SPY`, `MSFT`)
- [ ] Implement `portfolio.py`:
  - basic portfolio constructor with weights
  - rolling returns, allocation over time
- [ ] Create static CSV of 3-5 tickers and weights to test with

#### ✅ Risk & ML Prototyping
- [ ] In `risk_metrics.py`, compute:
  - rolling volatility
  - rolling Sharpe ratio
  - max drawdown
- [ ] In `ml_models.py`, prototype Isolation Forest or rolling Z-score

#### ✅ UI & Dashboard
- [ ] Start `dashboard/app.py` in Streamlit:
  - sidebar for user input (ticker list, dates)
  - line chart of portfolio value
  - table of key metrics

#### ✅ Admin
- [ ] Write short `README.md`
- [ ] Add `.gitignore`, `LICENSE`, and initial commit
- [ ] Bonus: Write 1–2 unit tests in `tests/`
