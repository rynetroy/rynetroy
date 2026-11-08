<img src="https://readme-typing-svg.herokuapp.com?font=JetBrains+Mono&size=24&pause=1000&color=58A6FF&vCenter=true&width=850&lines=Business+Intelligence+%7C+Data+Analytics+%7C+Data+Governance;10%2B+Years+Retail+Operations+%E2%86%92+Data+%26+Decisions;What+is+happening%3F+%E2%86%92+So+what%3F+%E2%86%92+What+next%3F" />

# Troy Dela Rosa

**Business Intelligence | Data Analytics | Data Governance | Operations Analytics**  
Former Retail Store Director | Data Science & Machine Learning Student  
Winnipeg, Manitoba, Canada · Available for a Winter 2027 co-op or internship (January 2027)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-tdra48-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/tdra48)
[![Email](https://img.shields.io/badge/Email-troy.dlrs%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:troy.dlrs@gmail.com)
[![Live Demo](https://img.shields.io/badge/Live%20Demo-PFA--GA4-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)](https://rynetroy-predictive-funnel-analytics-ga-appstreamlit-app-dcavuj.streamlit.app/)
[![Demo Video](https://img.shields.io/badge/Demo-Sandra%20%2B%20Margaux-D97757?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/feed/update/urn:li:activity:7516652514100936704/)

---

## 👋 Profile

For over a decade, I ran retail stores, most recently as Store Director at Saks OFF 5TH Winnipeg ($2M+ store, 6 leaders, 15 associates). I used weekly sales, margin, inventory and traffic reports to guide staffing, merchandising and operational priorities. Relying on those reports, I saw where they helped and where they fell short: information that arrived late, metrics that didn't reflect what was happening on the floor, and dashboards that showed what happened without explaining what to do next.

Now I build the data layers behind those reports: relational databases, star schemas, data quality checks and explainable models. Most of my projects come down to the same job: checking what in the data can be trusted, and finding the small part that matters for the decision.

Every project below answers three questions:  
**What is happening?** ➔ **So what does it mean?** ➔ **What should be done next?**


---

## 🛠️ Technical Skills

| Area | Technologies & Methods |
| :--- | :--- |
| **Business Intelligence** | Power BI, DAX, Power Query, Excel, multi-page reports, margin analysis |
| **SQL & Databases** | SQL, MySQL, MariaDB, DuckDB, relational database design, validation queries |
| **Data Modelling** | Star schemas (fact and dimension tables), normalization, ERDs |
| **Data Governance** | DAMA-DMBOK, data profiling, data dictionaries, governance charter, RACI, decision log |
| **Data Pipelines** | REST API ingestion, dated snapshots, snapshot comparison, Python scripts |
| **Python & Analytics** | Python, pandas, NumPy, matplotlib, exploratory data analysis |
| **Machine Learning** | scikit-learn, XGBoost, SHAP, probability calibration, propensity modeling |
| **Apps & AI Workflows** | Streamlit, Slack integration, Claude Code, human-in-the-loop design |

---

## 📊 Featured Projects

### 1. Winnipeg Business Licence Data Governance
**Independent Personal Project** | City of Winnipeg open data | November 2026 (Phase 1 of 2, in progress)  
`Python` `pandas` `DuckDB` `SQL` `REST API` `DAMA-DMBOK`

<a href="https://github.com/rynetroy/winnipeg-licence-governance"><img src="https://github.com/rynetroy/winnipeg-licence-governance/raw/main/reports/figures/downtown_funnel.png" width="480" alt="Downtown licences counted as active, rule by rule: April 2026 621, 322, 34; November 2026 234, 197, 196" /></a>

* **Business Question:** Can the City of Winnipeg's business licence data be trusted for decisions like counting active downtown businesses?
* **Key Findings:**
  * Counting "Issued" licences overstated active downtown licences about 18 times in April 2026: 621 records, 322 after removing duplicates, 34 after removing expired licences.
  * Seven months later the same count gave 196, after the City cleaned up expired statuses (1,655 expired-but-"Issued" records citywide fell to 1), and nothing on the portal documented the change.
* **What I Built:**
  * A pipeline that pulls the City's open data API into dated snapshots that are never overwritten, then compares them (history added back to 2010, duplicate rows down from 55.8% to 15.6%).
  * A governance charter, RACI, decision log and a data dictionary generated from code.
  * Raw records stay out of the repo because some licence types include addresses that may belong to individuals.

🔗 [View Repository](https://github.com/rynetroy/winnipeg-licence-governance)  
<sub>Personal project on public data, not affiliated with or endorsed by the City of Winnipeg. Next: quality rules, scorecard and a Power BI report.</sub>

---

### 2. Superstore Sales & Margin Dashboard
**Independent Academic Project** | Data Management (COMP-2702) | April 2026  
`Power BI` `DAX` `Power Query` `Star Schema`

<a href="https://github.com/rynetroy/Retail-Sales-Forecasting-Pricing-Analytics"><img src="https://github.com/rynetroy/Retail-Sales-Forecasting-Pricing-Analytics/raw/main/images/02_sales_by_region.png" width="480" alt="Superstore Power BI report: sales, average discount and profit margin by region" /></a>

* **Business Question:** Which regions and categories earn their sales, and where is discounting costing more than it brings in?
* **Key Findings:**
  * Central had the deepest average discount (24%) and the weakest margin (7.9%), and its furniture sales lost money (-1.9% margin).
  * The West discounted least (11%) and earned the best margin (14.9%) on the most sales ($725K), so Central's discounting is the first thing to review.
* **What I Built:**
  * A star schema in Power Query from a 9,994-row sales file, with a DAX date table.
  * DAX measures for sales, profit, margin and year-over-year growth (`SAMEPERIODLASTYEAR`).
  * A 5-page report published to Power BI Service: Dashboard, Sales by Region, Sales Trends, Category Performance and Certified Visual.

🔗 [View Repository](https://github.com/rynetroy/Retail-Sales-Forecasting-Pricing-Analytics)  
<sub>Superstore practice dataset. Discount and margin patterns are correlations, not tested causes.</sub>

---

### 3. Predictive Funnel Analytics (PFA-GA4)
**Independent Academic Project** | Supervised Machine Learning (COMP-2704) | April 2026  
`Python` `pandas` `scikit-learn` `XGBoost` `SHAP` `Streamlit`

<a href="https://github.com/rynetroy/Predictive-Funnel-Analytics-GA4"><img src="https://github.com/rynetroy/Predictive-Funnel-Analytics-GA4/raw/main/visualizations/propensity_decile.png" width="480" alt="Conversion rate by propensity decile" /></a>

* **Business Question:** Which ecommerce sessions are most likely to convert, and where should marketing spend go first?
* **Key Findings:**
  * The top 10% of sessions converted at 15.3%, about 3x the 5.2% baseline.
  * The top 20% of sessions accounted for about 55% of expected revenue.
* **What I Built:**
  * A two-stage model: a calibrated XGBoost conversion classifier (ROC-AUC ~0.80) times a spend estimate, so expected revenue = P(conversion) × predicted spend ($1.98M predicted vs $1.74M actual on the test set, +13.6%).
  * Leakage checks with train, validation and test splits, and SHAP to explain what drives each score.
  * An interactive Streamlit demo for non-technical review.

🔗 [View Repository](https://github.com/rynetroy/Predictive-Funnel-Analytics-GA4) | 🚀 [Launch App](https://rynetroy-predictive-funnel-analytics-ga-appstreamlit-app-dcavuj.streamlit.app/)  
<sub>Academic prototype on synthetic GA4-style data, not a production model.</sub>

---

### 4. DROP IF Orphan: Game Store Database
**Team Academic Project (5 members)** | Transforming Data Into Databases (COMP-1701) | April 2026, portfolio edition November 2026  
`SQL` `MySQL` `MariaDB` `Data Quality`

<a href="https://github.com/rynetroy/game_store_database"><img src="https://github.com/rynetroy/game_store_database/raw/main/images/erd.png" width="480" alt="Entity relationship diagram of the 17-table game store database" /></a>

* **Key Finding:** The schema allowed 18 of 35 table bookings to fall outside store hours, so I added 19 validation checks and a data quality report to catch problems like this before they reach reports and pricing.
* **What We Built:** A 17-table MySQL database for a simulated game store covering table bookings, peak pricing and retail sales.
* **My Role:** Wrote the busiest-day query (table-hours) and the peak-pricing query (pricing each booking by its overlap with peak hours). Later rebuilt the repo so it runs from scratch, fixing a load error that left 5 of 17 tables empty plus date-window, tie and revenue bugs.

🔗 [View Repository](https://github.com/rynetroy/game_store_database) | 🌐 [Project Site](https://rynetroy.github.io/game_store_database/)

---

<details>
<summary>📁 <b>More projects</b> (Downtown Winnipeg analysis, hand gesture recognition)</summary>

<br/>

**Downtown Winnipeg Transition Analysis** | Independent Academic Project | Python Essentials With Data Analysis (COMP-2040) | April 2026  
`Python` `pandas` `matplotlib` `scikit-learn`
* **Downtown office vacancy more than doubled, from 8.7% (2016) to 18.6% (2025).**
* Combined vacancy, investment pipeline and business-activity data into a weighted scenario index: 63/100 today, ~72 if planned development stays on schedule, ~34 if it stalls.
* 🔗 [Repository](https://github.com/rynetroy/downtown-winnipeg-transition-analysis) <sub>(constructed scenario index, not an official city metric)</sub>

**Dynamic Hand Gesture Recognition (CNN + GRU)** | Team Academic Project (5 members, in progress) | Neural Networks & Deep Learning (COMP-3704) | Fall 2026  
`TensorFlow` `Keras` `CNN` `GRU` `OpenCV`
* A webcam controller that recognizes dynamic hand gestures (Jester dataset) and turns them into presentation commands, comparing a CNN-only baseline with a CNN-GRU model.
* I'm the real-time application lead: OpenCV webcam capture, running the model on live video, mapping gestures to commands, and safety controls (confidence thresholds, cooldowns). Demo expected December 2026.
* 🔗 [Team repository](https://github.com/Qteneqja/GestureController)

</details>

---

## 🤖 AI & Workflow Automation

### Troy OS: Personal AI Workspace (Sandra + Margaux)
**Personal Project** | October 2026  
`AI Agents` `Human-in-the-Loop` `Slack Integration` `Permission Design`

The main design work was deciding what each agent is not allowed to do. Every assistant starts read-only and gets more access only after it proves reliable. I designed the roles, access limits and approval rules; Claude Code generated most of the code.
* **Sandra (personal assistant):** Voice-activated, with read-only access to my email, calendar and school deadlines. Sends morning briefs and evening recaps in Slack, and reports anything that needs action instead of doing it.
* **Margaux (business inbox):** Sorts inquiries from my website and drafts replies from approved site copy. She never quotes prices or promises dates, holds suspicious messages, and sends nothing except my booking link without my approval in Slack.

🎥 [Watch the Demo](https://www.linkedin.com/feed/update/urn:li:activity:7516652514100936704/)  
<sub>Personal tool for my own use. Code is private; the demo shows it working.</sub>

---

## 🤝 Riipen Team Projects

* **FanRyng (Toronto startup), Riipen Labs, Research Lead, August 2026:** Led research for a 5-person team across 7 NCAA Division I programs and recommended piloting Live Trivia + Make Some Noise!, with a 30/60/90-day rollout plan and KPIs.
* **Astrum Digital, Riipen Level Up, Team Project (2 members), February 2026:** Led product strategy for an AI-driven portfolio platform for retail investors: four investor personas, a KPI framework and the 16-slide project deck.

---

## 💼 Professional Experience

**Saks OFF 5TH**, Winnipeg, MB  
*Store Director* (October 2019 to April 2025); earlier Assistant Store Director and Selling Manager (from May 2018)
* Ran a $2M+ store (6 leaders, 15 associates, 6 departments), responsible for sales, margin (~40% gross profit), payroll (~20%) and expenses.
* Used weekly Looker sales-to-stock dashboards (this year vs last year), Storeforce reports and traffic data to make staffing, inventory, markdown and assortment decisions.
* Managed 15K to 20K units with shrink below 2%.

**H&M**, Winnipeg, MB  
*Visual Merchandising Manager* (March 2017 to April 2018); earlier Keyholder (from August 2014)
* Part of the $4M Kildonan Place store launch; keyholder at H&M's first Winnipeg location ($10M+).

---

## 🎓 Education & Certifications

**Red River College Polytechnic**, Winnipeg, MB  
*Applied Diploma, Data Science & Machine Learning* | August 2025 to May 2027 (expected)  
Coursework: Python, SQL, Statistics, Machine Learning, Data Management, Information & Data Architecture, Unsupervised ML, Neural Networks & Deep Learning, Introduction to AI

* **Certifications:** Introduction to MongoDB (MongoDB, Inc., April 2026) · Collaboration and Team Dynamics (IBM SkillsBuild, August 2026)
* **In progress:** Preparing for AWS Certified AI Business Strategist (AIB-C01) · AWS Academy Data Engineering (coursework)

---

## 📬 Contact & Target Roles

* **Target roles:** Business Intelligence Analyst, Data Analyst, Data Governance Analyst, Operations Analyst
* **Availability:** Full-time Winter 2027 co-op or internship (starting January 2027)
* **Location:** Winnipeg, MB (open to on-site, hybrid or remote roles across Canada)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Troy%20Dela%20Rosa-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/tdra48)
[![Email](https://img.shields.io/badge/Email-troy.dlrs%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:troy.dlrs@gmail.com)

*I'm also building [TDRA Consulting](https://tdraconsulting.com), a small data and BI practice for local businesses. It's in development, and Margaux (above) handles its inbox.*
