# Attrition Analysis

A Power BI dashboard that analyzes employee attrition using the classic HR Employee Attrition dataset. The report breaks down *who* is leaving, *where* in the organization, and *why* — surfacing the key drivers behind attrition so HR/business teams can act on them.

## 📊 Report Overview

The `.pbix` file contains a multi-page interactive report:

| Page | What it shows |
|---|---|
| **Home** | Landing page with navigation buttons to every report page |
| **Employee Details** | Headcount KPIs and demographic breakdowns (gender, marital status, education field, job role) via bar, pie, and line charts |
| **Department** | Attrition funnel and breakdown by department, business travel, and job level |
| **Salary Analysis** | Monthly income analysis by job role/level, income bands, and a pivot table view |
| **EDA** | Exploratory analysis — attrition rate gauge, training times, work-life balance, and cross-tab pivot tables |
| **Key Influencers** | Power BI's Key Influencers visual, identifying the strongest drivers of attrition |

## 🧮 Data Model

Built on a single table, **`HR_Employee_Attrition_Data`**, with fields including:

- **Demographics:** Age (and age bins), Gender, Marital Status, Education, Education Field
- **Job info:** Department, Job Role, Job Level, Business Travel, Overtime
- **Compensation:** Monthly Income (and income bins), Hourly Rate
- **Tenure & development:** Years at Company, Training Times Last Year
- **Satisfaction:** Job Satisfaction, Work-Life Balance
- **Target:** Attrition (Yes/No), plus a derived **Attrition Rate** measure

Key DAX measures include `Attrition_Rate` and `Total_count`, used across cards, gauges, and charts to summarize headcount and turnover at a glance.

## 🔍 Key Questions the Report Answers

- What is the overall attrition rate, and how does it trend across departments?
- Which departments, job roles, or job levels have the highest turnover?
- Does overtime, business travel, or work-life balance correlate with attrition?
- How does monthly income relate to attrition risk?
- What are the top statistical drivers of attrition (via Key Influencers)?

## 🛠️ Tools Used

- **Power BI Desktop** — data modeling, DAX measures, and report visuals

## 🚀 Getting Started

1. Clone this repo:
```bash
   git clone https://github.com/abhisekuma/Attrition-Analysis.git
```
2. Open `Attrition_analysis.pbix` in [Power BI Desktop](https://www.microsoft.com/en-us/download/details.aspx?id=58494).
3. Use the navigation buttons on the **Home** page to explore each section of the report.

## 📁 Files

- `Attrition_analysis.pbix` — the full Power BI report (data model + visuals)
- `README.md` — this file

## 📌 Notes

- All charts are interactive — click on any bar, slice, or slicer to cross-filter the rest of the page.
- The **Key Influencers** page uses Power BI's built-in AI visual and may take a moment to recalculate when filters change.
