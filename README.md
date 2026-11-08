<img src="https://readme-typing-svg.herokuapp.com?font=JetBrains+Mono&size=24&pause=1000&color=58A6FF&vCenter=true&width=850&lines=Analytics+%26+Business+Intelligence;10%2B+Years+Retail+Operations+%E2%86%92+Data+%26+Analytics;What+is+happening%3F+%E2%86%92+So+what%3F+%E2%86%92+What+next%3F" />

# Troy Dela Rosa

**Analytics & Business Intelligence Student | Former Retail Store Director** | Winnipeg, MB  
Available for Winter 2027 Co-op / Internship (January 2027)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-tdra48-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/tdra48)
[![Email](https://img.shields.io/badge/Email-troy.dlrs%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:troy.dlrs@gmail.com)
[![Live Demo](https://img.shields.io/badge/Live%20Demo-PFA--GA4-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)](https://rynetroy-predictive-funnel-analytics-ga-appstreamlit-app-dcavuj.streamlit.app/)
[![Demo Video](https://img.shields.io/badge/Demo-Sandra%20%2B%20Margaux-D97757?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/feed/update/urn:li:activity:7516652514100936704/)

---

## At a Glance

| | |
|---|---|
| **Education** | Applied Diploma in Data Science & Machine Learning, Red River College Polytechnic (Aug 2025 to May 2027) |
| **Work Background** | 10+ years in retail management. Store Director at Saks OFF 5TH Winnipeg (store P&L, shrink, inventory, scheduling, team of 15 associates). Earlier Visual Merchandising Manager at H&M Winnipeg |
| **Technical Focus** | Business intelligence, dimensional modeling (star schema), data governance (DAMA-DMBOK), predictive analytics |
| **Availability** | Full-time Winter 2027 co-op / internship (Data Analyst, BI, Data Governance, Operations Analytics). Eligible to work in Canada |



---

## How I Work

> **"If you look at my work, you'll see a consistent pattern: I specialize in data reconciliation and funnel auditing.** I take high-volume, inconsistent raw data and apply governance, validation, testing, and analytical methods to separate meaningful signals from the noise. My focus is identifying the small percentage of data, patterns, or workflows that actually matter for business decisions. I don't just build pipelines; I build systems that help distinguish what matters from what doesn't."

For over a decade, I ran retail stores using weekly sales, margin, inventory, and traffic reports to guide staffing, merchandising, and operational priorities. As someone who relied on these reports to make business decisions, I saw where they helped and where they fell short: information that arrived late, metrics that didn't reflect operational reality, and dashboards that showed what happened without explaining what to do next.

Now I build the data layers behind those reports: relational databases, dimensional models (star schemas), automated data quality checks, and explainable analytical models.

Every project below aims to answer three questions:  
**What is happening?** ➔ **So what does it mean?** ➔ **What should be done next?**

---

## 📊 Analytics & BI Projects

### 1. Superstore Sales & Margin Dashboard (Power BI)
**Academic Project (solo)** | Data Management (COMP-2702) | Apr 2026  
`Power BI` `DAX` `Power Query` `Star Schema`

<a href="https://github.com/rynetroy/Retail-Sales-Forecasting-Pricing-Analytics"><img src="https://github.com/rynetroy/Retail-Sales-Forecasting-Pricing-Analytics/raw/main/images/02_sales_by_region.png" width="480" alt="Superstore Power BI report: sales, average discount and profit margin by region" /></a>

- **Finding:** Central had the deepest average discount (24%) and the weakest margin (7.9%), with Furniture running at a loss (-1.9%). West discounted less (11%) and earned a 14.9% margin on $725K in sales.
- **Build:** Star schema in Power Query (fact table plus dimension tables), a DAX date table and time intelligence measures (including `SAMEPERIODLASTYEAR`), published as a 5-page Power BI Service report: Dashboard, Sales by Region, Predictive Insights, Prescriptive Recommendation, Certified Visual.

🔗 [Repository](https://github.com/rynetroy/Retail-Sales-Forecasting-Pricing-Analytics)

---

### 2. Winnipeg Business Licence Data Governance (DAMA-DMBOK)
**Independent Project** | City of Winnipeg Open Data | Nov 2026, in progress  
`dbt` `DuckDB` `SQL` `Python` `DAMA-DMBOK` `Data Quality`

<a href="https://github.com/rynetroy/winnipeg-licence-governance"><img src="https://github.com/rynetroy/winnipeg-licence-governance/raw/main/reports/figures/downtown_map.png" width="480" alt="Map of downtown Winnipeg business licences" /></a>

- **Finding:** Of 196 active licences tagged "Downtown" in the open data, only 5 fall inside the CentrePlan 2050 downtown boundary. The dataset's "Downtown" label and the official planning boundary define downtown differently, so analysis needs to pick one deliberately.
- **Cleaning:** Filtered 621 historical records to 34 valid active licences after removing expired and duplicate entries.
- **Build:** Repeatable extraction pipeline saving raw DuckDB snapshots, modular dbt transformation layers (staging ➔ intermediate ➔ marts) with automated data quality test assertions, auto-generated data dictionary, and DAMA-DMBOK documentation.

🔗 [Repository](https://github.com/rynetroy/winnipeg-licence-governance)

---

### 3. Predictive Funnel Analytics (PFA-GA4)
**Academic Project (solo)** | Supervised Machine Learning (COMP-2704) | Apr 2026  
`Python` `pandas` `scikit-learn` `XGBoost` `SHAP` `Streamlit`

<a href="https://github.com/rynetroy/Predictive-Funnel-Analytics-GA4"><img src="https://github.com/rynetroy/Predictive-Funnel-Analytics-GA4/raw/main/visualizations/propensity_decile.png" width="480" alt="Conversion rate by propensity decile" /></a>

- **Finding:** On synthetic GA4-style ecommerce sessions, the top propensity decile converted at about 3x the baseline (15.4% vs 5.2%), and the top 20% of sessions accounted for about 55% of revenue. In a real setting, that ranking could help focus retargeting spend.
- **Model:** Calibrated XGBoost conversion model (ROC-AUC about 0.80; other classifiers tested landed at a similar level) combined with a linear regression spend estimate: expected revenue = P(conversion) × predicted spend. Calibrated expected revenue came out at $1.98M vs $1.74M actual (+13.6%).
- **App:** Streamlit prototype with SHAP explanations. Not a production system.

🔗 [Repository](https://github.com/rynetroy/Predictive-Funnel-Analytics-GA4) | [Interactive App](https://rynetroy-predictive-funnel-analytics-ga-appstreamlit-app-dcavuj.streamlit.app/)

---

### 4. Game Store Relational Database
**Team Academic Project (5 members)** | Transforming Data Into Databases (COMP-1701) | Apr 2026  
`SQL` `MySQL` `MariaDB` `Schema Design` `Data Integrity`

<a href="https://github.com/rynetroy/game_store_database"><img src="https://github.com/rynetroy/game_store_database/raw/main/images/erd.png" width="480" alt="Entity relationship diagram of the 17-table game store database" /></a>

- **Team work:** 17-table normalized schema, 19 validation constraints and audit queries (including a fix that blocks table bookings outside store hours), peak-pricing and capacity reports, and reproducible setup scripts. Schema, scripts and data were built together by the team.
- **Now:** I'm cleaning up and documenting a portfolio edition of the project (Nov 2026).

🔗 [Repository](https://github.com/rynetroy/game_store_database) | [Project Site](https://rynetroy.github.io/game_store_database/)

---

## 🤝 Riipen Team Projects

- **FanRyng** (Riipen Labs, team of 5): research and strategy for a Toronto fan engagement startup on NCAA Division I programs. I led the research, built the Excel research tracker and wrote the final report; the strategy was developed with the team.
- **Astrum Digital** (Riipen, team of 2 with Mary Zhou): concept work on an explainable AI portfolio intelligence tool for retail investors.

---

## 🤖 Personal AI Project

### Troy OS: Personal Assistant Workspace (Sandra + Margaux)
**Personal Prototype** | Oct 2026, in use  
`AI Agents` `Human-in-the-Loop` `Slack API` `Permission Design`

- **Sandra:** reads my email and calendar (read-only) and sends morning briefs and evening recaps in Slack.
- **Margaux:** drafts replies to TDRA Consulting inquiry emails using approved website copy. She never quotes prices or commits to dates, holds suspicious emails, and anything involving price, scope or contracts waits for my approval in Slack.
- **My role:** I designed the system, workflows, guardrails and permission rules. Most of the code was written with AI assistance (Claude Code). The code is private; the demo video shows it working.

🎥 [Watch the demo](https://www.linkedin.com/feed/update/urn:li:activity:7516652514100936704/)

---

## 🛠️ Skills

| Area | Tools | What I've done with them |
| :--- | :--- | :--- |
| **BI & Analytics** | Power BI, DAX, Power Query, Excel | Star schema models, time intelligence, multi-page reports, margin analysis |
| **SQL & Data Modeling** | MySQL, MariaDB, DuckDB | Normalized schema design (team), validation queries, snapshot pipelines |
| **Data Governance** | DAMA-DMBOK | Governance charter, RACI matrix, data dictionary, data quality rules |
| **Python & ML** | pandas, NumPy, scikit-learn, XGBoost, SHAP, Streamlit | Propensity modeling, probability calibration, model explanations, prototype apps |
| **Retail Operations** | Store management | Store P&L, shrink, inventory, staff scheduling, visual merchandising |

---

## 🎓 Education & Certifications

**Red River College Polytechnic**, Data Science & Machine Learning, Applied Diploma | Aug 2025 to May 2027  
Coursework: Python, SQL, Statistics, Machine Learning, Data Management, Information & Data Architecture, Unsupervised ML, Neural Networks & Deep Learning, Introduction to AI

**Certifications:** Introduction to MongoDB, MongoDB, Inc. (Apr 2026) · Collaboration and Team Dynamics, IBM SkillsBuild (Aug 2026)  
**In progress:** AWS Certified AI Business Strategist (AIB-C01), exam prep


---

## 📬 Contact

* **Target roles:** Data Analyst, BI Analyst, Data Governance Analyst, Operations Analytics
* **Co-op availability:** Full-time from January 2027 (Winter 2027 term)
* **Location:** Winnipeg, MB (open to local, hybrid or remote roles in Canada)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Troy%20Dela%20Rosa-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/tdra48)
[![Email](https://img.shields.io/badge/Email-troy.dlrs%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:troy.dlrs@gmail.com)

Founder of [TDRA Consulting](https://tdraconsulting.com), an early-stage practice focused on practical data and BI for small businesses.
