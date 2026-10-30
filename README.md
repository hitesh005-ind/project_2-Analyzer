# project_2-Analyzer
📌 Project Overview & Objectives

The Analyzer project processes granular transaction data across multiple retail categories and regional channels. It converts transactional datasets into an actionable decision-support model designed for executive overview and strategy formulation.

Key Focus Areas:

Statistical Diagnostics: Calculate measures of central tendency and dispersion metrics using Data Analysis Toolpak functions.



Sensitivity Analysis: Construct dynamic What-If scenarios measuring the impact of varying discount rates (0% to 20%) on net revenue and margins.

Automated Customer Rank Lookup: Dynamically extract top spenders using dynamic array lookup combinations (INDEX, MATCH, LARGE).

Growth Indicators: Monitor Month-over-Month (MoM) sales velocity using custom directional arrow formatting.

2. Descriptive Statistics Summary

Statistical Metric

Calculated Value

Mean (Average Sales)

₹24,195.00

Median

₹17,100.00

Standard Deviation

₹20,183.12

Sample Variance

407,358,394.74

Minimum / Maximum

₹2,200.00 / ₹93,280.00

Range

₹91,080.00

3. Dynamic High-Value Spender Lookup

Automated top-customer extraction without manual sorting or VBA:

=INDEX('Sales Data'!G4:G23, MATCH(LARGE('Sales Data'!K4:K23, 1), 'Sales Data'!K4:K23, 0))


4. What-If Discount Sensitivity Matrix

Using dynamic SUMPRODUCT logic across discount intervals (0%, 5%, 8%, 10%, 12%, 15%, 20%):

project - 2 analyzer (hitesh).xlsx
│
├── 📊 Executive Dashboard
│   ├── KPI Cards (Total Sales, Total Profit, Total Orders, AOV)
│   ├── Top 10 High-Value Spenders Dynamic Ranking Table
│   ├── Data Storytelling & Strategic Recommendations Text Box
│   ├── Line Chart: Monthly Sales Growth Trend
│   └── Pie Chart: Category Revenue Share %
│
├── 📜 Sales Data
│   ├── Dynamic Header Timestamp (=NOW())
│   ├── Full Transaction Log with Unit Cost & Profit Margin Formulas
│   └── Soft Green Color Scale Conditional Formatting on Total Purchases
│
├── 🧪 What-If & Growth Analysis
│   ├── Discount Sensitivity Matrix (0% - 20% Discount Scenarios)
│   └── MoM Monthly Sales Growth Table with Custom Trend Indicators (▲ UP / ▼ DOWN)
│
├── 📐 Analysis Toolpak & Stats
│   ├── Complete Descriptive Statistics Output Table
│   └── OLS Linear Regression Summary Output (ANOVA, Coefficients, Intercept)
│
└── 📊 Pivot Table & Charts
    ├── Cross-Tabulated Pivot Table (Region vs. Product Category Sales)
    └── Clustered Bar Chart: Regional Category Breakdown
