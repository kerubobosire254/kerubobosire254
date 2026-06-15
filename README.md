# Hi, I'm Kerubo 👋

**Actuarial Scientist → Machine Learning Engineer + AI Engineer**

I build end-to-end ML systems across healthcare AI, financial intelligence, NLP, and behavioural analytics — from raw data to deployed, production-ready applications. My actuarial science background shapes how I think about risk, uncertainty, and model accountability. My projects reflect that rigour.

Currently: Pension Administrator at **Enwealth Financial Services** · Python & Data Science Trainer at **Tech Savvy Institute** · Actively seeking ML Engineer / Data Scientist/ AI Engineer roles.

## 🚀 Featured Projects

### 🎗️ BreastCare Kenya — Clinical Decision Support Platform
> *Python · Streamlit · Plotly · Rule-based NLP · Offline-first · Build54 Hackathon*

A 7-module, fully connected clinical decision support platform for breast cancer screening — built for Kenya's healthcare system where 54% of practitioners have poor knowledge scores and 78% of patients present at Stage III or IV.

**What makes it different:**
- Every module feeds the next — one patient, one journey, zero re-entering data
- CareBot: a rule-based NLP clinical assistant covering 11 topics — **zero API keys, works fully offline**
- Risk Assessment outputs a weighted score on a colour-coded gauge, auto-adds patient to Follow-Up Tracker, and generates a downloadable clinical handover summary
- Referral Intelligence Engine uses evidence-weighted scoring aligned to the Kenya MOH referral pathway
- Analytics Dashboard pulls live from session data across 4 tabs including a KAP Insights tab
- Grounded in a KAP survey of 250 Kenyan health practitioners, calibrated against published East African literature (2013–2024)
- Built for low-connectivity environments: core functions run without internet

🔗 [Live App](https://breastcarekenya.streamlit.app/) · [Live Dashboard](https://breastcaredashboard.streamlit.app/) · [Repo](https://github.com/kerubobosire254/breastcancer_help_app)

---

### 💳 SME Credit Risk Intelligence Platform
> *XGBoost · KMeans · Explainable AI · Scikit-learn · Streamlit · Pandas*

An AI-driven underwriting and risk analytics system that transforms raw SME financial data into actionable credit intelligence — built for emerging market lending environments where incomplete records and informal business structures are the norm.

**What it does:**
- Predicts Probability of Default (PD) using an XGBoost pipeline
- Engineers financial risk features: debt-to-income, cash flow stability, liquidity pressure, profit margin, revenue growth
- Segments SMEs into behavioural personas (Stable, Growth, Seasonal, Distressed) via KMeans clustering
- Benchmarks SME performance against industry-level reference metrics
- Provides explainable risk driver breakdowns for auditable lending decisions
- Generates downloadable credit risk reports

🔗 [Live Demo](https://sme-credit-risk-scoring-app-xadzpa4xvatoo2hk5zm5jj.streamlit.app/) · [Repo](https://github.com/kerubobosire254/sme-credit-risk-scoring-app)

---

### 🧠 SentimentIQ — NLP Review Classifier
> *Scikit-learn · TF-IDF · Logistic Regression · SVM · Naive Bayes · SMOTE · Streamlit*

A production-deployed NLP classifier for Amazon product review sentiment, built with deliberate model selection, class imbalance handling, and honest documentation of where traditional ML fails.

**What it does:**
- End-to-end NLP pipeline: text cleaning → TF-IDF vectorisation → model benchmarking → deployment
- Compares Naive Bayes, Logistic Regression, and Linear SVM using GridSearchCV + 5-fold CV, F1-score optimised
- Handles class imbalance via oversampling
- Documents model limitations explicitly: sarcasm, mixed sentiment, domain shift — intellectual honesty that matters in production

🔗 [Live Demo](https://sentiment-analysisapp-qqzxw6exrhfvsby5ygndf2.streamlit.app/) · [Repo](https://github.com/kerubobosire254/sentiment-analysis_app)

---

### 🎧 SpotifyDNA — Listening Personality Engine
> *Python · Pandas · Streamlit · Plotly · JSON Streaming Data · Behavioural Analytics*

A behavioural analytics app that transforms raw Spotify streaming history into an interpretable listening identity — not just what you listened to, but what kind of listener you are.

**What it does:**
- Ingests real Spotify streaming history JSON (or CSV)
- Engineers behavioural signals: skip rate, listening duration, artist diversity, time-of-day patterns
- Classifies listening traits: Explorer vs Loyalist, Deep vs Picky, Morning / Day / Night
- Maps traits to personality archetypes (e.g. Night Owl Explorer)
- Interactive Plotly dashboard with KPI metrics

🔗 [Live Demo](https://the-spotify-data-analysis-m6w3vxjncfcxyx8yaitjkb.streamlit.app/) · [Repo](https://github.com/kerubobosire254/The-spotify-data-analysis)

---

### 📈 Stock Price Intelligence Terminal
> *TensorFlow · Keras · LSTM · Monte Carlo (GBM) · Plotly · Streamlit · yfinance*

A multi-method stock forecasting platform that layers three complementary approaches so each compensates for what the others can't do alone — because a single price line with no uncertainty range is not how professionals reason about the future.

**What's built:**
- **LSTM** trained on 5 engineered features with a 60-day lookback, evaluated on RMSE / MAE / MAPE / directional accuracy
- **Monte Carlo simulation** — up to 2,000 GBM paths, configurable 10–90 day horizon, with 50th/95th/5th percentile bands and probability-of-upside reporting
- **Technical indicators** computed from scratch (no TA-Lib dependency): Bollinger Bands, RSI, MACD, ATR, %B
- Clean separation of `train_and_save.py` (training pipeline) and `app.py` (inference layer) — the same pattern used in production ML serving
- Ships with a synthetic 6-year demo dataset (1,500+ trading days) with realistic market regimes

🔗 [Repo](https://github.com/kerubobosire254/stock_app-101)

---

## 🧰 Tech Stack

| Area | Tools |
|------|-------|
| **Languages** | Python, SQL |
| **ML & Modelling** | Scikit-learn, XGBoost, TensorFlow, Keras, LSTM |
| **NLP** | TF-IDF, Logistic Regression, SVM, Naive Bayes, Rule-based NLP, Prompt Engineering |
| **Data** | Pandas, NumPy, Feature Engineering, yfinance |
| **Visualisation** | Plotly, Matplotlib, Seaborn |
| **Deployment** | Streamlit, Streamlit Cloud |
| **Other** | Explainable AI, KMeans Clustering, Monte Carlo Simulation, Time Series Forecasting, Offline-first Architecture |

---

## 📌 Currently Building Toward

- MLOps: MLflow experiment tracking, model versioning
- REST API deployment with FastAPI
- Cloud deployment: Azure / Databricks
- Docker & CI/CD pipelines

---

## 🤝 Let's Connect

Open to **Machine Learning Engineer** and **Data Scientist** roles — particularly in fintech, healthtech, or mission-driven organisations operating in emerging markets.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Kerubo%20Bosire-0077B5?style=flat&logo=linkedin)](https://linkedin.com/in/kerubo-bosire-364523283)
[![GitHub](https://img.shields.io/badge/GitHub-kerubobosire254-181717?style=flat&logo=github)](https://github.com/kerubobosire254)
📧 kerubobosire254@gmail.com
