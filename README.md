## 🏗️ Construction Project Analysis & Reporting Automation

This project delivers an end-to-end solution for cleaning, analyzing, and reporting construction project data using Python. It transforms raw, inconsistent records into business-ready insights covering material costs, labour utilization, monthly trends, and project status.


## 🔍 Scope of Work

### Data Cleaning & Preparation

- Standardized inconsistent column headers using a dynamic loop

- Removed duplicate entries based on Project ID and Report Date

- Treated missing values in Material_Cost and Labor_Hours with column averages

- Converted dates and percentage progress to correct types

- Standardized inconsistent text formats in Project_Status

- Built a reusable outlier-checking function  to detect anomaly using IQR method and visualized via boxplots


### Data Analysis

- Identified sites with the highest and lowest average material costs

- Measured correlation between Labor_Hours and Project_Progress, highlighting negative efficiency trends

- Tracked monthly totals for material cost and labour hours

- Counted projects by status (e.g. Completed, In Progress, Delayed)

- Estimated total project cost using a proxy rate derived from average cost and labour efficiency

- Flagged top 5 and bottom 5 most expensive projects


### Automated Reporting

All results are exported to a multi-sheet Excel report using XlsxWriter, including:

- Cleaned dataset

- Monthly material and labour trends

- Project status breakdown

- Cost efficiency rankings


## Use Case:

Stakeholders can use this automated report to track resource usage, compare cost performance across project sites, and prioritise investigation into underperforming or overbudget projects. It supports better planning, reporting accuracy, and operational efficiency in future construction cycles.

## 🧰 Tools Used

      - Python 3.x
      - pandas
      - matplotlib
      - seaborn
      - XlsxWriter (Excel export engine)
