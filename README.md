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
### 1.**How are key health markers distributed?**
To understand the general health patterns in the Pima Indians Diabetes dataset, we explored the distribution of four important clinical markers: **Glucose, Blood Pressure, BMI and Insulin.** These variables play major roles in assessing metabolic health and identifying diabetes risk.
<details>
<summary><strong> Distribution of Key Health Markers</strong></summary>
<br>
  
<details>
  
<summary><strong>🩸 Glucose Distribution</strong></summary>
<br>

- Glucose values show a right-skewed distribution.
- Most individuals fall between 80 and 140 mg/dL, which is typical for fasting glucose.
- A few extreme values above 180 mg/dL indicate possible undiagnosed diabetes or poor glycemic control.
- The presence of zeros suggests missing or unrecorded glucose measurements.

**Insight:**
- Glucose levels vary widely across the population, with a notable portion showing elevated values linked to higher diabetes risk.

<img width="989" height="360" alt="Distribution of Glucose" src="https://github.com/user-attachments/assets/e050e1ce-15d7-4051-9799-7b2b147561c3" />

</details>

---

<details>
<summary><strong>💓 Blood Pressure Distribution</strong></summary>
<br>

- Blood pressure (Diastolic) is moderately right-skewed.
- Most values cluster between 60 and 90 mmHg, which is within normal to slightly elevated range.
- Several zero or near-zero values reflect missing or invalid clinical measurements.
- Outliers above 100 mmHg indicate potential hypertension.

**Insight:**
While the majority fall in normal ranges, the dataset contains questionable zero readings and a small number of hypertensive cases.

<img width="1101" height="360" alt="Distribution of Blood Pressure" src="https://github.com/user-attachments/assets/f83dea99-5376-4bca-971d-6d2fa5fa00f9" />

</details>

---

<details>
<summary><strong>⚖️ BMI Distribution</strong></summary>

<br>

- BMI is fairly normally distributed, with a slight right skew.
- Most individuals have a BMI between 25 and 35, representing overweight to obese categories.
- Outliers above 50 indicate severe obesity.
- The distribution highlights high obesity prevalence in this population.

**Insight:**
- BMI trends show that excess body weight is common, reinforcing its role as a major diabetes risk factor.

<img width="1101" height="360" alt="Distribution of BMI" src="https://github.com/user-attachments/assets/d05674ff-2f17-4c47-850b-2ef89cceb8e9" />

</details>

---

<details>
<summary><strong>🧪 Insulin Distribution</strong></summary>

<br>

- Insulin has the heaviest right skew among all variables.
- A large concentration of values lies below 100 µU/mL.
- Many individuals have insulin = 0, indicating missing or uncollected laboratory data.
- Extreme outliers range from 200 to 800+ µU/mL, which is far beyond typical clinical ranges.

**Insight:**
- Insulin values require careful preprocessing due to extreme skewness, numerous missing values, and biologically improbable outliers.

<img width="1101" height="360" alt="Distribution of Insulin" src="https://github.com/user-attachments/assets/c48d8e2e-0484-45df-bdd9-2573cd7bb173" />

</details>

---

</details>

### 2. **How do these markers differ between diabetic and non-diabetic individuals? (Outcome)**

<details>
<summary><strong>Distribution by Diabetes Outcomes</strong></summary>
<br>
  
<details>
  
<summary><strong>🩸 Glucose Distribution by Outcomes</strong></summary>
<br>

<img width="1103" height="360" alt="Glucose Dist  by Outcome" src="https://github.com/user-attachments/assets/794871a6-0290-4937-939b-9b9f43a2f50e" />

</details>

---

<details>
<summary><strong>💓 Blood Pressure Distribution by Outcomes</strong></summary>
<br>

<img width="1103" height="360" alt="BloodPressure Dist  by Outcomes" src="https://github.com/user-attachments/assets/04952e23-4553-449f-99f7-7336e79e5caa" />

</details>

---

<details>
<summary><strong>⚖️ BMI Distribution by Outcomes</strong></summary>

<br>

<img width="1103" height="360" alt="BMI Dist  by Outcomes" src="https://github.com/user-attachments/assets/520339fd-3d99-404e-832a-c5f39cd8ab6b" />

</details>

---

<details>
<summary><strong>🧪 Insulin Distribution</strong></summary>

<br>

<img width="1103" height="360" alt="Insulin Dist  by Outcome" src="https://github.com/user-attachments/assets/c45de211-e5c4-488c-88ea-702a40445c6d" />

</details>

---

</details>

### 3. **Relationship between BMI & glucose levels between diabetic and non-diabetic individuals(outcomes)**

<img width="1103" height="360" alt="Relationship btw BMI   Glucose" src="https://github.com/user-attachments/assets/ab503489-54f0-4750-b58e-bc922e62e651" />

### 4. **How does age affect glucose and BMI levels between diabetes outcomes**
