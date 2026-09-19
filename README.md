# Global IT Company Analysis — Tableau Dashboard

An interactive Tableau dashboard that profiles **64 global IT companies** across hiring, compensation, work culture, scale and profitability — built to answer questions a student or job-seeker actually asks: *Who hires freshers? Who pays most? Who has the highest attrition? Where are they based?*

> Built with Tableau Desktop 2024.1 (workbook version 18.1). Packaged as `.twbx`, so the data extract ships with the file — no external connection needed.

---

## Preview

<!-- Add a screenshot of the dashboard here, e.g.:
![Dashboard](assets/dashboard.png)
-->

*(Export the dashboard as an image from Tableau → `Worksheet > Export > Image`, save it to `assets/`, and link it above.)*

---

## Dataset

**Source file:** `Sheet1 (IT Companies dataset)` — 64 rows × 20 columns, embedded as a Hyper extract inside the workbook.

| Field | Type | Description |
|---|---|---|
| IT Company | Text | Company name (TCS, Infosys, Accenture, Google, NVIDIA, …) |
| Headquarters | Text | HQ city — Bengaluru, Mumbai, Dublin, Seattle, Tokyo, Paris, etc. |
| Highest Paying Team | Text | Best-paid function (Cloud, AI/ML, Cybersecurity, …) |
| Highest Salary (₹ LPA) | Integer | Top package offered, in lakhs per annum |
| Interview Rounds | Integer | Number of rounds in the hiring process |
| Team with Highest Workload | Text | Function carrying the heaviest load |
| Avg. Working Hours/Day | Integer | Average daily working hours |
| Work Mode | Text | Hybrid / Remote / Onsite |
| Freshers Hiring | Text | Yes / No |
| Annual Hiring | Integer | Headcount hired per year |
| Employee Satisfaction (%) | Integer | Satisfaction score |
| Attrition Rate (%) | Integer | Annual attrition |
| Training Duration (Weeks) | Integer | Onboarding/training length for new joiners |
| Promotion Cycle (Months) | Integer | Typical time to promotion |
| Projects Running | Integer | Active projects |
| Global Offices | Integer | Number of offices worldwide |
| Internship Available | Text | Yes / No |
| Top Skill in Demand | Text | Most in-demand skill at that company |
| Average Annual Profit (USD Billion) | Decimal | Annual profit |
| Founded Year | Integer | Year founded |

---

## What's in the dashboard

One dashboard (`Dashboard 1`, fixed 1500 × 1600) assembled from 12 worksheets, all driven by a single **IT Company** filter so every view updates together.

| View | Type | Shows |
|---|---|---|
| KPI strip | Text tiles | Company count plus totals for hiring, offices, projects, profit, attrition and promotion cycle |
| Profit by company | Bar | Average annual profit (USD Bn) per company |
| Global offices | Bar | Office footprint per company |
| Annual hiring | Bar | Recruitment volume per company |
| Highest salary | Bar | Top package (₹ LPA) per company |
| Salary by team | Donut | Highest salary split across the highest-paying teams |
| Employee satisfaction | Pie ×2 | Satisfaction share across companies |
| Founded year | Line + dot | Company age timeline |
| HQ map | Symbol map | Headquarters plotted by city |
| Hiring detail | Text table | Freshers hiring, internships, top skill, interview rounds, training weeks, promotion cycle, attrition |

---

## How to open it

1. Install **Tableau Desktop** or the free **[Tableau Public](https://www.tableau.com/products/public/download)**.
2. Clone or download this repo.
3. Open `golbal_it_company_analyzes.twbx`.
4. Go to the **Dashboard 1** tab and use the **IT Company** filter to drill into individual companies.

No database setup is required — the `.twbx` is self-contained.

---

## Key questions it answers

- Which companies pay the most, and which team inside them commands that package?
- Who actively hires freshers and offers internships?
- How does attrition track against employee satisfaction and working hours?
- Which skills are most in demand across the industry?
- How is the industry distributed geographically, and how old are the major players?

---

## Repository structure

```
.
├── golbal_it_company_analyzes.twbx   # Packaged Tableau workbook (dashboard + data)
├── data/                             # Raw dataset (optional, if exported to CSV)
├── assets/                           # Dashboard screenshots
└── README.md
```

---

## Tools used

- **Tableau Desktop** — data prep, calculated fields, dashboard design
- **Excel / CSV** — source dataset
- **Tableau Hyper extract** — packaged data storage

---

## Author

**Bloom**

Aspiring Data Analyst — Python · SQL · Power BI · Tableau · Excel

---

## License

Released under the MIT License. The dataset is compiled for educational and portfolio use.
