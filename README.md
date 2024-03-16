# HR-ANALYTICS-REPORT
---

**Documentation Outlines**

- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Tools Used](#tools-used)
- [Data Cleaning](#data-cleaning)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Analysis](#data-analysis)
- [Results](#results)
- [Recommendations](#recommendations)

## Project Overview
---
This HR Analytics project aims to examine the factors influencing employee attrition within the organization over the past years. Through a comprehensive analysis of various   parameters in the provided data, our objective is to gain valuable insights that will inform strategic decisions. This process will enable us to construct compelling narratives around our data findings and identify the key contributors to employee retention or turnover. By understanding the factors driving attrition, we can implement targeted measures to enhance employee engagement and foster a positive work environment, ultimately reducing the organization's attrition rate.

## Data Sources
---
The primary dataset used for this analysis is the "hr_data.xlsx" file, containing comprehensive information about each employee in the organization. The HR dataset contains key attributes related to employee profiles, job details, performance, and satisfaction metrics. Analyzing these attributes will help identify attrition drivers and develop strategies for improving employee retention. Some of the key attributes includes:

- **Attrition:** This column indicates whether an employee has left the company or not.
- **CF_age band:** This column categorizes employees into age bands.
- **Department:** This column represents the department in which an employee works.
- **Education Field:** This column indicates the field of study of an employee.
- **Gender:** This column represents the gender of an employee.
- **Job Role:** This column indicates the job role of an employee within the organization.
- **Marital Status:** This column represents the marital status of an employee (e.g., Single, Married, Divorced).
- **CF_current Employee:** This column indicate whether an employee is currently employed or not (1 = Yes, 0 = No).
- **Education:** This column represents the highest level of education attained by an employee.
- **Employee Count:** This column represent the total number of employees.
- **Job Satisfaction:** This column represents an employee's overall satisfaction with their job or role.
- **Years At Company:** This column indicates the number of years an employee has been working at the company.

## Tools Used
---
- Microsoft Excel (For Data Cleaning) 
- Microsoft Power BI (For Reporting and Dashboarding)

## Data Cleaning
---
In the initial data preparation phase, the following tasks were performed:
- Data Loading and Inspection.
- Handling Duplicate Data.
- Handling Missing Data.
- Data Formatting.
- Feature Selection/Engineering.

## Exploratory Data Analysis 
---
EDA entails delving into the data to address various questions regarding its characteristics, which includes:
- Which gender had a higher count of attritions?
- What education field had the highest attrition counts?
- Which marital status category had the highest count of attritions?
- Which department had the highest count of attritions?
- Which age group had the highest attrition counts?
- Which education level had the highest attrition counts? 

## Data Analysis
---
Here is where I incorporated certain Data Analysis Expressions (DAX) utilized during my analysis.
```
Attrition Rate = sum('HR data'[Attrition Count]) / SUM('HR data'[Employee Count])
```
```
Average Years = AVERAGE('HR data'[Years At Company])
```
```
Rating = REPT("⭐", 'HR data'[Job Satisfaction])
```
```
Retained Employee = sum('HR data'[Employee Count]) - sum('HR data'[Attrition Count])
```

## Results 
---
This is where the insights obtained from the analysis are presented. "Access my insights here:[[Dashboard Report Link](https://app.powerbi.com/view?r=eyJrIjoiNWFmMDk4MTgtMGU2Yi00M2IwLTgyMWMtNWE5M2MxOWMzY2I4IiwidCI6IjBlZjcwYWU3LWI3NmUtNGI4ZC04NWEzLWZlZmFmNjg4MDAxZCJ9)]"
- The attrition count for males, at 150, exceeded that of females, which stood at 87.
- With a total attrition count of 89, Life Sciences recorded the highest figure, surpassing Human Resources by 82 counts, as it had the lowest attrition count at 7.
- Single had the highest sum of attrition count, reaching 120, followed by Married at 84, and Divorced at 33
- R&D recorded the highest sum of attrition count at 133, trailed by Sales at 92, and HR at 12.
- With a total attrition count of 112, the age group (25-34) had the highest sum, surpassing the age group (Over 55) by 101 counts, as it had the lowest attrition count at 11.
- With a total attrition count of 99, Bachelor's Degree had the highest sum, surpassing Doctoral Degree by 94 counts, as it had the lowest attrition count at 5.

## Recommendations
---
Based on the analysis, i recommend the following actions:
- Focus on improving retention strategies specifically for male employees.
- Investigate and address issues causing high attrition in the Life Sciences education field and R&D department.
- Provide better support and incentives for single employees and those in the 25-34 age group to encourage them to stay.
- Review and enhance career growth opportunities, compensation, and work-life balance for employees with Bachelor's degrees.
- Gather feedback from exiting employees to understand and resolve the root causes of attrition.
- Benchmark against companies with lower attrition rates and implement industry best practices.
- Foster a more inclusive and supportive company culture to improve overall employee retention.
