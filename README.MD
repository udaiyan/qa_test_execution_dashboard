# QA Test Execution Power BI Dashboard

## Overview

This Power BI dashboard demonstrates the ability to **develop data dashboards and data visualisations to support decision-making** by translating complex, raw operational data into clear, actionable intelligence for senior stakeholders.

The dashboard simulates a QA/Testing environment, allowing management to track quality gate pass rates, automation coverage, and module-specific defect severity. It is designed to support **operational decision-making in a fast-changing environment**, with a focus on **data quality, scalability, and reproducibility**.

---

## Objective

To demonstrate the ability to develop a data dashboard that translates complex, raw operational data into clear, actionable intelligence for senior decision-makers. This dashboard simulates a QA environment, allowing management to track quality gate pass rates, automation coverage, and module-specific defect severity.

![Screenshot](screenshot.png)

---

## Key Features

### Executive KPIs
Real-time calculation of overall pass rate and automation coverage to support strategic planning. These high-level metrics provide management with an immediate snapshot of quality and efficiency.

### Trend Analysis
Time-series line charts to identify if code stability is improving or degrading over sprints. This enables proactive intervention before issues escalate.

### Root Cause Identification
Stacked bar charts by module to pinpoint where critical defects are concentrated, enabling targeted resource allocation and informed decision-making.

### Interactive Filtering
Slicers for Environment (Staging, UAT, Production) and Modules to support operational decision-making in fast-changing environments. Stakeholders can drill down into specific areas of interest.

---

## Skills Demonstrated

| Skill | How It Is Demonstrated |
|-------|------------------------|
| **Data Transformation** | Importing and cleaning raw CSV data using Power Query, ensuring data integrity and consistency |
| **DAX Measure Creation** | Building complex business logic for KPIs, including pass rates, automation coverage, and average execution times |
| **Visual Design Principles** | Creating a clean, management-focused layout that prioritises clarity and actionable insights |
| **Translating Technical Data** | Converting raw test statuses and execution times into understandable management-level formats (rates, trends, ratios) |
| **Data Validation** | Ensuring data accuracy through careful type checking and validation during the transformation phase |

---

## Dataset

The dashboard uses a dummy dataset (`QA_Test_Execution_Data.csv`) containing simulated QA test execution data. The dataset includes:

| Field | Description |
|-------|-------------|
| `Date` | Date of test execution |
| `Module` | System module being tested (e.g., User Login, Payment Gateway) |
| `TestSuite` | Logical grouping of test cases |
| `TestCaseID` | Unique test case identifier |
| `Status` | Test result (Pass, Fail, Blocked) |
| `DefectSeverity` | Severity of any defect found (Critical, High, Medium, Low) |
| `TestType` | Automated or Manual |
| `Environment` | Deployment environment (Staging, UAT, Production) |
| `ExecutionTimeSeconds` | Duration of test execution |

---

## How to Use

### Prerequisites
- [Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/) (free version)

### Instructions
1. Clone this repository or download the `.pbix` and `.csv` files
2. Open the `.pbix` file in Power BI Desktop
3. Ensure the data source path points to the `QA_Test_Execution_Data.csv` file
4. Refresh the data if needed
5. Use the slicers to filter by Module or Environment
6. Hover over visuals to see detailed tooltips

### Interactive Features
- **Module Slicer** – Filter by specific system modules
- **Environment Slicer** – Filter by deployment environment
- **Cross-filtering** – Click on any visual to filter other visuals on the page

---

## Project Structure

```text
qa-test-execution-dashboard/
├── QA_Test_Execution_Dashboard.pbix    # Power BI report
├── QA_Test_Execution_Data.csv          # Dummy dataset
├── README.md                           # Project documentation
└── screenshot.png                      # Dashboard preview
```


---


---

## Future Enhancements

Potential improvements if this were a production dashboard:

- **RLS (Row-Level Security)** – Restrict access based on user role
- **Data Refresh Automation** – Connect to a live database or API
- **Alerts** – Email notifications when pass rate drops below threshold
- **Historical Comparison** – Year-on-year or sprint-on-sprint comparison
- **Export Functionality** – One-click export to PDF/Excel for stakeholders

---

## About the Author

This dashboard was created by **Dr. Darren Udaiyan** as part of a portfolio demonstrating data analytics skills.

- **GitHub:** [github.com/udaiyan](https://github.com/udaiyan)
- **ResearchGate:** [researchgate.net/scientific-contributions/33793758_D_Udaiyan](https://www.researchgate.net/scientific-contributions/33793758_D_Udaiyan)
- **US Patent:** [US8024705](https://patents.google.com/patent/US8024705)

---

## License

This project is for demonstration purposes only. The dataset contains purely synthetic data and is not derived from any real patient, healthcare, or production information.

---

*Last updated: September 2026*