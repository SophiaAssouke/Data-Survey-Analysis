# Data-Survey-Analysis
# Data Professional Survey Breakdown Dashboard

This repository contains a detailed breakdown of a survey conducted among data professionals across various job types, skillsets, and countries. The dashboard provides insights into job roles, salary distributions, job satisfaction, and the tools and programming languages commonly used by professionals in the data industry.

## Objective

The goal of this dashboard is to:
- Provide insights into salary trends across different job roles.
- Highlight employee satisfaction with work-life balance and salary.
- Examine the most popular tools and programming languages among data professionals.
- Analyze gender-based salary differences to identify any disparities.

---
### Key Technologies Used

1. **Power BI**:
   - Used for creating interactive data visualizations and dashboards.

2. **CSV Data**:
   - Data is in CSV format, allowing for easy use in multiple analysis tools.

3. **DAX Formulas**:
   - Utilized for calculating key metrics such as average salary, satisfaction scores, and gender-based salary differences.


## Methodology

### Data Collection:
The dataset consists of survey responses from data professionals across various countries and job roles. The survey covered topics such as:
- **Job Title** (e.g., Data Scientist, Data Engineer, Data Analyst)
- **Country of Residence**
- **Programming Languages** used in the role (e.g., Python, R, SQL)
- **Job Satisfaction** metrics, including work-life balance and salary satisfaction.
- **Salary Information** (in USD)

### Data Cleaning:
1. **Missing Data**: Rows with missing salary data were excluded from salary-based analysis, while missing data on job satisfaction was handled using median imputation.
2. **Categorization**: Job roles were categorized to simplify the analysis (e.g., "Data Scientist" and "Machine Learning Engineer" were grouped under **Data Scientist**).
3. **Currency Conversion**: If salary data was reported in non-USD currencies, it was converted to USD for consistency.
4. **Outliers**: Salary outliers (extremely high or low) were flagged and removed to avoid skewing the analysis.

### Dashboard Approach:
The dashboard is designed to give decision-makers a comprehensive view of the survey results. The analysis is broken down by:
- **Salary Trends** by job role and gender.
- **Job Satisfaction** scores for work-life balance and salary.
- **Programming Languages** ranked by their popularity.

---

## Key Visualizations and Formulas

### 1. **Country Distribution of Survey Respondents**
   ![Country Distribution](./visuals/country_distribution.png)
   - **Description**: A treemap showing where survey respondents are from.
   - **Formula**: A count of survey takers (`COUNTROWS` in Power BI) grouped by `Country`.


### Key Insights

1. **Salaries**:
   - Data Scientists and Data Architects have the highest average salaries, reflecting the specialized skill sets required for these roles.

2. **Programming Languages**:
   - **Python** is the most popular programming language in the industry, followed by **R** and **SQL**. This highlights the heavy reliance on these languages for data manipulation and machine learning tasks.

3. **Satisfaction Levels**:
   - **Work-Life Balance**: Satisfaction with work-life balance averages at **5.74**, indicating moderate satisfaction in this area.
   - **Salary Satisfaction**: Satisfaction with salary is lower, averaging **4.27**, suggesting that compensation remains a significant concern for many professionals.

4. **Gender Pay Gap**:
   - A slight gender pay gap exists, with male respondents generally earning more than female respondents. This finding underscores the need for ongoing dialogue and initiatives to address pay inequality.
