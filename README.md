# K-J Stores: Sales and Profitability Analysis Dashboard

An interactive Excel dashboard that analyzes two years of sales, profit, cost, and quantity data for a retail electronics and accessories business. It answers specific questions about when, where, and what sells, and whether higher sales translate into higher profit.

> **Data note:** The dataset is synthetic. It was generated for this portfolio project and does not represent a real business.

**Download the workbook:** [K-J Srores.xlsm](workbook/K-J%20Srores.xlsm)

---

## Project Overview

K-J Stores sells electronics and accessories across four regions. This project analyzes performance across 2023 and 2024 to answer one question: where is the business making money, and what changed between the two years?

The workbook contains four sheets:

| Sheet | Purpose |
|---|---|
| **Dataset** | Underlying synthetic sales records |
| **Pivot Tables** | Supporting summaries used by the dashboards |
| **Dashboard 1: Time Series Analysis** | Monthly and weekday sales and profit trends |
| **Dashboard 2: Product & Regional Analysis** | Sales and profit by region and product |

---

## Business Problem

Sales totals alone do not show whether a business is healthy. A month or product can generate high revenue and still contribute little profit. Management needs to see:

- Which periods, regions, and products drive revenue
- Which of them also drive profit
- How performance changed from 2023 to 2024

---

## Project Objectives

1. Summarize overall performance using sales, profit, cost, and quantity.
2. Compare 2023 and 2024 performance at the KPI level.
3. Identify high-performing months and weekdays for both sales and profit.
4. Compare regional and product performance.
5. Test whether sales leaders are also profit leaders.
6. Present findings in a format that does not require the reader to interpret each chart from scratch.

---

## Tools and Technologies

- **Microsoft Excel** (macro-enabled workbook, `.xlsm`)
- **PivotTables** for aggregating and summarizing data
- **Excel formulas** for KPI values and year-over-year percentage changes
- **Dynamic chart titles** built with formulas
- **Slicers** for filtering by product category and region
- **VBA** for the navigation system

---

## Dashboard Features

### Dashboard 1: Time Series Analysis

![K-J Srores Time series Analysis](screenshots/K-J%20Srores%20Time%20series%20Analysis.png)

- **KPI row:** Combined sales, profit, cost, and quantity for 2023 and 2024, with 2024 vs. 2023 percentage changes
- **Weekday sales trend:** Monday to Sunday sales, 2023 vs. 2024
- **Weekday profit trend:** Monday to Sunday profit, 2023 vs. 2024
- **Monthly sales trend:** January to December sales, 2023 vs. 2024
- **Monthly profit trend:** January to December profit, 2023 vs. 2024

### Dashboard 2: Product & Regional Analysis

![K-J Srores Product & Regional Analysis](screenshots/K-J%20Srores%20Product%20%26%20Regional%20Analysis.png)

- **KPI row:** Same four KPIs as Dashboard 1
- **Sales by region:** South, East, West, and North, 2023 vs. 2024
- **Profit by region:** South, East, West, and North, 2023 vs. 2024
- **Sales by product:** Monitor, Mouse, Headphones, Laptop, Printer, and Keyboard, 2023 vs. 2024
- **Profit by product:** Same six products, 2023 vs. 2024

---

## Interactive Capabilities

**Slicers.** Both dashboards include slicers for:
- Product category: Accessories, Electronics
- Region: East, North, South, West

**Dynamic chart titles.** Chart titles are formula-driven and update when a slicer selection changes. Instead of generic labels such as "Sales by Region," each title states the leading result, for example "South Led Overall Sales with $270.4K, 44.2% above North $187.5K Sales."

**VBA navigation.** Sidebar icons take the user to any of the four sheets: Time Series Analysis, Product & Regional Analysis, Calculations (PivotTables), and Dataset. A single reusable macro handles all four icons.

**Color encoding.** 2023 appears in a faded red and 2024 in a bright red across all charts. The donut charts in the KPI row follow the same encoding: the faded arc is 2023 and the bright arc is 2024. Hovering over any chart shows its values.

---

## Analytical Questions

1. How much revenue and profit did the business generate across both years?
2. How did sales, profit, cost, and quantity change from 2023 to 2024?
3. Did profit grow at the same rate as sales?
4. Which months generated the highest sales and the highest profit?
5. Which weekdays generated the strongest sales and profit?
6. Do high-sales months also produce high-profit months?
7. Which region leads in sales and profit?
8. Which products lead in cumulative sales and profit?
9. How do sales leaders compare with profit leaders?
10. How do Accessories and Electronics compare when filtered?

---

## Key Business Insights

### Overall performance
- Combined sales were **$862.1K** and combined profit was **$737.8K** across 2023 and 2024.
- Combined cost was **$124.3K** and combined quantity sold was **1,678** units.
- In 2024 compared with 2023, sales rose **35.8%**, profit rose **39.5%**, cost rose **16.0%**, and quantity rose **31.8%**.
- Profit grew faster than sales, and cost grew more slowly than both. The data shows this pattern but does not explain its cause.

### Time patterns
- **Weekday:** Saturday was the peak day in 2024 for both sales and profit. Saturday's 2024 sales were **18.5%** higher than Friday's 2023 peak, and Saturday's 2024 profit was **19.4%** higher than Friday's 2023 peak.
- **Monthly:** September was the peak month in 2024 for both sales and profit. September 2024 sales were **12.5%** higher than March 2023 sales, the 2023 peak. September 2024 profit was **13.1%** higher than the March 2023 profit peak.

### Regional performance
- **South** led both sales and profit. Its sales of **$270.4K** were **44.2%** above North's **$187.5K**, the lowest region.
- South's profit of **$233.0K** was **47.0%** above North's **$158.5K**.

### Product performance
- **Headphones** led both cumulative sales (**$170.6K**) and cumulative profit (**$147.0K**).
- Headphones' sales were **53.1%** above Printer's **$111.4K**, the lowest-selling product.
- Headphones' profit was **56.0%** above Printer's **$94.2K**.
- **Monitor** and **Mouse** grew sharply from 2023 to 2024 in both sales and profit.
- **Keyboard** declined in 2024 in both sales and profit.

---

## Business Recommendations

1. **Prioritize South for inventory and staffing.** South leads in both sales and profit by a wide margin. Allocating stock and sales effort there protects the strongest revenue base.

2. **Keep Headphones well stocked and visible.** Headphones lead in cumulative sum (2023 + 2024) for both sales and profit. Avoid stockouts and feature them in regional promotions.

3. **Review the Keyboard range.** Keyboard was the only product in this view to decline in both sales and profit in 2024. Review its pricing, placement, and competition before the next buying cycle.

4. **Plan Saturday staffing and promotions.** Saturday led both sales and profit in 2024. Schedule peak staffing and time-limited offers for Saturdays.

5. **Prepare inventory and marketing ahead of September.** September led in both sales and profit in 2024. Build stock and campaigns in August to meet demand.

6. **Track the cost-to-profit relationship each quarter.** In 2024, profit rose 39.5% while cost rose 16.0%. Monitor this gap so cost growth does not catch up with revenue growth.

7. **Use Monitor and Mouse growth as a model.** Both products grew sharply in 2024. Identify what changed in their pricing, placement, or promotion and apply the same approach to other products.

---

## Dashboard Screenshots

### Dashboard 1: Time Series Analysis
![K-J Srores Time series Analysis](screenshots/K-J%20Srores%20Time%20series%20Analysis.png)

### Dashboard 2: Product & Regional Analysis
![K-J Srores Product & Regional Analysis](screenshots/K-J%20Srores%20Product%20%26%20Regional%20Analysis.png)

### Pivot Tables
![K-J Srores Pivot Tables](screenshots/K-J%20Srores%20Pivot%20Tables.png)

### Dataset
![K-J Srores Dataset](screenshots/K-J%20Srores%20Dataset.png)

---

## Project Structure

```
kj-stores-sales-profitability-dashboard/
├── README.md
├── workbook/
│   └── K-J Srores.xlsm
└── screenshots/
    ├── K-J Srores Time series Analysis.png
    ├── K-J Srores Product & Regional Analysis.png
    ├── K-J Srores Pivot Tables.png
    └── K-J Srores Dataset.png
```

The dataset lives on the Dataset sheet inside `K-J Srores.xlsm`, so no separate data file is needed.

---

## How to Use the Workbook

1. Download [K-J Srores.xlsm](workbook/K-J%20Srores.xlsm) and open it in Microsoft Excel.
2. Enable macros so the navigation icons work.
3. Use the sidebar icons to move between sheets.
4. Click a slicer (Accessories, Electronics, East, North, South, or West) to filter the dashboard. Chart titles and values update automatically.
5. Hold Ctrl and click slicer buttons to select more than one option.
6. Use the Pivot Tables sheet to see the summaries behind each chart.

---

## Technical Implementation

- **Data:** Synthetic sales records covering 2023 and 2024, stored on the Dataset sheet.
- **Summaries:** PivotTables on the Pivot Tables sheet aggregate sales, profit, cost, and quantity by month, weekday, region, and product.
- **KPIs:** Combined totals and year-over-year percentage changes are calculated with formulas.
- **Dynamic titles:** Formula-driven chart titles read from the summaries and update with slicer selections.
- **Slicers:** Connected to the dashboard charts to filter by category and region.
- **Navigation:** A reusable VBA macro is assigned to the four sidebar icons.
- **File format:** Macro-enabled workbook (`.xlsm`).

---

## Limitations

- The dataset is synthetic, so findings describe the sample, not a real business.
- Two years of data are enough to compare years but not to establish seasonal patterns with confidence.
- The analysis shows relationships between sales, profit, and cost. It does not identify their causes.

---

*Author: Obiekwe Emmanuel C. (Business Analyst with Strong Data Analysis Skills)*
