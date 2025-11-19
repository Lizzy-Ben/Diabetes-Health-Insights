# **Diabetes Health Insights: EDA of Pima Indians Dataset**
## Project Overview
- This project explores the Pima Indians Diabetes dataset through exploratory data analysis (EDA) to uncover meaningful health insights. The analysis focuses on understanding how key health markers relate to diabetes outcome and how factors such as age, BMI, pregnancies, and genetic risk influence diabetes likelihood.
## Objectives
- Analyse distributions of important health indicators.
- Compare health markers between diabetic and non-diabetic individuals.
- Examine relationships between BMI, glucose, age, pregnancies, and insulin.
- Explore correlation structure among all health variables.
- Evaluate how genetic risk influences diabetes outcomes.
## Dataset Source
- Pima Indians Diabetes Dataset available publicly on Kaggle. [Download_here](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database)
## Tools Used
- Python
## Exploratory Data Analysis (EDA)
Below are the 7 key analysis questions addressed in this project.  
Each section includes collapsible dropdowns showing the corresponding chart(s).
1. How are key health markers distributed?
- To understand the general health patterns in the Pima Indians Diabetes dataset, we explored the distribution of four important clinical markers: **Glucose, Blood Pressure, BMI and Insulin.** These variables play major roles in assessing metabolic health and identifying diabetes risk.
<details>
<summary><strong>📊 Distribution of Key Health Markers</strong></summary>
<br>
  
<details>
  
<summary><strong>🩸 Glucose Distribution</strong></summary>
<br>
(<img width="989" height="360" alt="Distribution of Glucose" src="https://github.com/user-attachments/assets/e050e1ce-15d7-4051-9799-7b2b147561c3" />)

**Glucose Distribution**
- Glucose values show a right-skewed distribution.
- Most individuals fall between 80 and 140 mg/dL, which is typical for fasting glucose.
- A few extreme values above 180 mg/dL indicate possible undiagnosed diabetes or poor glycemic control.
- The presence of zeros suggests missing or unrecorded glucose measurements.

***Insight:***
- Glucose levels vary widely across the population, with a notable portion showing elevated values linked to higher diabetes risk.

</details>

---

<details>
<summary><strong>💓 Blood Pressure Distribution</strong></summary>

<br>

**Image Placeholder:**  
![Blood Pressure Distribution](images/bloodpressure_distribution.png)

**Insights:**  
- Moderately right-skewed  
- Most readings range from 60–90 mmHg  
- Zeros/unrealistically low values indicate missing data  
- Some values >100 mmHg suggest possible hypertension  

</details>

---

<details>
<summary><strong>⚖️ BMI Distribution</strong></summary>

<br>

**Image Placeholder:**  
![BMI Distribution](images/bmi_distribution.png)

**Insights:**  
- Roughly normal distribution with slight right skew  
- Most values fall between 25–35 → overweight/obese  
- Outliers above 50 indicate severe obesity  

</details>

---

<details>
<summary><strong>🧪 Insulin Distribution</strong></summary>

<br>

**Image Placeholder:**  
![Insulin Distribution](images/insulin_distribution.png)

**Insights:**  
- Extremely right-skewed  
- Many values below 100 µU/mL  
- Numerous zeros suggest missing or unrecorded insulin tests  
- Several extreme outliers (300–800+)  

</details>

---

</details>
