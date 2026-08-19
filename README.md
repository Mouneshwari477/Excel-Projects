# 📊 E-Commerce Sales & Analysis Dashboard
This project is an interactive Excel-based analytics dashboard designed to analyze key performance metrics of an e-commerce business. It provides a complete overview of Sales, Profit, Orders, Quantity, Profit Margin, and enables deep-dive analysis across categories, sub-categories, states, and customer segments.

The dashboard also includes YoY (Year-over-Year) growth indicators, helping measure performance improvements at a glance.

### 🚀 Key Features
### ✅ 1. KPI Summary Cards

Total Sales

Total Profit

Total Quantity Sold

Number of Orders

Overall Profit Margin

Year-over-Year Growth (%) for each KPI

These indicators instantly highlight business performance trends.

### ✅ 2. Monthly Sales & Profit Trend

A combined line & column chart showing:

Monthly Sales

Monthly Profit
This visual helps identify seasonal patterns, growth spikes, and low-performing months.

### ✅ 3. Category-wise Profit Analysis

A bar chart breaking down profit by:

Technology

Office Supplies

Furniture
Useful for understanding which areas drive or drain profitability.

### ✅ 4. Category-wise Sales % (Donut Chart)

A clean visualization of the sales contribution of each category, helping stakeholders track market mix and category dominance.

### ✅ 5. State-wise Sales Map

A geographic heat map showing sales performance across various states, enabling region-wise business planning and expansion strategy.

### ✅ 6. Top 5 Sub-Categories by Sales

Displays the highest revenue-generating sub-categories (e.g., Phones, Chairs), helping identify focus areas for marketing and inventory planning.

### ✅ 7. Fully Interactive Filters

Users can slice and explore data using:

Year

Region

Segment (Consumer, Corporate, Home Office)
These filters update all visuals dynamically.

### 🧰 Tools & Techniques Used

Microsoft Excel

Pivot Tables & Pivot Charts

Conditional Formatting

Map Chart Visualization

Slicers for Interactive Filters

### 🎯 Dashboard Insights (High-Level)

Sales show a strong upward trend with ~20% YoY growth.

Profit also increased ~14%, but profit margin decreased slightly, indicating discount/margin pressure.

Phones and Chairs dominate top sub-category sales.

Western and Central states contribute the highest revenue.

Office Supplies and Furniture categories show varying profit performance.

# Grocery-Inventory-Management-Excel-Dashboard
Dynamic Excel dashboard for grocery sales performance, using Power Query and PivotTables to transform raw data into actionable insights for optimizing sales and inventory.

# Data Description
This dataset provides detailed information on various grocery items, including product details, supplier information, stock levels, reorder data, pricing, and sales performance. The data covers 990 products across various categories such as Grains & Pulses, Beverages, Fruits & Vegetables, and more.

# Data Cleaning and Preprocessing 📊
During this project, rigorous data cleaning and preprocessing steps were undertaken to ensure the dataset's integrity and prepare it for robust analysis:

Data Transformation: The raw .csv dataset was transformed into a usable Excel format using Power Query, maintaining data integrity throughout the process.

Missing Value Imputation: Missing values in the 'Category' column were appropriately filled based on relevant product items to ensure comprehensive and robust analysis.

Data Type Formatting: All datatypes were meticulously checked and accurately formatted according to their variable descriptions, preventing inconsistencies in analysis.

Feature Engineering - Sales Revenue: An essential 'Sales Revenue' column was created by calculating Sales_Volume * Unit_Price, providing a key metric for financial analysis.

Categorical Feature Creation - Turnover Segment: A 'Turnover_Segment' was defined based on the 'Inventory_Turnover_Rate' to categorize products, facilitating segmented analysis:
High: > 60
Medium: 20-60
Low: 0-20

# Dashboard Creation
All visuals and KPIs were dynamically created using PivotTables and PivotCharts for Summary Statistics and to visualize the trends, with strategic use of Slicers for interactive exploration.

# Key Performance Indicators (KPIs) Insights 📈
Analysis of the key performance indicators reveals crucial insights into operational efficiency and sales performance:

Total Sales Revenue: Achieved 344,269.3 in total income from all product sales for the period 2024-25, highlighting overall financial performance.

Total Sales Volume: Recorded 58,336 units, providing a clear understanding of the sheer volume of goods moved.

Average Sales Volume Per Product Sold: An average of 58.925 units per product establishes a baseline for individual product performance. Products significantly exceeding this warrant attention as exceptional performers, while those falling below may require re-evaluation.

Zero Stock Products: Currently, none of the products are completely out of stock, effectively preventing lost sales and enhancing customer satisfaction.

Stock-to-Sales Ratio: A value of 0.9437 indicates efficient inventory management, where for every 1 unit of sales volume, approximately 0.9437 units are held in stock. This suggests the company is effectively meeting demand without significant overstocking or stockouts.

# Visual Interpretation & Core Findings 📊
Visualizations were instrumental in uncovering patterns and relationships within the data:

Product Categories Dominance: "Fruits and Vegetables" combined with "Dairy" constitute over 50% of the total sales volume, indicating these categories are primary revenue drivers.

Price-Volume Correlation: No significant correlation was observed between 'Unit Price' and 'Sales Volume', suggesting pricing isn't the sole driver of sales quantity. The scatter plot also revealed outliers, indicating unique product performances that warrant deeper investigation.

Sales vs. Revenue Divergence: The 'Top 10 products by Sales Volume' differ from the 'Top 10 products by Sales Revenue', primarily indicating that the products generating the most money are not necessarily the same as the products selling the most units.

Turnover Segment Performance: Products categorized as 'High Turnover' (selling fastest) generate the most sales volume. 'Medium Turnover' products contribute a respectable amount, while 'Low Turnover' products generate the least sales volume, aligning inventory speed with sales contribution.

# Implications 🚀
Prioritize Star Performers (Fruits & Vegetables, Dairy): Focus rigorously on ensuring consistent availability, optimal freshness, and competitive pricing for 'Fruits & Vegetables' and 'Dairy' categories. Any disruption in these areas could significantly impact overall revenue, as they constitute over 50% of total sales volume.

Segment-Specific Pricing Strategies: Develop and implement more granular, segment-specific pricing strategies. The observed outliers in 'Unit Price' vs. 'Sales Volume' suggest unique product behaviors that warrant deeper investigation and tailored pricing approaches.

Optimize Inventory for Volume vs. Profit Drivers:
Volume Drivers: Ensure these products are consistently well-stocked to maintain customer traffic and overall sales volume.
Profit Drivers: Optimize merchandising and pricing strategies for products that generate the most revenue (profit drivers) to maximize financial returns, even if they don't sell in the highest volume.

# Automated MIS Reporting & KPI Dashboard

## 📌 Overview
An end-to-end Excel-based MIS (Management Information System) dashboard that consolidates sales, employee, branch, and product data into a single automated reporting system — complete with data validation checks, dynamic pivot-style summaries, interactive filters, and a one-click VBA refresh macro.

## 🎯 Problem Statement
Sales operations teams often struggle to consolidate data scattered across multiple sources (raw transactions, employee records, branch/product masters, targets) into a single, reliable, decision-ready report. This project builds a fully formula-driven MIS dashboard that automatically merges, validates, and summarizes this data — eliminating manual reconciliation and reducing reporting errors.

## 🗂️ Data Structure
The workbook is built on a relational, multi-sheet structure:
| Sheet | Purpose |
|---|---|
| `Sales_Data` | Raw transactional records (date, branch, employee, product, qty, revenue, target) — 1,000 rows |
| `Employee_Master` | Employee ID, name, department, manager, region |
| `Branch_Master` | Branch, city, state mapping |
| `Product_Master` | Product code, category, price |
| `Targets` | Monthly revenue targets per branch |
| `Merged_Data` | Consolidated table joining all sources via INDEX-MATCH lookups |
| `Data_Quality_Checks` | Automated validation checks on the raw data |
| `Dashboard` | Final KPI summary, pivot-style tables, and visual report |
| `Filters` / `FilterLists` | Dropdown-based filtered view (slicer substitute) |
| `Macro_RefreshDashboard` | VBA macro documentation and button |

## 🔧 Approach
1. **Data Consolidation** – Used `INDEX-MATCH` (wrapped in `IFERROR`) to enrich every raw sales transaction with employee, branch, product, and target details into a single `Merged_Data` table — the single source of truth for the dashboard.
2. **Data Quality Checks** – Built automated validation formulas using `SUMPRODUCT`, `COUNTIF`, and `COUNTBLANK` to flag duplicate employee IDs, blank revenue entries, and invalid product codes before they reach the report.
3. **KPI Calculation** – Computed core metrics (Total Revenue, Total Orders, Average Order Value, Target Achievement %) using `SUM`, `COUNTA`, `AVERAGE`, and `ROUND`.
4. **Pivot-Style Summaries** – Built dynamic breakdowns by Month, Branch, Region, Department, Product Category, and Top 10 Employees using `SUMIF`, `INDEX`, `MATCH`, and `LARGE` — replicating pivot table functionality with live formulas.
5. **MoM Growth Tracking** – Calculated month-over-month revenue growth % using `=(Current - Previous)/Previous`.
6. **Interactive Filtering** – Implemented dropdown-based filters (Branch, Department, Month, Region) as a slicer substitute using Data Validation lists.
7. **Automation via VBA** – Added a `RefreshDashboard` macro (triggered by a button) that recalculates all formulas and resets filters to "(All)" with a single click.

## 🛠️ Tech Stack
- **Tool:** Microsoft Excel (Macro-Enabled Workbook, `.xlsm`)
- **Formulas:** INDEX-MATCH, SUMIF, SUMPRODUCT, COUNTIF, COUNTA, COUNTBLANK, LARGE, IFERROR, TEXT, ROUND
- **Automation:** VBA (macro-based dashboard refresh)
- **Techniques:** Data Validation, Data Quality Auditing, MIS Reporting, KPI Tracking, MoM Growth Analysis

## 📈 Key Features
- **Live, formula-driven dashboard** — no static/pasted values; every KPI recalculates automatically as source data changes
- **Built-in data quality layer** — flags duplicate records, blank fields, and invalid references before they affect reporting
- **Multi-dimensional breakdowns** — revenue by month, branch, region, department, product category, and top-performing employees
- **One-click refresh** — VBA macro recalculates all formulas and resets filters instantly

## 🚀 How to Run
1. Download `mis_kpi_dashboard.xlsm` and open in Excel (enable macros when prompted)
2. Review raw data in `Sales_Data`, `Employee_Master`, `Branch_Master`, `Product_Master`, `Targets`
3. View the consolidated dataset in `Merged_Data` and validation results in `Data_Quality_Checks`
4. Open the `Dashboard` tab to view KPIs and pivot-style summaries
5. Use the `Filters` tab to filter the view, or click **"Refresh Dashboard"** to recalculate everything and reset filters.
