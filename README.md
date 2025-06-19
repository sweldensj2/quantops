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
