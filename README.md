<div align="left">

# Hi, I'm Baran Erdogan 👋

### MSc Business Analytics · ESADE Business School
**Building at the intersection of machine learning, cloud infrastructure, and operational intelligence**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](www.linkedin.com/in/baran-erdogan-34526921a)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/baranerdogan11)
[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:erdoganbaran98@gmail.com)

</div>

---

## About Me

I'm a Business Analytics student at ESADE with a passion for turning messy, real-world data into systems that actually work in production. I'm particularly drawn to problems where ML meets physical processes — manufacturing, logistics, operations — where a good prediction has a tangible, measurable impact.

I come from **[YOUR BACKGROUND — e.g. a background in industrial engineering / finance / consulting]**, which gave me a strong appreciation for the gap between theoretical models and operational reality. At ESADE I've been closing that gap — building end-to-end pipelines from raw sensor data all the way to cloud-deployed inference endpoints.

- Based in **Barcelona, Spain**
- Fluent in **[Turkish, English, Spanish]**
- Looking for roles in **Data Science, ML Engineering, or Analytics Engineering**

---

## Tech Stack

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)
![R](https://img.shields.io/badge/R-276DC3?style=flat-square&logo=r&logoColor=white)

**Data & ML**

![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-0071C5?style=flat-square&logo=xgboost&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white)

**Cloud & Infrastructure**

![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazon-aws&logoColor=white)
![SageMaker](https://img.shields.io/badge/SageMaker-FF9900?style=flat-square&logo=amazon-aws&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)

**Apps & Dashboards**

![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

---

## Featured Projects

### VaultTech — Industrial Cycle Time Prediction
> **Real industrial ML case study** · Python · XGBoost · PostgreSQL · Streamlit · AWS SageMaker

A full end-to-end ML pipeline built on ~180k PLC sensor readings from a steel forging line producing track chain links for heavy earthmoving equipment. Each piece travels ~58 seconds through four zones: Furnace → Main Press (4 strikes) → Auxiliary Press → Quench Bath.

**The core challenge:** predict total bath time using only data available after the *2nd strike* — just 18 seconds into the process — giving operators a real-time early-warning signal for anomalous pieces.

**What I built:**
- **Medallion data architecture** (Bronze → Silver → Gold) backed by PostgreSQL 16 with versioned Flyway migrations
- **XGBoost regression model** with 3 carefully constrained features (die matrix, 2nd-strike timing, rolling OEE) — achieving sub-second inference
- **Streamlit dashboard** for live cycle time monitoring and delay alerts
- **AWS deployment** via SageMaker Model Registry + real-time endpoints, containerised with Docker and hosted on ECS/Fargate

The constraint-driven feature selection (nothing after the 2nd strike is allowed) is the interesting design decision here — the model is useless if it's accurate but late.

---

### [YOUR SECOND PROJECT]
> **[Brief description]** · [Tech stack]

[2–3 sentence description of the project, the problem it solves, and what you built]

---

### [YOUR THIRD PROJECT]
> **[Brief description]** · [Tech stack]

[2–3 sentence description of the project, the problem it solves, and what you built]

---

## GitHub Stats

<div align="center">

![Baran's GitHub Stats](https://github-readme-stats.vercel.app/api?username=BaranErdogan&show_icons=true&theme=github_dark&hide_border=true&include_all_commits=true)
&nbsp;
![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=BaranErdogan&layout=compact&theme=github_dark&hide_border=true)

</div>

---

## What I'm Thinking About

- How far can **constraint-aware ML** go in manufacturing — models that know what they're not allowed to see
- **Medallion architecture** as a pattern for analytics engineering, not just data warehousing
- The line between a **data analyst** and an **ML engineer** — I think it's blurring fast

---

<div align="center">

*Open to opportunities in data science, ML engineering, and analytics engineering — especially where the data is messy and the stakes are real.*

**[LinkedIn](https://linkedin.com/in/YOUR_LINKEDIN) · [Email](mailto:YOUR_EMAIL@esade.edu)**

</div>

