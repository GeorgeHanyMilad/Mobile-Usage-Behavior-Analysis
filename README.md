<p align="center">
  <img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExcXFycDVxenZqaDl4enRkNzIzMTdjZXJnenVkcXc2OGF3azlyMXR1NCZlcD12MV9zdGlja2Vyc19zZWFyY2gmY3Q9cw/8f3nS1Gajtv70qNicE/giphy.gif" width="200px" height="200px">
</p>

# 📱 Mobile Usage Behavior Analysis (Excel Dashboard Project)

<p align="center">
  <img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExcXFycDVxenZqaDl4enRkNzIzMTdjZXJnenVkcXc2OGF3azlyMXR1NCZlcD12MV9zdGlja2Vyc19zZWFyY2gmY3Q9cw/8f3nS1Gajtv70qNicE/giphy.gif" alt="Project Preview" width="200px" height="200px">
</p>

---

## 📌 Table of Contents
- [📖 Project Overview](#-project-overview)
- [📊 Dataset](#-dataset)
- [🛠️ Data Preparation & Transformation](#️-data-preparation--transformation)
- [🧮 Pivot Tables](#-pivot-tables)
- [📈 Dashboard](#-dashboard)
- [🔍 Insights](#-insights)
- [💡 Possible Reasons](#-possible-reasons)
- [✅ Recommendations](#-recommendations)
- [🧰 Tools & Technologies](#-tools--technologies)
- [🙌 Acknowledgments](#-acknowledgments)

---

## 📖 Project Overview
This project focuses on analyzing **mobile usage behavior** using **Excel only**.  
The main goal is to study **user behavior**, identify **potential signs of mobile addiction**, and explore how **age and gender** affect:
- Mobile screen time
- Data usage
- Number of installed applications
- App usage patterns

The output is an **interactive dashboard** that helps decision-makers understand trends and take action.

---

## 📊 Dataset
- **Source:** [Kaggle - Mobile Device Usage and User Behavior Dataset](https://www.kaggle.com/datasets/valakhorasani/mobile-device-usage-and-user-behavior-dataset)  
- **Size:** 700 rows × 11 columns  
- **Format:** CSV file  

### 📑 Columns Description
| Column | Description |
|--------|-------------|
| User ID | Unique identifier for each user |
| Device Model | Model of the smartphone |
| Operating System | OS of the device (iOS / Android) |
| App Usage Time (min/day) | Daily app usage in minutes |
| Screen On Time (hours/day) | Average screen time per day |
| Battery Drain (mAh/day) | Daily battery consumption |
| Number of Apps Installed | Total installed apps |
| Data Usage (MB/day) | Daily data consumption |
| Age | Age of the user |
| Gender | Male / Female |
| User Behavior Class | Classification of user usage behavior (1–5) |

---

## 🛠️ Data Preparation & Transformation
Performed in **Power Query**:
1. **Data Cleaning**  
   - No missing values  
   - No duplicates  
   - No outliers (validated using Box Plot)

2. **Transformations**  
   - Converted `User ID` & `User Behavior Class` to *Text*  
   - Created **Age Groups** instead of raw ages  
   - Replaced numeric **Behavior Classes (1–5)** with labels:  
     - `1 → Uses Rarely`  
     - `2 → Uses Sometimes`  
     - `3 → Uses Normally`  
     - `4 → Uses Often`  
     - `5 → Uses Always`  
   - Converted `App Usage Time` from minutes → hours

📷 Power Query Preview: *(ضع لينك الصورة)*

---

## 🧮 Pivot Tables
The analysis is powered by **Pivot Tables**, which summarize and structure the dataset before visualization.  

📷 Pivot Table Previews:  

<div align="center">

**Pivot Table 1** – App Usage by Age Group  
<img src="ضع_لينك_الصورة_الأولى" alt="Pivot Table 1" width="80%"/>

**Pivot Table 2** – Screen Time & Data Usage by Gender  
<img src="ضع_لينك_الصورة_الثانية" alt="Pivot Table 2" width="80%"/>

**Pivot Table 3** – Apps Installed vs App Usage  
<img src="ضع_لينك_الصورة_الثالثة" alt="Pivot Table 3" width="80%"/>

</div>

> All slicers are connected to these Pivot Tables using **Report Connections** for a fully synchronized experience.

---

## 📈 Dashboard
The interactive dashboard was built using **Pivot Tables, Charts, KPIs, and Slicers**.  
All slicers are connected via **Report Connections** for a fully dynamic experience.  

📷 Dashboard Preview: *(ضع لينك الصورة)*  

### 🔑 KPIs:
- **Users:** 700  
- **Avg App Usage (Hr):** 4.5  
- **Avg Screen Time (Hr):** 5.3  
- **Avg Data Usage (MB):** 929.7  
- **Avg Apps Installed:** 51  

### 📊 Charts:
1. App Usage (Hr) by Age  
2. Screen Time (Hr) by Age  
3. Data Usage (MB) by Age & Gender  
4. App Usage (Hr) vs Data Usage (MB)  
5. Apps Installed vs App Usage (Hr)  
6. App Usage (Hr) by Gender  

### 🎛️ Slicers:
- Gender  
- Age  
- User Behavior Class  

---

## 🔍 Insights
- **18–25** spend the most time on apps (avg. 4.8 hrs/day)  
- **18–25** install the most apps (avg. 54 apps)  
- **46–59** have the highest screen time (avg. 5.5 hrs/day)  
- **36–45** show the lowest usage in all metrics  
- Highest data consumption is among **46–59** (avg. 1022.4 MB for males, 929.2 MB for females)  
- **Males vs Females:** Nearly identical app usage (~4.5 hrs/day)  
- **Positive correlations:**  
  - App Usage ⬆️ → Data Usage ⬆️  
  - Apps Installed ⬆️ → App Usage ⬆️  

---

## 💡 Possible Reasons
- **36–45:** Busy with work/family → lower usage  
- **18–25:** Curious, more free time → higher usage & app installs  
- **46–59:** Depend heavily on phones for news & entertainment → high data & screen time  
- **Gender similarity:** Social apps (WhatsApp, Instagram, TikTok) used equally by both  
- **Correlations:** More apps = more time, more time = higher data usage  

---

## ✅ Recommendations
- Raise awareness among **18–25** on time management  
- Encourage **46–59** to use data-saving tools  
- Run awareness campaigns on **TikTok, Instagram, Facebook** for 18–25 age group  
- Motivate **26–35** to balance entertainment with educational/utility apps  
- Introduce **in-app notifications** reminding users to take breaks after 3 hours  

---

## 🧰 Tools & Technologies
- **Microsoft Excel**: Data Analysis, Pivot Tables, Charts, Slicers  
- **Power Query**: Data Cleaning & Transformation  
- **Box Plot**: Outlier detection  

---

## 🙌 Acknowledgments
- Dataset provided by [Kaggle](https://www.kaggle.com/datasets/valakhorasani/mobile-device-usage-and-user-behavior-dataset)  
- Project developed as part of **Data Analysis practice using Excel**  

---
🚀 *Crafted with passion for Data Analytics & Visualization.*
