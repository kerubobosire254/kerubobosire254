<div align="center">

<img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=24&duration=3000&pause=1000&color=14CC60&center=true&vCenter=true&width=650&lines=Actuarial+Scientist+%E2%86%92+ML+Engineer;I+build+AI+systems+for+problems+that+matter;Actuarial+brain%2C+data+science+hands." alt="Typing SVG" />

### Actuarial Scientist → Machine Learning Engineer + AI Engineer

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Kerubo%20Bosire-0077B5?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/kerubo-bosire-364523283)
[![Email](https://img.shields.io/badge/Email-kerubobosire254-D14836?style=flat&logo=gmail&logoColor=white)](mailto:kerubobosire254@gmail.com)
[![Open to Work](https://img.shields.io/badge/Open%20to-ML%20Engineer%20Roles-14CC60?style=flat)](https://linkedin.com/in/kerubo-bosire-364523283)

</div>

---

I'm a self-taught ML Engineer who builds AI systems for problems that actually matter.

My background is Actuarial Science, which means I think in probabilities, risk, and real-world uncertainty before I ever touch a model. That foundation shapes everything I build.

I work across the full ML stack: feature engineering, model development, explainability, deployment. XGBoost, LSTM networks, Poisson regression, SHAP, TF-IDF, vector search, dynamic feedback systems — not as buzzwords, but as tools I've broken, debugged, and rebuilt until they worked the way I needed them to.

By day I work in pensions and financial services, which means I understand what it costs when systems get things wrong. I also teach Python and Data Science at Tech Savvy Institute, teaching tells you very fast what you actually understand versus what you just think you do.

I have a thing for systems that are honest, models that show their reasoning, and tools built for people who don't have the luxury of perfect infrastructure.

**If you're building something with stakes — in health, fintech, or humanitarian tech — and you need someone who gets unreasonably invested in making it work properly: I'm your person.**

---

## 🔎 TraceKE — Missing Persons Identification System

**[TraceKE](https://github.com/kerubobosire254/TraceKE)** 

170 women were killed in Kenya in 2024. Over 8,800 children were reported missing. Some were found weeks later, alive, sitting in a hospital or a police station, unidentified not always because no one was looking, but because there's often no easy way to connect a person found in one place to a report filed in another. TraceKE is an attempt to close that gap.

- Designed the confidence score to be **multi-signal on purpose**, not just face similarity: facial embedding match carries 55% of the score, age estimation 25%, gender 20%. Location is shown as context only and never used to penalize a match, because a person found 400km from home may have been trafficked, not misidentified.
- Made the harder call to **never reject a low-quality photo**. For some families, one blurry image taken years ago is the only one they have — the system flags uncertainty instead of discarding data, and redistributes confidence weights when a signal is missing rather than punishing incomplete cases.
- Documented the model's limitations as rigorously as its features: Facenet was trained predominantly on Western datasets and hasn't been independently benchmarked on East African faces under real-world lighting and resolution conditions — the single biggest gap the next version needs to close.

`Python` `Streamlit` `Facenet-PyTorch` `ChromaDB` `OpenCV (YuNet)` `Face Recognition`

---

## 🩺 BreastCare Kenya

**[breastcancer_help_app](https://github.com/kerubobosire254/breastcancer_help_app)** 

Built a 7-module clinical decision support app addressing a documented gap in Kenyan breast cancer care: published KAP research shows practitioners know the screening guidelines (54.7%) but don't consistently act on them in practice (29.2%, as low as 12.7% among community health workers) — a major reason patients aren't caught until Stage III or IV.

- Designed an end-to-end workflow where each patient encounter automatically drives the next stage of care — symptoms flow into the screening checklist, red flags trigger referral recommendations, referrals generate follow-up records, and the encounter produces a clinical handover summary with zero duplicate data entry.
- Engineered the platform to run fully offline: a weighted risk-scoring engine, an evidence-based referral recommendation system, and CareBot (a rule-based NLP clinical assistant covering 11 breast cancer topics) so practitioners get instant guidance with no internet, API keys, or subscriptions required.

`Streamlit` `NLP` `Plotly`

---

## 💳 SME Credit Risk Intelligence Platform

**[sme-credit-risk-scoring-app](https://github.com/kerubobosire254/sme-credit-risk-scoring-app)**

Small businesses in Africa are starved of credit not because they're bad borrowers, but because lenders have no reliable, fast way to assess their risk. Traditional credit scoring models weren't built for SMEs with thin or informal financial histories.

- Uses XGBoost and KMeans clustering to score SME creditworthiness and segment borrowers by risk profile.
- Includes batch scoring for multiple applicants at once, SHAP-based model explainability so you can see *why* a decision was made, and a full interactive dashboard.
- Built with actuarial rigour no random noise injected into predictions, deterministic and auditable by design.

`XGBoost` `KMeans` `SHAP` `Streamlit` `Credit Scoring` `Batch Processing`

---

## ⚽ World Cup 2026 Match Predictor

**[World-Cup-2026-Predictor](https://github.com/kerubobosire254/World-Cup-2026-Predictor)** 

Every four years, millions of people predict World Cup results with complete confidence. Every four years, Argentina loses to Saudi Arabia and ruins everything.

- Built a match predictor for all 48 WC 2026 teams that gives real probabilities: who's likely to win, by how much, and with what scoreline.
- Trained on 964 World Cup matches going back to 1930. The trickiest part was stopping it from just predicting "home win" every time (technically 57% accurate but useless). Fixed by adjusting output probabilities to match real-world outcome frequencies.
- Built a live feedback loop: enter real results as the tournament plays out and the app recalculates every team's form and rating on the fly.

`Python` `XGBoost` `Poisson Regression` `ELO Ratings` `Streamlit`

---

## 🎵 SpotifyDNA — Listening Analytics

**[The-spotify-data-analysis](https://github.com/kerubobosire254/The-spotify-data-analysis)** 

Your Spotify history is a goldmine of data about who you are, but the platform only shows you what you listened to, not what it says about you.

- Analyses listening patterns to infer personality archetypes, mood trends, and audio fingerprints across genres and time periods.
- Surfaces energy levels, danceability curves, and listening identity, upload your own Spotify export and see yourself in the data.

`Spotify API` `Pandas` `Plotly` `Personality Archetypes` `Mood Inference` `Streamlit`

---

## 🔍 SentimentIQ — NLP Sentiment Intelligence Engine

**[sentiment-analysis_app](https://github.com/kerubobosire254/sentiment-analysis_app)** 

Every organisation collects customer feedback. Almost none of them can actually read it at scale.

- Benchmarked Naive Bayes, Logistic Regression, and Linear SVM head-to-head using GridSearchCV with 5-fold cross-validation; selected Logistic Regression for accuracy, stability on sparse TF-IDF features, and native interpretability.
- Addressed real-world class imbalance with random oversampling, explicitly flagging the overfitting risk rather than glossing over it.
- Built word-level explainability into every prediction, plus bulk CSV batch processing and a session analytics tab.

`Python` `TF-IDF` `Scikit-learn` `Plotly` `Streamlit`

---

## 📈 Stock Price Intelligence Terminal

**[Stock-Price-Prediction-API](https://github.com/kerubobosire254/Stock-Price-Prediction-API)** 

Professional-grade stock analysis tools cost thousands of dollars a year and are built for trading desks, not everyday investors.

- Runs LSTM deep learning predictions on stock price history, overlays technical indicators (RSI, MACD, Bollinger Bands), and simulates 600 possible price futures using Monte Carlo modelling.
- Built-in demo mode so it never loads blank, no CSV required to get started.

`LSTM` `Monte Carlo` `Technical Analysis` `Streamlit` `Time Series` `Deep Learning`

---

## 🧰 Tech Stack

**Languages**
![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/-SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)
![R](https://img.shields.io/badge/-R-276DC3?style=flat-square&logo=r&logoColor=white)

**ML & Modelling**
![Scikit-learn](https://img.shields.io/badge/-Scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![XGBoost](https://img.shields.io/badge/-XGBoost-2C7FB8?style=flat-square)
![TensorFlow](https://img.shields.io/badge/-TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![Keras](https://img.shields.io/badge/-Keras-D00000?style=flat-square&logo=keras&logoColor=white)

**NLP & Vector Search**
![TF-IDF](https://img.shields.io/badge/-TF--IDF-14CC60?style=flat-square)
![ChromaDB](https://img.shields.io/badge/-ChromaDB-6E56CF?style=flat-square)
![Facenet-PyTorch](https://img.shields.io/badge/-Facenet--PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)

**Data & Deployment**
![Pandas](https://img.shields.io/badge/-Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/-NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![Streamlit](https://img.shields.io/badge/-Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)
![Plotly](https://img.shields.io/badge/-Plotly-3F4F75?style=flat-square&logo=plotly&logoColor=white)

**Other**
![SHAP](https://img.shields.io/badge/-SHAP-000000?style=flat-square)
![OpenCV](https://img.shields.io/badge/-OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)
![Monte Carlo](https://img.shields.io/badge/-Monte%20Carlo-14CC60?style=flat-square)

---

## 📊 GitHub Stats

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=kerubobosire254&show_icons=true&theme=dark&hide_border=true&count_private=true" width="48%" />
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=kerubobosire254&layout=compact&theme=dark&hide_border=true" width="48%" />

</div>

---

## 📌 Currently Building Toward

- MLOps: MLflow experiment tracking, model versioning
- REST API deployment with FastAPI
- Cloud deployment: Azure / Databricks
- Docker & CI/CD pipelines

---

<div align="center">

### 🤝 Let's Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/kerubo-bosire-364523283)
[![Gmail](https://img.shields.io/badge/Email-Reach%20Out-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:kerubobosire254@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-Explore%20My%20Work-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/kerubobosire254)

*If you're reading this, you've already seen more of my work than most job descriptions ask for. Let's talk.*

</div>
