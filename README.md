# 📊 Atlas Lab HR Analytics Dashboard

An interactive Business Intelligence and HR analytics solution designed to monitor core workforce metrics, evaluate department performance, analyze employee demographics, and investigate attrition trends.

---

## 🚀 Dashboard Overview
<img width="725" height="351" alt="Screenshot 1" src="https://github.com/user-attachments/assets/4100dc9a-2040-466e-9629-5b9404eca68b" />
<img width="722" height="350" alt="Screenshot 2" src="https://github.com/user-attachments/assets/9a18ace8-550d-4ebf-8765-1e284e413ff5" />
<img width="721" height="350" alt="Screenshot 3" src="https://github.com/user-attachments/assets/58b1f4b5-0b38-4694-8e38-8e336214eda4" />
<img width="722" height="349" alt="Screenshot 4" src="https://github.com/user-attachments/assets/d1df335f-4f36-4381-9f52-8b02dd1f8fd8" />

---

## 🚀 Project Overview
Managing human resources efficiently requires deep visibility into employee lifecycles, satisfaction, and retention. The **Atlas Lab Dashboard** provides comprehensive visual insights across four main modules:
1. **Overview:** High-level executive summary tracking total headcounts, inactive employees, hiring trends, and active distributions by department[cite: 1, 2].
2. **Demographics:** Detailed breakdowns of workforce diversity, age distribution, marital status, and average salary by ethnicity[cite: 2].
3. **Performance Tracker:** Individual and aggregate performance ratings, job satisfaction levels, work-life balance, and environment scores[cite: 4].
4. **Attrition:** Deep-dive analysis into employee turnover rates categorized by department, travel frequency, hire date, and years spent at the company[cite: 4].

---

## 🧮 Used Measures & Calculated Metrics
To power the dynamic filtering, headcount evaluations, and performance calculations across the Atlas Lab dashboard, a dedicated _Measures table was implemented using Data Analysis Expressions (DAX).

**1. Headcount & Attrition KPIs**
Total Employees
Computes the total historical and current workforce count based on unique employee identifiers.

Active Employees
Filters the workforce baseline to isolate active personnel currently employed by the organization.

Inactive Employees
Isolates employees who have separated from the company (attrition status marked as 'Yes').

Attrition Rate (%)
Calculates the overall organizational or segment-level turnover proportion relative to total headcount.

**2. Compensation & Workforce Analytics**
Average Salary
Calculates the mean compensation value across ethnic groups.

Years at Company (Tenure)
Evaluates the active lifecycle duration of employees from their hire date to the current date or termination period.

**3. Advanced Performance & Relationship Modeling**
Satisfaction & Rating Measures (Context Transition)
Measures evaluating performance dimensions (such as Job Satisfaction, Environment Satisfaction, Work-Life Balance, and Manager Ratings) utilize expanded relationships and context transitions via USERELATIONSHIP to connect active fact tables with date or rating dimension models seamlessly.

---

## 🛠️ Key Process & Workflow

### **1. Data Preparation & Cleaning**
* Aggregated raw organizational datasets containing employee records (active and inactive status, hire dates, departments, job roles, and compensation).
* Standardized demographic features including age groups, gender categories, marital status, and ethnic groups[cite: 2].
* Engineered key metrics such as **Attrition Rate** (overall ~16%) and **Years at Company**[cite: 1, 4].

### **2. Dashboard Modules & Visual Implementation**
* **Overview:** Displays total active employees (1,233), inactive employees (237), hiring trends from 2012 to 2022, and active headcounts by department/job role (e.g., Software Engineers, Data Scientists)[cite: 1].
* **Demographics:** Visualizes employee age brackets (highest concentration in ages 20–38), marital status breakdown (Married: 42%, Single: 37%, Divorced: 20%), and salary correlations across ethnic backgrounds[cite: 2].
* **Performance Tracker:** Maps evaluation metrics across job satisfaction, relationship satisfaction, manager ratings, and work-life balance against standardized performance rating levels[cite: 4].
* **Attrition Analysis:** Examines turnover hotspots—highlighting higher attrition in Sales (21%) and Human Resources (19%), tenure risk windows (highest turnover within the first 0–1 years), and travel frequency impacts[cite: 4].

---

## 📊 Key Insights & Findings
* **Turnover Peak:** Attrition peaks heavily during the first year of employment (32–34%), signaling a need to improve onboarding and early-stage employee engagement[cite: 4].
* **Department Breakdown:** Technology maintains the largest workforce share (828 active employees) with a lower attrition rate (14%) compared to Sales (21%)[cite: 1, 4].
* **Demographic Distribution:** Youngest employee recorded is 18 and the oldest is 51, with the dominant age demographic falling between 20 and 39 years old[cite: 2].

---

