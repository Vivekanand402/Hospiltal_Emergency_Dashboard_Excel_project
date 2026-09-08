# Hospiltal_Emergency_Dashboard_Excel_project
# 🏥 Hospital Emergency Room Analysis Dashboard

## 📌 Project Overview

The **Hospital Emergency Room Analysis Dashboard** is an end-to-end data analytics project designed to analyze Emergency Room (ER) patient data and provide meaningful insights for better decision-making.

The dashboard helps stakeholders monitor patient volume, waiting time, satisfaction levels, admission status, age distribution, timeliness, gender distribution, and department referrals.

---

## 🎯 Project Objective

The main objective of this project is to:

* Analyze Emergency Room patient data
* Monitor key performance indicators (KPIs)
* Identify patient admission patterns
* Analyze patient waiting time
* Measure patient satisfaction
* Understand patient age and gender distribution
* Track department referrals
* Identify operational trends and areas for improvement

---

## 🛠️ Tools & Technologies

* **Microsoft Excel**
* **Power Query**
* **Power Pivot**
* **DAX**
* **Pivot Tables**
* **Data Visualization**
* **Dashboard & KPI Analysis**

---

## 🔄 Project Workflow

The project follows an end-to-end data analytics workflow:

1. Business Requirement Gathering
2. Understanding of Data
3. Data Connection using Power Query
4. Data Cleaning & Data Quality Check
5. Calendar Table Creation
6. Data Modeling using Power Pivot
7. Creating Required Columns using DAX
8. Pivot Table Creation
9. Dashboard Layout Design
10. Chart Development & Formatting
11. Dashboard / Report Development
12. Insights Generation

---

## 📊 Key KPIs

### 👥 Number of Patients

Measures the total number of patients visiting the Emergency Room each day.

A daily trend is used to identify busy days and patient-volume patterns.

### ⏱️ Average Wait Time

Measures the average time patients wait before being seen by a medical professional.

The trend helps identify days with higher waiting times and potential operational issues.

### ⭐ Patient Satisfaction Score

Measures the average patient satisfaction score to evaluate service quality.

The trend can help identify changes in satisfaction and their relationship with patient volume and waiting time.

---

## 📈 Dashboard Analysis

The dashboard includes the following analysis:

### 1. Patient Admission Status

Shows the number of patients who were:

* Admitted
* Not Admitted

### 2. Patient Age Distribution

Patients are grouped into different age categories:

* 0–4
* 05–14
* 15–29
* 30–44
* 45–59
* 60–69
* 70–79

### 3. Timeliness Analysis

Measures the percentage of patients who were seen within **30 minutes**.

Patients are classified as:

* **Within Time**
* **Delay**

### 4. Gender Analysis

Displays the number of patients by gender.

### 5. Department Referrals

Identifies which departments receive the highest number of patient referrals.

---

## 🧮 DAX Calculations

### Age Group

```DAX
=IF([Patient Age]>=70,"70-79",
IF([Patient Age]>=60,"60-69",
IF([Patient Age]>=45,"45-59",
IF([Patient Age]>=30,"30-44",
IF([Patient Age]>=15,"15-29",
IF([Patient Age]>=5,"05-14","0-4"))))))
```

### Patient Attend Status

```DAX
=IF([Patient Waittime]<30,"Within Time","Delay")
```

---

## 📅 Calendar Table

A calendar table was created using Power Query for date-based analysis and trend reporting.

```Power Query
= List.Dates(
    #date(2023,01,01),
    731,
    #duration(1,0,0,0)
)
```

---

## 📊 Dashboard Features

The final dashboard provides a centralized view of Emergency Room performance and includes:

* KPI cards
* Patient trends
* Admission analysis
* Age distribution
* Gender analysis
* Waiting-time analysis
* Department referral analysis
* Patient satisfaction trends
* Interactive Pivot-based analysis

---

## 💡 Business Insights

The dashboard can help hospital stakeholders:

* Monitor Emergency Room workload
* Identify high patient-volume periods
* Track waiting-time performance
* Evaluate patient satisfaction
* Understand patient demographics
* Monitor admission patterns
* Identify departments receiving more referrals
* Support data-driven operational decisions

---

## 📁 Project Structure

```text
Hospital-Emergency-Room-Analysis/
│
├── Hospital Emergency Room Analysis.xlsx
├── README.md
└── Dashboard/
    └── Final Dashboard Screenshot.png
```

---

## 🚀 Skills Demonstrated

* Data Cleaning
* Data Transformation
* Data Modeling
* Power Query
* Power Pivot
* DAX
* KPI Development
* Pivot Tables
* Dashboard Design
* Data Visualization
* Business Intelligence
* Business Requirement Analysis
* Data-Driven Insights

---

## 👨‍💻 Author

**Vivekanand Dubey**

**Aspiring Data Analyst | Excel | SQL | Power BI | Python**

---

⭐ If you find this project useful, consider giving the repository a star!
