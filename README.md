# Hi, I'm Kerubo 👋

**Actuarial Scientist → Machine Learning Engineer + AI Engineer**

I'm a self-taught ML Engineer who builds AI systems for problems that actually matter.

My background is Actuarial Science, which means I think in probabilities, risk, and real-world uncertainty before I ever touch a model. That foundation shapes everything I build.
  
I work across the full ML stack: feature engineering, model development, explainability, deployment. And I'm equally comfortable in the math as I am in the code. XGBoost, LSTM networks, Poisson regression, SHAP, TF-IDF, dynamic feedback systems, Streamlit, not as buzzwords, but as tools I've broken, debugged, and rebuilt until they worked the way I needed them to.

By day I work in pensions and financial services, which means I understand what it costs when systems get things wrong.
  
I also teach Python and Data Science at the Tech Savvy Institute. Teaching does something to you. You find out very quickly what you actually understand versus what you just think you do. A room full of curious people has no patience for vague answers. I love it.
  
I have a thing for systems that are honest, models that show their reasoning, solutions that fit real constraints, tools built for people who don't have the luxury of perfect infrastructure.
  
If you're building something with stakes — in health, fintech, or humanitarian tech — and you need someone who gets unreasonably invested in making it work properly:

I'm your person

## 🩺 BreastCare Kenya
**[breastcancer_help_app](https://github.com/kerubobosire254/breastcancer_help_app)**

Breast cancer is one of the leading causes of cancer deaths among Kenyan women yet most healthcare workers have no clinical decision support tool at their fingertips. Screening decisions are made from memory, in under-resourced settings, often without internet access.

BreastCare Kenya is a clinical decision support platform built specifically for Kenyan healthcare workers. It uses a KAP survey of 250 practitioners as its foundation, flags high-risk patients based on clinical inputs, generates automatic referral letters and handover summaries, and includes an offline-capable NLP chatbot covering 11 clinical topics — no paid API, no internet required. Built as a hackathon entry for Build54.

It is a 7-module platform: risk assessment → screening checklist → referral intelligence → follow-up tracking → analytics dashboard → clinical CareBot. Every module feeds the next automatically. One patient. One journey. Zero re-entry.

`Streamlit` `NLP` `Clinical Decision Support` `Offline-First` `Kenya`

---

## 💳 SME Credit Risk Intelligence Platform
**[sme-credit-risk-scoring-app](https://github.com/kerubobosire254/sme-credit-risk-scoring-app)**

Small businesses in Africa are starved of credit not because they're bad borrowers, but because lenders have no reliable, fast way to assess their risk. Traditional credit scoring models weren't built for SMEs with thin or informal financial histories.

This platform uses XGBoost and KMeans clustering to score SME creditworthiness and segment borrowers by risk profile. It includes batch scoring for multiple applicants at once, SHAP-based model explainability so you can see *why* a decision was made, and a full interactive dashboard. Built with actuarial rigour — no random noise injected into predictions, deterministic and auditable by design.

`XGBoost` `KMeans` `SHAP` `Streamlit` `Credit Scoring` `Batch Processing`

---

### ⚽ World Cup 2026 Match Predictor
Python | XGBoost | Poisson Regression | Streamlit
↗ Live Demo: https://2026-worldcuppredictions-msqvpuk2xsy4w8zsuo7taz.streamlit.app/
– Every four years, millions of people predict World Cup results with complete confidence. Every four years, Argentina loses to Saudi Arabia and ruins everything. Most prediction tools either pretend upsets don't happen, or hide behind "football is unpredictable" as an excuse not to try.
– Built a match predictor for all 48 WC 2026 teams that gives you real probabilities: who's likely to win, by how much, and with what scoreline. Drop in any two teams, pick the stage, and you get win/draw/loss odds, expected goals for each side, and a full scoreline table ranked from most to least likely.
– The model learned from 964 World Cup matches going back to 1930. The trickiest part was stopping it from just predicting "home win" every single time, which is technically 57% accurate but completely useless. Fixed it by letting the model learn normally, then adjusting the output probabilities to match how often each outcome actually happens in practice.
– The part I enjoyed most: a live feedback loop. Enter real results as the tournament plays out and the app immediately recalculates every team's form and rating, so the next prediction uses what teams actually did on the pitch, not what we assumed before kickoff.

---

### 🔍 ATS Resume Analyzer
Python | Flask | spaCy | TF-IDF | Scikit-learn
↗ Live Demo: https://2026-worldcuppredictions-msqvpuk2xsy4w8zsuo7taz.streamlit.app/
– A lot of great candidates never hear back after applying , not because they're unqualified, but because their resume uses slightly different words than the job description, and the automated system never makes the connection. This tool helps bridge that gap.
– Upload your resume, paste the job description, and the app tells you how well they match: a compatibility score, the keywords you share, the ones you're missing, and what you can do about it. It turns resume optimization from guesswork into something you can actually act on.
– The hardest design decision was honesty. A high match score doesn't automatically mean you're the right person for the job. A low one doesn't mean you aren't. The app is upfront about this, the score is a guide, not a verdict.
– Built with the real limitations of keyword-based systems in mind: they struggle with synonyms, can't weigh soft skills, and trip over the fact that two companies describing the same role will use completely different language. Documenting what the tool can't do turned out to be just as important as building what it can.

---
## 🎵 SpotifyDNA — Listening Analytics
**[The-spotify-data-analysis](https://github.com/kerubobosire254/The-spotify-data-analysis)**

Your Spotify history is a goldmine of data about who you are but the platform only shows you what you listened to, not what it says about you.

SpotifyDNA analyses listening patterns to infer personality archetypes, mood trends, and audio fingerprints across genres and time periods. It goes beyond play counts to surface what your music taste actually reveals  energy levels, danceability curves, and listening identity. Upload your own Spotify export and see yourself in the data.

`Spotify API` `Pandas` `Plotly` `Personality Archetypes` `Mood Inference` `Streamlit`

---

### 🔍  SentimentIQ — NLP Sentiment Intelligence Engine
 Python   |   TF-IDF   |   Scikit-learn   |   Plotly   |   Streamlit 
↗ Live Demo: https://sentiment-analysisapp-qqzxw6exrhfvsby5ygndf2.streamlit.app/
–	Every organisation collects customer feedback. Almost none of them can actually read it not at scale. Thousands of reviews sit unanalyzed because the volume is unmanageable by hand.
–	Benchmarked Naive Bayes, Logistic Regression, and Linear SVM head-to-head using GridSearchCV with 5-fold cross-validation on a three-class sentiment task; selected Logistic Regression for accuracy, stability on sparse TF-IDF features, and native interpretability.
–	Addressed real-world class imbalance with random oversampling; explicitly flagged the overfitting risk that technique introduces rather than glossing over it.
–	Built word-level explainability into every prediction surfacing terms driving the verdict and their relative weight alongside a confidence score. Extended to bulk CSV batch processing and a session analytics tab for lightweight sentiment monitoring.

---

## 📈 Stock Price Intelligence Terminal
**[stock_app-101](https://github.com/kerubobosire254/stock_app-101)**

Professional-grade stock analysis tools cost thousands of dollars a year and are built for trading desks, not everyday investors. The data exists —the access doesn't.

This terminal brings Bloomberg-style analysis to anyone with a browser. It runs LSTM deep learning predictions on Netflix stock price history, overlays technical indicators (RSI, MACD, Bollinger Bands), and simulates 600 possible price futures using Monte Carlo modelling — all in one clean dashboard with a built-in demo mode so it never loads blank. No CSV required to get started.

`LSTM` `Monte Carlo` `Technical Analysis` `Streamlit` `Time Series` `Deep Learning`

# 🧰 Tech Stack

| Area | Tools |
|------|-------|
| **Languages** | Python, SQL, R |
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

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Kerubo%20Bosire-0077B5?style=flat&logo=linkedin)](https://linkedin.com/in/kerubo-bosire-364523283)
[![GitHub](https://img.shields.io/badge/GitHub-kerubobosire254-181717?style=flat&logo=github)](https://github.com/kerubobosire254)
📧 kerubobosire254@gmail.com
