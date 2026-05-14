# 📊 Customer Support Operations KPI Dashboard

> An end-to-end automated reporting pipeline that transforms raw support ticket data into actionable business insights using Python, Excel, and Power BI.

---

## 🧩 Problem Statement

Customer support teams generate hundreds of tickets daily. Without proper tracking, SLA breaches go unnoticed, escalations are mismanaged, and agent performance is invisible to management.

This project builds an **automated KPI reporting system** that ingests raw ticket data, cleans it, calculates business-critical metrics, and delivers a fully interactive Power BI dashboard — the kind of system real operations teams use daily.

---

## 🎯 KPIs Tracked

| KPI | Description |
|-----|-------------|
| **First Response Time (FRT)** | Time between ticket creation and first agent response |
| **Resolution Time** | Total time to resolve a ticket |
| **SLA Breach Rate** | % of tickets that exceeded SLA limits by priority |
| **Escalation Analysis** | Volume and type of escalations (Customer/Internal/Manager) |
| **Agent Performance** | Per-agent ticket volume, FRT, and resolution time |
| **Reopened Tickets** | Tickets reopened after being marked resolved |

---

## 🔍 Key Insights

- **38% SLA Breach Rate** — 190 out of 500 tickets breached SLA limits
- **Medium priority** tickets had the highest breach volume despite longer SLA limits
- **Critical tickets** showed fastest resolution but highest escalation rate
- **Agent_Kumar** handled the highest ticket volume with above-average resolution time
- **Manager escalations** were the most common escalation type — signaling potential first-line resolution gaps

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| **Python** | Data cleaning, KPI calculation, visualization |
| **Pandas** | Data manipulation and aggregation |
| **Matplotlib / Seaborn** | Exploratory charts |
| **OpenPyXL** | Excel report generation |
| **Power BI** | Interactive dashboard |

---

## 📁 Project Structure

```
operations-kpi-dashboard/
│
├── data/
│   └── support_tickets_raw.csv       # Raw messy ticket data (520 rows, 16 cols)
│
├── notebooks/
│   └── 01_cleaning_kpis.ipynb        # Full pipeline: clean → calculate → export
│
├── output/
│   └── kpi_report.xlsx               # Excel report (3 sheets: Raw, Daily, Weekly)
│
├── dashboard/
│   └── operations_kpi_dashboard.pbix # Interactive Power BI dashboard
│
├── requirements.txt
└── README.md
```

---

## ⚙️ Pipeline Overview

```
Raw CSV → Data Cleaning → KPI Calculation → Excel Export → Power BI Dashboard
```

**Step 1 — Data Cleaning**
- Removed 20 duplicate rows
- Standardized 3 mixed date formats to datetime64
- Handled 67 null FRT values
- Fixed column data types

**Step 2 — KPI Calculation**
- Calculated FRT breach flag vs SLA limit by priority
- Calculated resolution breach flag
- Combined into overall SLA breach flag
- Aggregated daily and weekly KPI summaries

**Step 3 — Excel Export**
- Raw_Data sheet — cleaned full dataset
- Daily_KPIs sheet — day-level aggregations
- Weekly_KPIs sheet — week-level aggregations

**Step 4 — Power BI Dashboard**
- 4 KPI cards (Total Tickets, Avg FRT, Avg Resolution, SLA Breaches)
- Breaches by Priority bar chart
- Monthly Ticket Trend line chart
- Tickets by Category pie chart
- Escalation Breakdown bar chart
- Agent Performance table

---

## 🚀 How to Run

```bash
# Clone the repo
git clone https://github.com/PriyaKumari2002/operations-kpi-dashboard.git

# Install dependencies
pip install -r requirements.txt

# Run the notebook
jupyter notebook notebooks/01_cleaning_kpis.ipynb
```

To view the dashboard — open `dashboard/operations_kpi_dashboard.pbix` in **Power BI Desktop** (free download from microsoft.com/powerbi)

---

## 👤 Author

**Priya**  
Data Analyst | Python • SQL • Power BI • Excel  
[LinkedIn](https://linkedin.com/in/yourprofile) • [GitHub](https://github.com/yourusername)
