# HR-ANLAYSTIC# Human Resources Analytics Dashboard – README

## Project Overview

The **Human Resources Analytics Dashboard** is an interactive Power BI dashboard designed to analyze workforce data, employee distribution, departmental headcount, gender diversity, and organizational structure. The dashboard helps HR teams monitor employee statistics and make data-driven workforce decisions. 

---

# Dashboard Objectives

This dashboard is built to:

* Monitor employee headcount
* Analyze workforce distribution by department and group
* Track gender diversity
* Review monthly employee trends
* Filter employees by year, quarter, gender, and confirmation status
* Improve HR reporting and workforce planning

---

# Key Metrics

## Total Employee Headcount

* **18 Employees**

## Gender Distribution

* Female: 9 Employees (50%)
* Male: 9 Employees (50%)

The dashboard provides equal gender representation insights within the organization. 

---

# Dashboard Visualizations

## 1. Gender Distribution

Donut chart displaying employee count by gender.

### Categories

* Female (F)
* Male (M)

### Purpose

* Analyze workplace diversity
* Monitor gender balance

---

## 2. Headcount by Group

Bar chart representing employee count across different organizational groups.

### Groups Included

* 5
* 6
* 7
* F
* G
* L
* 10
* 8
* 9
* J
* K
* Part Time

### Purpose

* Compare workforce allocation across groups
* Identify departments with larger staffing

---

## 3. Monthly Headcount

Scatter/line chart showing employee headcount by month.

### Example

* June Headcount: 18

### Purpose

* Track monthly workforce trends
* Monitor hiring and attrition patterns

---

## 4. Headcount by Function

Horizontal bar chart analyzing employee count by business function.

### Functions Included

* Administration
* Finance
* First Choice
* General Management
* Human Resources
* Information Systems
* Marketing
* Commercial
* Customer Service
* Operations
* Procurement

### Purpose

* Analyze staffing by department
* Support workforce planning

---

# Filters & Slicers

The dashboard includes interactive slicers for:

* Month
* Quarter
* Gender
* Year
* Group
* Confirmed Status

### Confirmed Status Options

* Y (Confirmed)
* N (Not Confirmed)

These slicers allow dynamic filtering and detailed HR analysis.

---

# Dashboard Design

## Theme

The dashboard uses a clean professional HR design with:

* Beige background theme
* Yellow and black highlight colors
* Human resource icons
* Structured corporate layout

## UI Features

* Interactive filtering
* Professional HR styling
* Responsive chart arrangement
* Easy-to-read KPI visuals

---

# Tools & Technologies Used

* Power BI Desktop
* DAX Measures
* Power Query
* Data Modeling
* Interactive Charts & Slicers

---

# Suggested DAX Measures

## Total Headcount

```DAX
Total Headcount = COUNT(Employee[EmpID])
```

## Female Employees

```DAX
Female Employees =
CALCULATE(
    COUNT(Employee[EmpID]),
    Employee[Gender] = "F"
)
```

## Male Employees

```DAX
Male Employees =
CALCULATE(
    COUNT(Employee[EmpID]),
    Employee[Gender] = "M"
)
```

## Monthly Headcount

```DAX
Monthly Headcount =
COUNT(Employee[EmpID])
```

---

# Business Insights

* The organization currently maintains balanced gender diversity.
* Some groups and functions contain higher employee concentration.
* Administration, Finance, HR, and Marketing departments have stronger representation.
* Monthly headcount monitoring helps identify workforce stability.
* HR teams can use confirmation status filters for employee tracking.

---

# Future Improvements

Possible enhancements include:

* Employee attrition analysis
* Hiring trend forecasting
* Salary and compensation analytics
* Attendance and leave tracking
* Performance evaluation metrics
* Employee age and experience analysis
* Department-wise KPI tracking

---

# Dataset Fields Used

The dashboard uses HR-related fields such as:

* Employee ID
* Gender
* Group
* Function
* Month
* Quarter
* Year
* Confirmation Status

---

# Conclusion

The **Human Resources Analytics Dashboard** provides a centralized HR reporting solution for workforce analysis and employee monitoring. It combines interactive visuals, KPI tracking, and dynamic filtering to support better HR decision-making and organizational planning. 
