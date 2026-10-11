# 📊 Customer Churn Analysis & Retention Intelligence

An end-to-end data analytics project uncovering the structural, behavioral, and operational drivers of subscription churn using Python, Pandas, Matplotlib, and Seaborn.

---

## 📌 Executive Summary

Customer acquisition costs significantly outpace retention expenses. This project evaluates subscription churn across customer demographics, plan tiers, and support service logs to diagnose why users abandon the platform and identify early warning signals for proactive retention.

* **Cohort Churn Rate:** 28.57% (Retention Rate: 71.43%)
* **Average Revenue Per User (ARPU):** $18.85
* **Monthly Revenue at Risk:** $73.94k in lost recurring revenue
* **Support Escalation Impact:** Strong positive correlation (**0.77**) between service ticket escalations and churn.

---

## 🏗️ Project Architecture & Pipeline

```text
Raw Data Ingestion (Excel: 3 Sheets)
       ↓
Data Audit & Quality Checks (NaNs, Categorical Inconsistencies, Datatypes)
       ↓
Feature Engineering (Age Cohorts, Churn Risk, Escalation Flags)
       ↓
Exploratory Data Analysis (Plan Tiers, Contract Terms, Geography)
       ↓
Statistical Correlation & Heatmap Analysis
       ↓
Actionable Retention Strategy

🛠️ Tech StackLanguage: PythonData Manipulation: Pandas, NumPyData Visualization: Matplotlib, SeabornDatabase / File Handling: OpenPyXL, SQLite / CSV🔍 Key Business Findings1. The Basic Tier Value GapSubscribers on the Basic tier experienced a 60.00% churn rate, compared to 22.22% on Standard and 14.29% on Premium. Feedback logs indicate content scarcity and pricing mismatches relative to utility.2. Support Escalations as Leading Churn PredictorsCustomers with escalated support tickets (escalations == 'Y') churned at an alarming rate (100% of escalated users left).The average customer satisfaction (CSAT) score among churned users was 31.7 / 100, compared to 90.0 / 100 for retained customers.3. Contract Commitment DiscrepancyMonthly Contracts: 55.6% churn rate | Average CLTV: $308.56Annual Contracts: 8.3% churn rate | Average CLTV: $1,209.75📈 VisualizationsMetric / ChartDescriptionCorrelation HeatmapShows high positive alignment between churn score, escalations, and cancellation status.Churn by Plan TierIdentifies severe drop-offs in introductory and basic subscriptions.Monthly TrendMaps churn seasonality over calendar periods.(Add your exported images under the images/ folder and link them here using ![Heatmap](images/correlation_heatmap.png))🚀 How to Run LocallyClone the repository:Bashgit clone [https://github.com/](https://github.com/)<YOUR_GITHUB_USERNAME>/customer-churn-analysis.git
cd customer-churn-analysis
Create and activate a virtual environment:Bashpython -m venv venv
# Windows:
venv\Scripts\activate
# macOS/Linux:
source venv/bin/activate
Install dependencies:Bashpip install -r requirements.txt
Launch Jupyter Notebook:Bashjupyter notebook notebooks/churn_analysis.ipynb
👤 AuthorMohammad RaheemLinkedIn | GitHub
---

