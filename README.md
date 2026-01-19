# finance_risk_analysis
An end-to-end Financial Risk Management dashboard using MSExcel, SQL and Power BI to analyze 3,500+ corporate entities. Features automated risk scoring, liquidity tracking, and sector-wise solvency analysis.
Finance Risk Analysis Dashboard 📊
Project Overview
This project focuses on identifying and visualizing financial instability within a global portfolio of 3,500+ entities. By analyzing the relationship between assets, liabilities, and market volatility, this dashboard provides a "Risk Pulse" to help financial analysts detect potential insolvency before it occurs.

Technical Workflow
1. Data Processing (Excel & SQL)
Cleaning: Standardized financial columns including Total_Assets, Revenue, and Operating_Income.

Validation: Handled missing values and ensured all monetary values were correctly formatted for cross-sector comparison.

Logic: Established the primary risk metric based on the Financial_Risk_Label to determine the "Market Health Score."

2. Data Modeling & DAX (Power BI)
Custom Measures: Created high-value DAX measures to drive the dashboard's logic:

Burn Rate: Average(Revenue) - Average(Operating_Income)

Risk Score %: DIVIDE(Sum(Risk_Label), Count(Risk_Label))

Leverage Ratio: Total_Liabilities / Total_Assets

Conditional Formatting: Integrated a dynamic alerting system where KPI colors shift (Green 🟢, Amber 🟡, Red 🔴) based on the severity of the financial risk.

Dashboard Features
Top Row: The "Pulse" (KPI Cards)
Total Liquidity: Instant view of available cash/current assets ($174.4B).

Burn Rate: Tracks the velocity of spending across all entities.

Risk Score: A high-level indicator showing that 16.08% of the portfolio is currently flagged as "At Risk."

Leverage: A gauge showing the average Debt-to-Asset ratio (currently 0.49).

Middle Section: Risk Distribution
Sector Risk (Treemap): Visualizes asset concentration. Finance and Healthcare show the largest asset volumes, with colors indicating their respective risk levels.

Risk by Industry (Bar Chart): A direct comparison of which sectors (Energy, Tech, Finance, etc.) are currently the most unstable.

Bottom Section: Deep Dive & Stress Testing
Asset vs. Liability (Column Chart): A side-by-side comparison of solvency per sector.

Sensitivity Analysis: A "What-If" parameter that allows users to simulate how an increase in interest rates would impact the total debt burden.

Key Insights
Critical Sector: The Finance sector holds the highest volume of assets but is currently in an "Amber" state, approaching the 20% high-risk threshold.

Efficiency Gap: Operating expenses across the portfolio account for approximately 82% of revenue, indicating a thin margin for error in operational costs.

Solvency Alert: While total assets are high, the 0.49 leverage ratio suggests that nearly half of the portfolio's assets are funded by debt, making them sensitive to interest rate hikes.
