<img src="https://readme-typing-svg.herokuapp.com?font=JetBrains+Mono&size=26&pause=1000&color=58A6FF&vCenter=true&width=850&lines=Business+x+Data+x+AI+Problem+Solver;10%2B+Years+Retail+Operations+%2B+Data+Science;Business+Questions+%E2%86%92+Data+%E2%86%92+Decisions" />

# Troy Dela Rosa

**Business x Data x AI Problem Solver** | Winnipeg, MB | Available for a Winter 2027 co-op (Jan 2027)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-tdra48-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/tdra48)
[![Email](https://img.shields.io/badge/Email-troy.dlrs%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:troy.dlrs@gmail.com)
[![Live Demo](https://img.shields.io/badge/Live%20Demo-PFA--GA4-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)](https://rynetroy-predictive-funnel-analytics-ga-appstreamlit-app-dcavuj.streamlit.app/)
[![Demo Video](https://img.shields.io/badge/Demo-Sandra%20%2B%20Margaux-D97757?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/feed/update/urn:li:activity:7516652514100936704/)

---

## At a Glance

| | |
|---|---|
| **Education** | Data Science & Machine Learning, Applied Diploma, Red River College Polytechnic (Aug 2025 to May 2027) |
| **Experience** | 10+ years in retail operations, most recently Store Director at Saks OFF 5TH ($2M+ store, 6 leaders, 15 associates) |
| **Focus** | Data analytics, business intelligence, data governance, predictive modeling, applied AI |
| **Looking for** | Winter 2027 co-op or internship in data analytics, BI, data governance or applied AI. Eligible to work full-time in Canada |

## How I Work

I spent 10+ years running retail stores, reading sales, margin, traffic and inventory reports every week to decide what to do next. Now I'm building the other half: SQL, Power BI, Python and machine learning.

A model can be accurate and still solve the wrong problem, so every project below answers three questions:

**What is happening? → So what does it mean? → What should be done next?**

<details>
<summary>🐍 <b>framework.py: Not All Pain Is Progress</b> (the story behind the career change)</summary>

<br/>

After more than a decade in retail leadership, the store I'd built my career around closed. Instead of climbing the same ladder somewhere else, I went back to school. I used to measure progress by career height. Now I measure it by what I can do that I couldn't do before. This small script is that idea told in a language I'm learning (a personal story, not an application).

```python
"""
NOT ALL PAIN IS PROGRESS
A Personal Framework for Career Evolution
"""

from dataclasses import dataclass, field


@dataclass
class CareerState:
    title: str
    years_built: int
    skills: list[str] = field(default_factory=list)
    progress_metric: str = "career_height"


class ProfessionalJourney:

    def __init__(self):
        self.state = CareerState(
            title="Store Director",
            years_built=10,
            skills=[
                "Leadership",
                "Operations",
                "People Management",
                "Business Decision Making",
                "Decision Making Under Pressure",
            ],
        )

    def trigger_disruption(self):
        print(">>> EVENT: Store closure announced.")
        print(">>> RESULT: The old career path is no longer available.")

    def redefine_progress(self):
        self.state.progress_metric = "capability"

        print("--- PERSPECTIVE SHIFT ---")
        print("Old metric: Career height")
        print("New metric: Capability")

    def execute_pivot(self):
        new_capabilities = [
            "Python",
            "Statistics",
            "Linear Algebra",
            "SQL",
            "Data Analysis",
            "Machine Learning",
        ]

        self.state.skills.extend(new_capabilities)
        self.state.title = "Data Science & Machine Learning Student"

    def calculate_trajectory(self):
        return """
Progress is not a straight line upward.

Sometimes the ladder disappears.

The old life is gone.
The foundation remains.
The direction has changed.

Not all pain is progress,
but the right kind of discomfort
builds something the old version of you didn't have.
"""


if __name__ == "__main__":
    journey = ProfessionalJourney()

    journey.trigger_disruption()
    journey.redefine_progress()
    journey.execute_pivot()

    print(journey.calculate_trajectory())
```

</details>

---

## 📊 Data & Analytics Projects

### Predictive Funnel Analytics (PFA-GA4)
**Independent Academic Project** | Supervised Machine Learning (COMP-2704) | Apr 2026
`Python` `pandas` `scikit-learn` `XGBoost` `SHAP` `Streamlit`

<a href="https://github.com/rynetroy/Predictive-Funnel-Analytics-GA4"><img src="https://github.com/rynetroy/Predictive-Funnel-Analytics-GA4/raw/main/visualizations/propensity_decile.png" width="450" alt="Conversion rate by propensity decile" /></a>

- **The top 10% of sessions converted at 3x the baseline (15.33% vs 5.16%),** so a marketing team could focus spend there instead of treating every visitor the same.
- XGBoost model (~0.80 ROC-AUC) with leakage checks and calibrated probabilities (Platt scaling), turned into expected revenue ($1.98M predicted vs $1.74M actual on the test set, +13.6%) and explained with SHAP in a live Streamlit demo.

🔗 [Repository](https://github.com/rynetroy/Predictive-Funnel-Analytics-GA4) | [Live demo](https://rynetroy-predictive-funnel-analytics-ga-appstreamlit-app-dcavuj.streamlit.app/)
<sub>Prototype on synthetic GA4-style data. Not a production model.</sub>

### Winnipeg Business Licence Data Governance (DAMA-DMBOK)
**Independent Personal Project** | Data governance on public data | Nov 2026, in progress
`Python` `pandas` `DuckDB` `SQL` `REST API` `matplotlib` `DAMA-DMBOK`

<a href="https://github.com/rynetroy/winnipeg-licence-governance"><img src="https://github.com/rynetroy/winnipeg-licence-governance/raw/main/reports/figures/downtown_map.png" width="450" alt="Map of downtown Winnipeg and surrounding neighbourhoods: of 196 active licences in the City's Downtown planning area in November 2026, 5 are inside the CentrePlan 2050 downtown boundary" /></a>

- **Of 196 active licences the City's data labels "Downtown", only 5 are inside the City's own downtown plan boundary (CentrePlan 2050);** most of the rest are rooming houses in surrounding neighbourhoods. The count also depended on the pull date: in April 2026, 621 records said "Issued" but only 34 were active once duplicates and expired licences were removed.
- Built a pipeline that saves dated, never-overwritten snapshots from the City's open data API, compares them and maps licences by neighbourhood, plus a governance charter, RACI, decision log and code-generated data dictionary. Raw records stay out of the repo because some include addresses that may belong to individuals.

🔗 [Repository](https://github.com/rynetroy/winnipeg-licence-governance)
<sub>Personal project on City of Winnipeg open data, not affiliated with or endorsed by the City. Downtown neighbourhoods matched to the CentrePlan 2050 map by eye. Next: quality rules, scorecard and a Power BI report.</sub>

### DROP IF Orphan: Game Store Database (SQL)
**Team Academic Project (5 members)** | Transforming Data Into Databases (COMP-1701) | Apr 2026, portfolio edition Nov 2026
`SQL` `MySQL` `MariaDB` `GitHub Pages`

<a href="https://github.com/rynetroy/game_store_database"><img src="https://github.com/rynetroy/game_store_database/raw/main/images/erd.png" width="450" alt="Entity relationship diagram of the 17-table game store database" /></a>

- **The schema let 18 of 35 table bookings fall outside store hours.** I added 19 validation checks and a data quality report so problems like this are caught before they reach reports and pricing.
- In a 5-person team building a 17-table MySQL database, I wrote the busiest-day and peak-pricing queries, then rebuilt the repo so it runs from scratch (fixed a load error that left 5 tables empty, plus date-window, tie and revenue bugs).

🔗 [Repository](https://github.com/rynetroy/game_store_database) | [Project site](https://rynetroy.github.io/game_store_database/)

### Downtown Winnipeg Transition Analysis
**Independent Academic Project** | Python Essentials With Data Analysis (COMP-2040) | Apr 2026
`Python` `pandas` `matplotlib` `scikit-learn`

<a href="https://github.com/rynetroy/downtown-winnipeg-transition-analysis"><img src="https://github.com/rynetroy/downtown-winnipeg-transition-analysis/raw/main/visuals/fig_vacancy.png" width="450" alt="Office vacancy rates: Winnipeg vs. the national average, 2016 to 2025" /></a>

- **Downtown office vacancy more than doubled, from 8.7% (2016) to 18.6% (2025).**
- I combined vacancy, investment pipeline and business-activity data into a weighted scenario index: 63/100 today, ~72 if planned development stays on schedule, ~34 if it stalls.

🔗 [Repository](https://github.com/rynetroy/downtown-winnipeg-transition-analysis)
<sub>The score is a constructed scenario index, not an official city metric. Some vacancy years are estimated; see the repo for methodology.</sub>

### Superstore Sales Dashboard (Power BI)
**Independent Academic Project** | Data Management (COMP-2702) | Apr 2026
`Power BI` `DAX` `Power Query`

<a href="https://github.com/rynetroy/Retail-Sales-Forecasting-Pricing-Analytics"><img src="https://github.com/rynetroy/Retail-Sales-Forecasting-Pricing-Analytics/raw/main/images/02_sales_by_region.png" width="450" alt="Superstore Power BI report: sales, average discount and profit margin by region" /></a>

- **Central gave the deepest discounts (24%) and earned the lowest margin (7.9%), and its furniture sales lost money (-1.9%).** The West had the lowest discounts (11%), the most sales ($725K) and the best margin (14.9%).
- Star schema in Power Query with a DAX date table, DAX measures (margin, YoY growth with SAMEPERIODLASTYEAR), and a 5-page report published to Power BI Service.

🔗 [Repository](https://github.com/rynetroy/Retail-Sales-Forecasting-Pricing-Analytics)
<sub>Built on the Superstore practice dataset. Discount and margin patterns are correlations, not tested causes.</sub>

---

## 🤖 AI Builds

### Troy OS: Personal AI Workspace (Sandra + Margaux)
**Personal Project** | Oct 2026
`Claude Code` `AI agents` `Slack integration` `Human-in-the-loop` `Permission design`

- **The main design work was deciding what each agent is not allowed to do.** Every assistant starts read-only and gets more access only after it proves reliable. I designed the roles, access limits and approval rules; Claude Code generated most of the code.
- **Margaux** sorts my website inquiries and drafts replies from approved copy. She never quotes prices or promises dates, and sends nothing except my booking link without my approval in Slack.
- **Sandra** is voice-activated with read-only access to my email, calendar and school deadlines, and sends morning briefs and evening recaps in Slack. Anything that needs action comes to me.

🎥 [Watch the Sandra + Margaux demo on LinkedIn](https://www.linkedin.com/feed/update/urn:li:activity:7516652514100936704/)
<sub>Personal tool for my own use. Code is private; the demo shows it working.</sub>

### Dynamic Hand Gesture Recognition (CNN + GRU)
**Team Academic Project (5 members, in progress)** | Neural Networks & Deep Learning (COMP-3704) | Fall 2026
`TensorFlow` `Keras` `CNN` `GRU` `OpenCV`

- A webcam controller that recognizes dynamic hand gestures (Jester dataset) and turns them into presentation commands, comparing a CNN-only baseline with a CNN-GRU model.
- I'm the real-time application lead: OpenCV webcam capture, running the model on live video, mapping gestures to commands, and safety controls (confidence thresholds, cooldowns) so normal hand movements don't trigger actions. Demo expected Dec 2026.

🔗 [Team repository](https://github.com/Qteneqja/GestureController)

---

## 🤝 Riipen Team Projects

**FanRyng (Toronto startup)** | Riipen Labs, Team 71, Research Lead | Aug 2026
- **Recommended piloting Live Trivia + Make Some Noise!** after leading research for a 5-person team across 7 NCAA Division I programs, with a 30/60/90-day rollout plan and KPIs.

**Astrum Digital** | Riipen Level Up (March Cohort), Team Project (2 members) | Feb 2026
- Led product strategy for an AI-driven portfolio platform for retail investors: four investor personas, a KPI framework and the 16-slide project deck.

---

## 💼 Professional Experience

**Saks OFF 5TH, Winnipeg** | Store Director, Assistant Store Director, Selling Manager | May 2018 to Apr 2025
- Ran a $2M+ store (6 leaders, 15 associates, 6 departments), responsible for sales, margin (~40% gross profit), payroll (~20%) and expenses.
- Used weekly Looker sales-to-stock dashboards (this year vs last year), Storeforce reports and traffic data to make staffing, inventory, markdown and assortment decisions; managed 15K to 20K units with shrink below 2%.

**H&M, Winnipeg** | Visual Merchandising Manager; Keyholder | Aug 2014 to Apr 2018
- Part of the $4M Kildonan Place store launch; keyholder at H&M's first Winnipeg location ($10M+).

---

## 🎓 Education & Certifications

**Red River College Polytechnic**, Data Science & Machine Learning, Applied Diploma | Aug 2025 to May 2027
Coursework: Python, SQL, Statistics, Machine Learning, Data Management, Information & Data Architecture, Unsupervised ML, Neural Networks & Deep Learning, Introduction to AI

**Certifications:** Introduction to MongoDB, MongoDB, Inc. (Apr 2026) · Collaboration and Team Dynamics, IBM SkillsBuild (Aug 2026) · Preparing for AWS Certified AI Business Strategist (AIB-C01) · AWS Academy Data Engineering, in progress (coursework)

---

## 🛠️ Technical Skills

**Databases & SQL**
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![DuckDB](https://img.shields.io/badge/DuckDB-FFF000?style=flat-square&logo=duckdb&logoColor=black)

**BI & Reporting**
![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat-square&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-F2C811?style=flat-square&logo=powerbi&logoColor=black)
![Power Query](https://img.shields.io/badge/Power%20Query-217346?style=flat-square&logo=microsoft&logoColor=white)
![Excel](https://img.shields.io/badge/Excel-217346?style=flat-square&logo=microsoftexcel&logoColor=white)

**Python & Machine Learning**
![Python](https://img.shields.io/badge/Python-3670A0?style=flat-square&logo=python&logoColor=ffdd54)
![pandas](https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-FF6600?style=flat-square)
![SHAP](https://img.shields.io/badge/SHAP-8A2BE2?style=flat-square)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)

**Tools**
![Git](https://img.shields.io/badge/Git-F05033?style=flat-square&logo=git&logoColor=white)
![Claude Code](https://img.shields.io/badge/Claude%20Code-D97757?style=flat-square&logo=anthropic&logoColor=white)

<sub>Also used in coursework: NumPy, Matplotlib, Jupyter, MongoDB, TensorFlow, GitHub Pages, Jira.</sub>

---

## 📬 Connect

Looking for a Winter 2027 co-op or internship in data analytics, BI, data governance or applied AI. Happy to connect with anyone working where business and data meet.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Troy%20Dela%20Rosa-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/tdra48)
[![Email](https://img.shields.io/badge/Email-troy.dlrs%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:troy.dlrs@gmail.com)

📍 Winnipeg, MB | Open to opportunities across Canada

I'm also building [TDRA Consulting](https://tdraconsulting.com), a small data and BI practice for local businesses. It's in development, and Margaux (above) handles its inbox.

![Profile Views](https://komarev.com/ghpvc/?username=rynetroy&label=Profile%20Views&color=58A6FF&style=flat-square)
