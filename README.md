# ai-driven-sales-opportunity-analysis
Power BI project for sales opportunity analysis, key influencers, anomaly detection, and KPI reporting


# AI-Driven Sales Opportunity Analysis in Power BI

## Overview

This project is a Power BI business intelligence solution designed to analyze sales opportunity performance and explain key drivers behind win/loss outcomes. It combines standard BI reporting with AI-powered visuals to support decision-making around opportunity conversion, revenue trends, pipeline behavior, and anomaly detection.

The report is built to answer practical business questions such as:

- Which factors are associated with opportunities being won or lost?
- Which product categories perform better in terms of close rate?
- Which products generate the highest won revenue?
- Are there unusual changes in revenue over time?
- How do managers and product categories compare across performance views?

This project was developed as a portfolio case to demonstrate business-focused reporting, data modeling, KPI design, and the use of advanced Power BI visuals.

---

## Business Objective

The goal of this project is to transform sales opportunity data into a decision-ready analytical experience that helps users:

- monitor revenue performance
- understand win/loss patterns
- identify influential business factors
- detect unusual revenue behavior over time
- compare results across product and management dimensions

The report is designed for business users, analysts, and hiring managers who want to evaluate both technical execution and business thinking.

---

## Project Scope

This solution focuses on five main analytical areas:

1. **Opportunity performance**
2. **Win/Loss analysis**
3. **Revenue trend monitoring**
4. **AI-supported explanation of outcomes**
5. **Manager and product comparison**

---

## Tools and Technologies

- **Power BI Desktop**
- **Power BI Service**
- **Power Query**
- **DAX**
- **Data Modeling**
- **AI Visuals in Power BI**
  - Key Influencers
  - Decomposition Tree
  - Anomaly Detection
  - Smart Narrative
  - Q&A

---

## Data Model

The model follows a business intelligence structure with fact and dimension tables.

### Core fact tables
- **Opportunities**
- **Cases**

### Core dimensions
- **Accounts**
- **Products**
- **Campaigns**
- **Owners**
- **Industries**
- **Opportunity Calendar**
- **Case Calendar**

### Modeling approach
- one-to-many relationships from dimensions to facts
- dedicated calendar tables
- hidden technical key columns for cleaner report consumption
- measures organized in a dedicated `_Measures` table

---

## Key KPIs

The report includes core business measures such as:

- Opportunity Count
- Won Opportunity Count
- Lost Opportunity Count
- Closed Opportunity Count
- Total Opportunity Value
- Revenue Won
- Revenue Lost
- Revenue Open
- Weighted Pipeline
- Revenue per Opportunity
- Average Opportunity Value
- Close %
- Win Rate
- Lost Rate
- Average Discount
- Avg Days to Close

---

## Report Pages

### 1. Key Influencers
Analyzes which factors are associated with opportunities being won or lost.

Main elements:
- Close % by Product Category
- Revenue Won by Product
- Key Influencers visual
- interaction-driven filtering between visuals

### 2. Decomposition Tree
Allows interactive breakdown of performance by dimensions such as:
- Manager
- Product Category
- Campaign
- Industry
- Purchase Process

### 3. Anomaly Detection
Explores revenue trends over time and highlights unusual points in the time series.

Main elements:
- Revenue Won Over Time
- anomaly detection with expected range
- monthly and recent-period analysis
- small multiples by manager and product category
- smart narrative summary

### 4. KPI Test / Model Test
Validation pages used to confirm:
- measure behavior
- relationship integrity
- slicer interaction
- category-level breakdown

---

## AI Features Used

This project includes several Power BI AI capabilities:

### Key Influencers
Used to identify which business attributes are associated with `Status = Won` or `Status = Lost`.

### Anomaly Detection
Used to identify unexpected changes in revenue over time and compare actual values against expected ranges.

### Decomposition Tree
Used to support guided exploration of KPI changes across business dimensions.

### Smart Narrative
Used to generate an executive-style summary of report insights.

### Q&A
Used to test natural-language querying of the semantic model.

---

## Data Preparation Highlights

Key data preparation activities included:

- data profiling
- type correction
- duplicate checks on business keys
- text standardization
- date conversion and calendar preparation
- relationship validation
- hiding technical columns
- measure formatting and KPI documentation

---

## Design Principles

This report was built with the following principles in mind:

- clear business questions
- readable layout
- simple but meaningful KPI structure
- interaction testing before final design
- separation between technical fields and user-facing fields
- portfolio-ready presentation quality

---

## Example Business Insights Supported by the Report

The report structure is designed to surface insights such as:

- product categories with higher or lower close rates
- managers associated with stronger revenue outcomes
- campaigns linked to better conversion performance
- purchase processes associated with win/loss outcomes
- unusual revenue spikes or drops over time

---

## How to Use the Report

1. Open the report in Power BI Desktop or Power BI Service.
2. Start with the **Key Influencers** page for high-level business explanation.
3. Use the **Decomposition Tree** for guided breakdown analysis.
4. Review the **Anomaly Detection** page for revenue trend behavior.
5. Use slicers and interactions to explore category-, manager-, and time-based changes.
6. Use Q&A for quick natural-language testing of the model.

---
## Screenshots

### Key Influencers
![Key Influencers](screenshots/key-influencers-1.png)
![Key Influencers](screenshots/key-influencers-2.png)
![Key Influencers](screenshots/key-influencers-3.png)

### Decomposition Tree
![Decomposition Tree](screenshots/decomposition-tree-1.png)

### Anomaly Detection
![Anomaly Detection](screenshots/anomaly-detection-1.png)


---

## Notes

- This project was developed for portfolio and demonstration purposes.
- AI visuals in Power BI may behave differently depending on filters, data distribution, and model structure.
- Q&A quality depends on semantic model clarity and field naming quality.

---

## Author

**Amir Hossein Bagheri**  
Business Intelligence Analyst | Power BI | Microsoft Fabric | SQL | Data Modeling

## Repository Contents

structure Amir's Repository:

```text
/
├── README.md
├── report/
│   └── [project-file].pbix
├── screenshots/
│   ├── key-influencers1.png
│   ├── decomposition-tree1.png
│   ├── anomaly-detection1.png
│   
├── docs/
│   ├── kpi-dictionary.pdf
│   └── project-summary.pdf
