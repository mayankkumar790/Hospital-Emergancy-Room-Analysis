# 🏥 Hospital Emergency Room Analysis

## 📊 Project Overview
This Excel-based data analysis project explores **Hospital Emergency Room performance** to identify patterns in patient admissions, waiting times, age distribution, gender, and departmental referrals.

The analysis helps hospital management understand operational efficiency, patient demographics, and areas that need improvement.

---

## 🧾 Objectives
- Analyze **Patient Admission Status** (Admitted vs. Not Admitted)
- Study **Age Distribution** of patients
- Measure **Timeliness** — percentage of patients seen within 30 minutes
- Compare **Gender Distribution** among patients
- Identify top **Department Referrals**

---

## 🧹 Data Cleaning Process
Two datasets were used in this project:

- 🧱 **Uncleaned Dataset**: [View on Google Drive](https://drive.google.com/file/d/1ghIowsfFSsAsio02dCrFnC4lr4r5gsEI/view?usp=sharing)
- ✨ **Cleaned Dataset**: [View on Google Sheets](https://docs.google.com/spreadsheets/d/1Np6--T_7RQPk_us6DCXYLTU-MC5ThgcA/edit?usp=sharing&ouid=114879746492443693925&rtpof=true&sd=true)

### Cleaning Steps:
1. Removed duplicate and missing values  
2. Corrected inconsistent data (e.g., gender and department names)  
3. Converted date/time fields into proper Excel date formats  
4. Created helper columns for time difference (waiting time)  
5. Created calculated columns using DAX and Excel formulas

---

## 🧮 DAX & Excel Formulas Used
#### 👶 Age Group Calculation
=IF([Patient Age]>70,"70-79",
IF([Patient Age]>60,"60-69",
IF([Patient Age]>50,"50-59",
IF([Patient Age]>40,"40-49",
IF([Patient Age]>30,"30-39",
IF([Patient Age]>20,"20-29",
IF([Patient Age]>10,"10-19","0-9")))))))

#### ⏱️ Patient Attend Status
=IF([Patient Waittime]>30,"Delay","Ontime")

### 📆 Calendar Table Formula
= List.Dates(#date(2023,01,01), 731, #duration(1,0,0,0))

## 📈 Dashboard Insights

#### Key Visuals:
- Patient Admission Status – Admitted vs. Not Admitted
- Patient Age Distribution – Age groups 0–79
-Timeliness – % of patients seen within 30 minutes
-Gender Analysis – Male vs. Female patients
-Department Referrals – Top referred departments

#### KPI Metrics:
-Total Number of Patients
-Daily Average Wait Time
-Daily Patient Satisfaction Score

## 🧰 Tools & Skills Used:
-Microsoft Excel / Power Query / Power Pivot
-Data Cleaning & Transformation
-Pivot Tables and Dashboards
-DAX Formulas
-Data Visualization

## 📅 Project Author:
-👨‍💻 Mayank Kumar
-📧 Email: mayankkumar21july@gmail.com

## 🏁 Conclusion:
-The Hospital Emergency Room Analysis Dashboard provides clear insights into patient flow and operational efficiency.
It can help healthcare administrators identify bottlenecks and improve emergency response performance.

## 🖼️ Dashboard Preview:
![Dashboard Screenshot](<img width="887" height="395" alt="Dashboard" src="https://github.com/user-attachments/assets/8a8afbc1-b113-4cf7-976c-398afd4c3684" />
)
