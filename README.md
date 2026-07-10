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

–	Built a 7-module clinical decision support app addressing a documented gap in Kenyan breast cancer care: published KAP research shows practitioners know the screening guidelines (54.7%) but don't consistently act on them in practice (29.2%, as low as 12.7% among community health workers) - a major reason patients aren't caught until Stage III or IV.
–	Designed an end-to-end workflow where each patient encounter automatically drives the next stage of care, symptoms flow into the screening checklist, red flags trigger referral recommendations, referrals generate follow-up records, and the encounter produces a clinical handover summary with zero duplicate data entry across the journey.
–	Engineered the platform to run fully offline, building a weighted risk-scoring engine, an evidence-based referral recommendation system, and CareBot (a rule-based NLP clinical assistant covering 11 breast cancer topics) so practitioners get instant guidance with no internet access, API keys, or subscriptions required.

`Streamlit` `NLP` `Plotly` 

---

## 💳 SME Credit Risk Intelligence Platform
**[sme-credit-risk-scoring-app](https://github.com/kerubobosire254/sme-credit-risk-scoring-app)**

Small businesses in Africa are starved of credit not because they're bad borrowers, but because lenders have no reliable, fast way to assess their risk. Traditional credit scoring models weren't built for SMEs with thin or informal financial histories.

This platform uses XGBoost and KMeans clustering to score SME creditworthiness and segment borrowers by risk profile. It includes batch scoring for multiple applicants at once, SHAP-based model explainability so you can see *why* a decision was made, and a full interactive dashboard. Built with actuarial rigour — no random noise injected into predictions, deterministic and auditable by design.

`XGBoost` `KMeans` `SHAP` `Streamlit` `Credit Scoring` `Batch Processing`

---

🔎 TraceKE — Missing Persons Identification System
          Python | Streamlit | Facenet-PyTorch | ChromaDB | OpenCV (YuNet)
         ↗ Live Demo: https://traceke.streamlit.app/
–	170 women were killed in Kenya in 2024. Over 8,800 children were reported missing. Some were found weeks later, alive, sitting in a hospital or a police station, unidentified, while their families were still searching. Not always because no one was looking, but because there's often no easy way to connect a person found in one place to a report filed in another. TraceKE is an attempt to close that gap.
–	Designed the confidence score to be multi signal on purpose, not just face similarity. Facial embedding match carries 55% of the score, age estimation 25%, gender 20%. Location is shown as context only and never used to penalize a match, because a person found 400km from home may have been trafficked, not misidentified.
–	Made the harder call to never reject a low quality photo. For some families, one blurry image taken years ago is the only one they have. The system flags uncertainty instead of discarding data, and redistributes confidence weights when a signal is missing rather than punishing incomplete cases.
–	Documented the model's limitations as rigorously as its features. Facenet was trained predominantly on Western datasets and has not been independently benchmarked on East African faces under real world lighting and resolution conditions, which is the single biggest gap the next version needs to close.

### ⚽ World Cup 2026 Match Predictor
Python | XGBoost | Poisson Regression | Streamlit
↗ Live Demo: https://2026-worldcuppredictions-msqvpuk2xsy4w8zsuo7taz.streamlit.app/
– Every four years, millions of people predict World Cup results with complete confidence. Every four years, Argentina loses to Saudi Arabia and ruins everything. Most prediction tools either pretend upsets don't happen, or hide behind "football is unpredictable" as an excuse not to try.
– Built a match predictor for all 48 WC 2026 teams that gives you real probabilities: who's likely to win, by how much, and with what scoreline. Drop in any two teams, pick the stage, and you get win/draw/loss odds, expected goals for each side, and a full scoreline table ranked from most to least likely.
– The model learned from 964 World Cup matches going back to 1930. The trickiest part was stopping it from just predicting "home win" every single time, which is technically 57% accurate but completely useless. Fixed it by letting the model learn normally, then adjusting the output probabilities to match how often each outcome actually happens in practice.
– The part I enjoyed most: a live feedback loop. Enter real results as the tournament plays out and the app immediately recalculates every team's form and rating, so the next prediction uses what teams actually did on the pitch, not what we assumed before kickoff.

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
