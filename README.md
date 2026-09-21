
<div align="center">

<img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=24&duration=3000&pause=1000&color=14CC60&center=true&vCenter=true&width=650&lines=Actuarial+Scientist+%E2%86%92+Machine+Learning+Engineer;I+build+AI+systems+for+problems+that+matter." alt="Typing SVG" />

### Actuarial Scientist → Machine Learning Engineer + AI Engineer

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Kerubo%20Bosire-0077B5?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/kerubo-bosire-364523283)
[![Email](https://img.shields.io/badge/Email-kerubobosire254-D14836?style=flat&logo=gmail&logoColor=white)](mailto:kerubobosire254@gmail.com)
[![Open to Work](https://img.shields.io/badge/Open%20to-ML%20Engineer%20Roles-14CC60?style=flat)](https://linkedin.com/in/kerubo-bosire-364523283)

</div>

---

I build things, break them, figure out why they broke, and then build them better.

My background is in Actuarial Science, so I naturally think in terms of risk, patterns, probabilities, and "okay, but what happens if this goes wrong?" Somewhere along the way, that question took me from analysing numbers to building software.

Over the past few months I've gone deep into engineering: Python, JavaScript, HTML, CSS, SQL, FastAPI, PostgreSQL, React, pytest, Docker and Git, not because I wanted a long list of technologies, but because I wanted to understand how things actually work end to end.

Python is where I'm strongest. I've built ML and data applications using XGBoost, Scikit-learn, TensorFlow, OpenCV and more, and I've fallen slightly too far down the engineering rabbit hole to discover I genuinely enjoy building the whole thing, API, database, and the frontend people actually have to look at.

I've built systems for postpartum healthcare follow-up, breast cancer screening, SME credit risk, missing-person identification, and sports prediction. Once I become interested in a problem, there's a good chance I'll disappear into it until I figure it out.

So yes, I'm probably going to keep building things. And yes, I'm probably going to break a few along the way.

---

## 🚩 Flagship Projects

### 🩺 MamaCare AI — Postpartum Risk Screening & Follow-Up Platform

**[Live Demo →](https://mamacare-frontend-v2.vercel.app/)** · **[GitHub →](https://github.com/kerubobosire254/mamacare_ai)**

<!-- Add a screenshot or GIF of the nurse dashboard here: ![MamaCare dashboard](./assets/mamacare-demo.png) -->

Mothers leave hospital with no follow-up, and manually calling every patient doesn't scale. I built a system that automates the check-in instead.

- Used CALL-E's voice AI to place scheduled calls at Day 3, Day 7, and Week 6, then built a risk engine that scores every answer as routine, urgent, or emergency with a clear reason attached, and a hard override that routes any disclosure of self-harm straight to a human
- Built the full stack behind that pipeline: FastAPI/PostgreSQL backend integrating CALL-E through a custom task prompt and structured webhook schema, tested end to end with pytest, and a React/Vite frontend giving nurses a dashboard to act on escalations
- Deployed live on Render, Neon, and Vercel

`FastAPI` `PostgreSQL` `REST & Webhooks` `CALL-E` `pytest` `React` `Vercel` `Render`

---

### 🔎 TraceKE — Missing Persons Identification System

**[GitHub →](https://github.com/kerubobosire254/TraceKE)**

<!-- Add a screenshot of the match-confidence UI here: ![TraceKE demo](./assets/traceke-demo.png) -->

170 women were killed in Kenya in 2024. Over 8,800 children were reported missing. Some were found weeks later, alive, unidentified, not because no one was looking, but because there's often no easy way to connect a person found in one place to a report filed in another. TraceKE closes that gap.

- Designed the confidence score to be multi-signal on purpose, not just face similarity: facial embedding match carries 55% of the score, age estimation 25%, gender 20%. Location is context only, never a penalty, because a person found 400km from home may have been trafficked, not misidentified
- Made the harder call to never reject a low-quality photo. For some families, one blurry image is the only one they have, so the system flags uncertainty and redistributes confidence weights instead of discarding data
- Documented the model's limitations as rigorously as its features: Facenet was trained predominantly on Western datasets and hasn't been independently benchmarked on East African faces under real-world lighting and resolution, the single biggest gap the next version needs to close

`Python` `Streamlit` `Facenet-PyTorch` `ChromaDB` `OpenCV (YuNet)` `Face Recognition`

---

### 💳 SME Credit Risk Intelligence Platform

**[GitHub →](https://github.com/kerubobosire254/sme-credit-risk-scoring-app)**

<!-- Add a screenshot of the SHAP explainability dashboard here: ![SME Credit Risk demo](./assets/sme-credit-demo.png) -->

Small businesses in Africa are starved of credit not because they're bad borrowers, but because lenders have no reliable, fast way to assess their risk. Traditional credit scoring wasn't built for SMEs with thin or informal financial histories.

- Uses XGBoost and KMeans clustering to score SME creditworthiness and segment borrowers by risk profile
- Includes batch scoring for multiple applicants, SHAP-based model explainability so you can see *why* a decision was made, and a full interactive dashboard
- Built with actuarial rigour: no random noise injected into predictions, deterministic and auditable by design

`XGBoost` `KMeans` `SHAP` `Streamlit` `Credit Scoring` `Batch Processing`

---

### 🩺 BreastCare Kenya

**[GitHub →](https://github.com/kerubobosire254/breastcancer_help_app)**

Published KAP research shows Kenyan practitioners know breast cancer screening guidelines (54.7%) but don't consistently act on them (29.2%, as low as 12.7% among community health workers), a major reason patients aren't caught until Stage III or IV.

- Built a 7-module clinical decision support app where each patient encounter drives the next stage of care: symptoms flow into the screening checklist, red flags trigger referrals, referrals generate follow-up records, all with zero duplicate data entry
- Engineered to run fully offline: weighted risk-scoring engine, evidence-based referral system, and CareBot (a rule-based NLP assistant covering 11 breast cancer topics), so practitioners get guidance with no internet, API keys, or subscriptions required

`Streamlit` `NLP` `Plotly`

---

### ⚽ World Cup 2026 Match Predictor

**[GitHub →](https://github.com/kerubobosire254/World-Cup-2026-Predictor)**

Every four years, millions of people predict World Cup results with complete confidence. Every four years, Argentina loses to Saudi Arabia and ruins everything.

- Built a match predictor for all 48 WC 2026 teams, trained on 964 World Cup matches back to 1930, that gives real win probabilities and likely scorelines
- The trickiest part was stopping it from just predicting "home win" every time (technically 57% accurate but useless); fixed by adjusting output probabilities to match real-world outcome frequencies
- Built a live feedback loop: enter real results as the tournament plays out and every team's form and rating recalculates on the fly

`Python` `XGBoost` `Poisson Regression` `ELO Ratings` `Streamlit`

---

### 🧠 Brainy — ADHD Executive Function App

**[Live Demo →](https://kerubobosire254.github.io/executive-function-app/)** · **[GitHub →](https://github.com/kerubobosire254/executive-function-app)**

ADHD isn't simply about being unable to focus. For many people, the harder part is starting tasks, breaking them down, and actually finishing things.

- Built Brainy around how ADHD brains actually struggle with tasks: turning overwhelming tasks into manageable actions, capturing thoughts before they disappear, and using focused work sessions to get started
- Responsive web app with interactive task flows, timers, reminders, calendar functionality, and persistent UI state

`HTML` `CSS` `JavaScript`

---

## 🧪 More Experiments

A few smaller builds that taught me just as much, because something always breaks:

- **[SentimentIQ](https://github.com/kerubobosire254/sentiment-analysis_app)** — NLP sentiment engine; benchmarked Naive Bayes, Logistic Regression, and Linear SVM with 5-fold CV, plus word-level explainability and bulk CSV processing
- **[SpotifyDNA](https://github.com/kerubobosire254/The-spotify-data-analysis)** — Infers personality archetypes and mood trends from your own Spotify export
- **[Stock Price Intelligence Terminal](https://github.com/kerubobosire254/Stock-Price-Prediction-API)** — LSTM price prediction, RSI/MACD/Bollinger overlays, and 600-path Monte Carlo simulation

---

## 🧰 Tech Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat&logo=postgresql&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)

![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=flat&logo=scikitlearn&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-EB0028?style=flat)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat&logo=tensorflow&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat&logo=opencv&logoColor=white)

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat&logo=react&logoColor=black)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat&logo=streamlit&logoColor=white)

![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)
![Render](https://img.shields.io/badge/Render-46E3B7?style=flat&logo=render&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat&logo=vercel&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat&logo=amazonaws&logoColor=white)

---

## 📊 GitHub Activity

<!-- These render automatically once your username is set correctly, no image upload needed -->
![Kerubo's GitHub stats](https://github-readme-stats.vercel.app/api?username=kerubobosire254&show_icons=true&theme=tokyonight&hide_border=true)
![GitHub Streak](https://github-readme-streak-stats.herokuapp.com/?user=kerubobosire254&theme=tokyonight&hide_border=true)

---

<div align="center">

### 🤝 Let's Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/kerubo-bosire-364523283)
[![Gmail](https://img.shields.io/badge/Email-Reach%20Out-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:kerubobosire254@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-Explore%20My%20Work-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/kerubobosire254)

**Open to ML Engineer roles.** If you're reading this, you've already seen more of my work than most job descriptions ask for. Let's talk.

</div>
