# 📊 Executive Retail Sales & Workforce Performance Dashboard (Jan–Oct 2026)

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Microsoft Excel](https://img.shields.io/badge/Microsoft%20Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)
![DAX](https://img.shields.io/badge/DAX-Data%20Modeling-0F2744?style=for-the-badge)
![Star Schema](https://img.shields.io/badge/Architecture-Star%20Schema-0F766E?style=for-the-badge)

> **End-to-end commercial and HR payroll analytics solution** reconciling raw Excel records (**1,499 orders** and **365 active + on-leave staff**) into an interactive **Power BI Star Schema** executive report.

![Dashboard Preview](assets/dashboard_preview.png)

---

## 🎯 Project Overview
This project bridges the gap between **retail sales performance** and **branch workforce payroll costs** across 6 branches (*Amman, Irbid, Zarqa, Salt, Madaba, and Aqaba*) from **January to October 2026**. It empowers leadership to evaluate top-line growth, gross margins, target gaps, and data hygiene in a single interactive view.

## 🏗️ Data Architecture & Workflow
1. **Data Reconciliation & Cleaning (Excel):** Audited raw sales and workforce datasets, removed exact duplicates (`INV01400`), isolated salary exceptions, and logged open audit items (`Q001–Q015`).
2. **Data Modeling (Star Schema):** Structured fact tables (`Fact_Sales`, `Fact_Workforce`) linked to conformed dimensions (`Dim_Date`, `Dim_Branches`, `Dim_Products`, `Dim_Employees`).
3. **DAX Measures (`_Measures`):** Built dynamic KPIs for Net Sales, COGS, Gross Profit, Gross Margin %, Average Order Value (AOV), Monthly Active Payroll, and Branch Monthly Actuals vs. Targets.
4. **Interactive Visualization (Power BI):** Designed an executive layout with dynamic dropdown slicers (`Month`, `Branch`, `Category`, `Sales Channel`) and an explicit **Data Governance Disclosure** panel.

## 📈 Key Executive Metrics
* **Total Net Sales:** `461,437.69 JOD` (Gross Sales: `507,932.27 JOD`)
* **Total Cost (COGS):** `322,183.50 JOD` (`69.83%` of Net Sales)
* **Gross Profit & Margin:** `139,199.19 JOD` (`30.17%` Gross Margin)
* **Order Volume & AOV:** `1,499 Orders` | `307.83 JOD` Average Order Value
* **Active Monthly Payroll:** `211,029 JOD` across `365` Active + Leave staff (`25.86%` allocated to branch management)

## 📂 Repository Structure
* `/data` — Reconciled Excel workbook (`Retail_Company_Analytics.xlsx`)
* `/powerbi` — Interactive Power BI report file (`Retail_Company_Analytics.pbix`)
* `/assets` — High-resolution dashboard screenshots
