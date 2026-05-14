# 📊 Customer Support Operations KPI Dashboard | Python + Excel + Power BI

> An end-to-end automated reporting pipeline that transforms raw customer support ticket data into actionable operational insights using Python, Excel, and Power BI.

---

## 📌 Project Highlights

* Automated KPI pipeline for 500+ support tickets
* Built interactive Power BI dashboard for SLA monitoring
* Generated daily and weekly operational summaries
* Automated Excel reporting using Python
* Identified SLA breaches, escalation trends, and agent performance bottlenecks

---

## 🧩 Problem Statement

Customer support teams generate hundreds of tickets daily. Without proper operational tracking, SLA breaches go unnoticed, escalations are poorly monitored, and agent performance becomes difficult to evaluate.

This project builds an automated KPI reporting system that:

* Cleans raw support ticket data
* Calculates business-critical operational KPIs
* Generates Excel reports
* Delivers an interactive Power BI dashboard for decision-making

This simulates a real-world operations analytics workflow used by support and service teams.

---

## 🎯 KPIs Tracked

| KPI                           | Description                                            |
| ----------------------------- | ------------------------------------------------------ |
| **First Response Time (FRT)** | Time between ticket creation and first agent response  |
| **Resolution Time**           | Total time required to resolve a ticket                |
| **SLA Breach Rate**           | Percentage of tickets exceeding SLA limits             |
| **Escalation Analysis**       | Volume and types of escalations                        |
| **Agent Performance**         | Ticket volume, FRT, and resolution efficiency by agent |
| **Reopened Tickets**          | Tickets reopened after resolution                      |

---

## 🔍 Key Insights

* 38% SLA Breach Rate — 190 out of 500 tickets breached SLA limits
* Medium priority tickets showed the highest breach volume
* Critical tickets had the fastest resolution time but highest escalation rate
* Agent_Kumar handled the highest ticket volume with above-average resolution time
* Manager escalations were the most common escalation type, indicating potential first-line resolution gaps

---

## 💼 Business Impact

This dashboard helps operations managers:

* Monitor SLA compliance in real time
* Detect operational bottlenecks early
* Identify overloaded agents
* Track escalation patterns
* Improve response and resolution efficiency
* Support data-driven operational decisions

---

## 🛠️ Tech Stack

| Tool           | Purpose                                    |
| -------------- | ------------------------------------------ |
| **Python**     | Data cleaning, KPI calculation, automation |
| **Pandas**     | Data manipulation and aggregation          |
| **Matplotlib** | Exploratory data visualization             |
| **OpenPyXL**   | Automated Excel report generation          |
| **Power BI**   | Interactive dashboard and reporting        |

---

## 📁 Project Structure

```text
operations-kpi-dashboard/
│
├── data/
│   └── support_tickets_raw.csv
│
├── notebooks/
│   └── 01_cleaning_kpis.ipynb
│
├── output/
│   └── kpi_report.xlsx
│
├── dashboard/
│   └── operations_kpi_dashboard.pbix
    |__ dashboard_overview.png
│
├── requirements.txt
└── README.md
```

---

## ⚙️ Pipeline Workflow

```text
Raw CSV → Data Cleaning → KPI Calculation → Excel Export → Power BI Dashboard
```

### Step 1 — Data Cleaning

* Removed duplicate records
* Standardized mixed date formats
* Handled missing FRT values
* Corrected inconsistent data types

### Step 2 — KPI Engineering

* Calculated FRT breach flags
* Calculated resolution SLA breaches
* Generated overall SLA compliance indicators
* Created daily and weekly KPI summaries

### Step 3 — Automated Excel Reporting

Generated:

* Raw cleaned dataset
* Daily KPI summaries
* Weekly KPI summaries

### Step 4 — Dashboard Development

Built an interactive Power BI dashboard containing:

* KPI cards
* SLA breach analysis
* Ticket trend analysis
* Escalation breakdown
* Agent performance monitoring
* Category-level ticket insights

---

## 🚀 How to Run

```bash
# Clone repository
git clone https://github.com/PriyaKumari2002/operations-kpi-dashboard.git

# Install dependencies
pip install -r requirements.txt

# Launch notebook
jupyter notebook notebooks/01_cleaning_kpis.ipynb
```

To view the dashboard:
Open `operations_kpi_dashboard.pbix` using Power BI Desktop.

---

## 👤 Author

**Priya Kumari**
Data Analyst | Python • SQL • Power BI • Excel

* GitHub: https://github.com/PriyaKumari2002
* LinkedIn: https://www.linkedin.com/in/priya374/
