# 📊 Excel Salary Intelligence Dashboard

![Salary Dashboard Preview]("/Excel/Images/1_Salary_Dashboard_Final_Dashboard.gif")

## 🚀 Project Overview

This project is an interactive **Excel-based Salary Intelligence Dashboard** built to analyze real-world data science job salaries from 2023.

The objective was simple:

> Transform raw salary data into a dynamic, decision-support tool that helps professionals evaluate compensation trends across roles, countries, and job types.

Instead of static analysis, I designed a dashboard that allows users to filter and explore salary insights based on:

- Job Title  
- Country  
- Job Schedule Type  

This project demonstrates practical data analysis, dashboard design, and advanced Excel functionality.

---

## 🎯 Business Problem

Salary transparency is often fragmented and unclear.

Job seekers frequently struggle to:
- Understand market compensation benchmarks
- Compare salaries across countries
- Evaluate the impact of role seniority and job type

This dashboard provides a structured, interactive solution for answering those questions using real-world data.

---

## 🛠 Technical Skills Demonstrated

### 📉 Data Visualization
- Horizontal Bar Charts
- Geographic Map Charts
- Dynamic Dashboard Layout Design
- Structured Data Sorting & Formatting

### 🧮 Advanced Excel Functions
- `MEDIAN()` with multi-criteria filtering
- Nested `IF()` logic
- `SEARCH()` with conditional matching
- `FILTER()` for dynamic list creation
- Array formulas

### ❎ Data Validation & UX Design
- Dynamic dropdown filtering
- Input control using validated lists
- Error prevention for cleaner analysis
- Improved usability through controlled user interaction

---

## 📊 Dashboard Components

### 1️⃣ Data Science Job Salaries – Median Comparison

<img src="/Excel/Images/1_Salary_Dashboard_Chart1.png" width="850" height="550" alt="Salary Bar Chart">

**Purpose:** Compare median salaries across job roles.

**Why horizontal bar chart?**
- Clear salary comparison
- Better readability for long job titles
- Sorted in descending order for immediate insights

**Key Insight:**
Senior and Engineering roles consistently outperform Analyst-level roles in compensation.

---

### 2️⃣ Global Salary Distribution – Country Map

![Country Salary Map](/Excel/Images/1_Salary_Dashboard_Country_Map.gif)

**Purpose:** Visualize salary disparities across countries.

**Implementation Highlights:**
- Excel Map Chart with median salary aggregation
- Color-coded intensity to reflect compensation levels
- Geographic salary comparison in a single visual

**Key Insight:**
Significant variation exists across regions, reinforcing the importance of geographic positioning in compensation strategy.

---

## 🧠 Core Analytical Logic

### 📌 Multi-Criteria Median Salary Calculation

```excel
=MEDIAN(
IF(
    (jobs[job_title_short]=A2)*
    (jobs[job_country]=country)*
    (ISNUMBER(SEARCH(type,jobs[job_schedule_type])))*
    (jobs[salary_year_avg]<>0),
    jobs[salary_year_avg]
)
)
