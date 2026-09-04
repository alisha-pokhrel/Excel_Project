# 📊 Data Science Salary Calculator

An interactive Excel dashboard designed to explore and compare data science salaries across different job titles, countries, job types, and platforms.

## 📌 Project Overview

This project analyzes data science job and salary information to help users understand salary differences across roles, locations, and employment types.

The dashboard allows users to interact with the data using filters and quickly compare salary trends through charts, a geographic visualization, and key performance indicators (KPIs).

## 🎯 Objectives

- Analyze salary differences across data science job titles.
- Compare salaries across different countries.
- Understand salary variations by job type.
- Identify the median salary for the selected criteria.
- Identify the platform with the highest number of relevant job postings.
- Provide an interactive and easy-to-understand salary analysis dashboard.

## 📊 Dashboard Preview

![Salary Dashboard](https://github.com/user-attachments/assets/c204e919-bb0b-4eac-89b0-e3fc120d3711)

## 📊 Excel Skills Used
The following Excel skills were utilized for analysis:
- 📉 **Charts**
- 🧮 **Formulas and Functions**
- 🔽 **Data Validation**

## 📊 Data Science Jobs Dataset

The dataset used for this project contains information about data science jobs and salaries. It provides the data needed to analyze salary trends across different roles, locations, and job types.

It includes detailed information on:

- 👨‍💼 **Job Titles**
- 💰 **Salaries**
- 📍 **Locations**
- 💼 **Job Types**
- 🌐 **Job Platforms**

## 📊 Dashboard Build

### 📉 Charts

#### 📊 Data Science Job Salaries – Bar Chart

![Job_Title](https://github.com/user-attachments/assets/a745c221-fadd-452c-914c-44c211302599)


- 🧮 **Excel Features:** Used a horizontal bar chart with formatted salary values for clear comparison.
- 🎨 **Design Choice:** A horizontal bar chart makes it easy to compare median salaries across different job titles.
- 📋 **Data Organization:** Job titles are sorted by median salary in descending order for better readability.
- 💡 **Insights Gained:** The chart makes it easy to identify higher-paying roles and compare salary differences across positions.

#### 🌍 Country Median Salaries – Map Chart

![Country](https://github.com/user-attachments/assets/444f05cb-46a6-4efe-a67a-d006a83ee4af)


- 🗺️ **Excel Features:** Used an Excel Map Chart to visualize median salaries across different countries.
- 🎨 **Design Choice:** A map provides a quick geographic view of salary differences between locations.
- 📋 **Data Organization:** Country and median salary data were organized to allow Excel to identify and visualize each location.
- 💡 **Insights Gained:** The map helps identify countries with relatively higher or lower median salaries.

#### 💼 Salary by Job Type

![Job_type](https://github.com/user-attachments/assets/6419e3c3-99af-41fd-9023-724fa7e4d089)


- 📊 **Excel Features:** Used a chart to compare median salaries across different job types.
- 🎨 **Design Choice:** Visual comparison makes salary differences between employment types easier to understand.
- 💡 **Insights Gained:** The chart helps identify salary patterns across different job types.

## 🧮 Formulas and Functions

### 💰 Median Salary by Job Title

```
  =MEDIAN(
IF(
(DATA!$A$2:$A$32673=JOB_TITLE!$A5)*
(DATA!$M$2:$M$32673<>"")*
(DATA!$K$2:$K$32673=COUNTRY)*
(ISNUMBER(SEARCH(TYPE,DATA!$E$2:$E$32673))),DATA!$M$2:$M$32673))
```
The dashboard uses Excel formulas to calculate median salaries based on selected job titles, countries, and job types.


- 🔎 **Multi-Criteria Filtering:** Filters salary data based on job title, country, and job type.
- 🧮 **Median Calculation:** Uses the `MEDIAN()` function to calculate the median salary from the filtered data.
- 🎯 **Conditional Logic:** Uses `IF()` to apply multiple conditions and exclude invalid or blank salary values.
- 📊 **Dynamic Analysis:** The formulas update the salary results based on the selected dashboard filters.

#### Background Table
![Median](https://github.com/user-attachments/assets/65d638e3-679d-4504-8817-b1c34e72f68a)

#### Dashboard Implementation

![job_title_median](https://github.com/user-attachments/assets/44bb24e3-3824-4d82-98db-e4127abe0d34)

### 📝 Conclusion

This project demonstrates how Excel can be used to analyze and visualize data science job and salary data effectively. The interactive dashboard makes it easy to compare salaries across job titles, countries, and job types. It also strengthened my skills in Excel formulas, data visualization, and dashboard design.
