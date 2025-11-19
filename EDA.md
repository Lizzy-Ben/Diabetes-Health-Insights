# Diabetes Health Insights: Summary EDA

## Overview
Exploratory Data Analysis (EDA) of the Pima Indians Diabetes dataset to understand how health markers relate to diabetes outcomes.

---

### 1. How are key health markers distributed?

<details>
<summary>Distributions of Glucose, Blood Pressure, BMI, Insulin</summary>

- **Glucose:** Right-skewed; higher in diabetics.  
- **Blood Pressure:** Mostly normal, slightly elevated in diabetics.  
- **BMI:** Higher in diabetics; many overweight/obese individuals.  
- **Insulin:** Highly skewed; higher and more variable in diabetics.  

**Charts Placeholder:**  
- ![Glucose](<img width="989" height="360" alt="Distribution of Glucose" src="https://github.com/user-attachments/assets/05be00f3-3365-4f49-b484-8be63bf82f39" />)
- ![Blood Pressure](<img width="1101" height="360" alt="Distribution of Blood Pressure" src="https://github.com/user-attachments/assets/ef571cc0-fe8b-4fbd-a5ea-a88a9dafdbe7" />)
- ![BMI](<img width="1101" height="360" alt="Distribution of BMI" src="https://github.com/user-attachments/assets/fba928e9-e9fc-4ad3-bdc7-17fc09ff0eb1" />)  
- ![Insulin](<img width="1101" height="360" alt="Distribution of Insulin" src="https://github.com/user-attachments/assets/6e3a73e5-f2bb-4608-807f-134c00200d4a" />)


</details>

---

### 2. How do these markers differ between diabetic and non-diabetic individuals? 

<details>
<summary>Comparison of Diabetic vs Non-Diabetic</summary>

- Diabetics show **higher glucose, BMI, blood pressure, and insulin**.  
- Non-diabetics maintain lower and more stable marker levels.

**Charts Placeholder:**  
- ![Glucose Outcome](<img width="1103" height="360" alt="Glucose Dist  by Outcome" src="https://github.com/user-attachments/assets/794871a6-0290-4937-939b-9b9f43a2f50e" />)
- ![BMI Outcome](<img width="1103" height="360" alt="BloodPressure Dist  by Outcomes" src="https://github.com/user-attachments/assets/04952e23-4553-449f-99f7-7336e79e5caa" />)

</details>

---

### 3. Relationship between BMI & glucose levels between diabetic and non-diabetic individuals(outcomes)

<details>
<summary>Insights</summary>

- Positive correlation between BMI and glucose.  
- Diabetics: **steeper increase** in glucose with BMI.  
- Non-diabetics: mild upward trend.  

**Chart Placeholder:** 
![BMI vs Glucose](<img width="1103" height="360" alt="Relationship btw BMI   Glucose" src="https://github.com/user-attachments/assets/ab503489-54f0-4750-b58e-bc922e62e651" />)

</details>

---

### 4. How does age affect glucose and BMI levels between diabetes outcomes?

<details>
<summary>Age vs Glucose and BMI</summary>

- Diabetics: **higher glucose and BMI** across all ages; steeper age-related increase.  
- Non-diabetics: stable or moderate increase.  

**Charts Placeholder:**  
- ![Age vs Glucose](<img width="1103" height="360" alt="Age vs Glucose" src="https://github.com/user-attachments/assets/dd99b9cc-bd7a-4158-870a-6add19366c37" />)  
- ![Age vs BMI](<img width="1103" height="360" alt="Age vs BMI" src="https://github.com/user-attachments/assets/ab10bfe0-2244-476e-9299-d14d3a6a4318" />)

</details>

---

### 5. Compare Glucose, BMI and Insulin distributions by number of pregnancies

<details>
<summary>Glucose, BMI, Insulin vs Number of Pregnancies</summary>

- Higher pregnancies: **Increase in glucose and BMI**, especially in diabetics.  
- Insulin variability rises with pregnancy count.  

**Charts Placeholder:**  
- ![Glucose](<img width="1103" height="360" alt="Glucose levels" src="https://github.com/user-attachments/assets/80848c46-9652-44d3-a5eb-9afb102d4173" />)
- ![BMI](<img width="1103" height="360" alt="BMI levels" src="https://github.com/user-attachments/assets/66d0d016-e968-47ec-8dd1-bc4e3b4f66ab" />)  
- ![Insulin](<img width="1103" height="360" alt="Insulin levels" src="https://github.com/user-attachments/assets/a94e1184-4496-4234-8cfe-8e05027d41e1" />)

</details>

---

### 6. How does genetic risk (Diabetes Pedigree Function) relate to diabetes outcomes?

<details>
<summary>Insights</summary>

- Diabetics have **higher Diabetes Pedigree Function scores**.  
- High genetic risk increases likelihood of diabetes but does not guarantee it.

**Chart Placeholder:** 
![DPF vs Outcome](<img width="989" height="360" alt="DPF" src="https://github.com/user-attachments/assets/c587d466-8f87-42af-ad41-3e449c4dcb8f" />)

</details>

---

### 7. Correlation between the different health markers. Are some linked?

<details>
<summary>Insights</summary>

- **Strong correlations:** Glucose ↔ Outcome, BMI ↔ Insulin.  
- **Weak correlations:** Blood Pressure with most variables.  
- Glucose and BMI are most influential for diabetes risk.

**Chart Placeholder:** 
![Correlation](<img width="1103" height="360" alt="Correlation" src="https://github.com/user-attachments/assets/6d344fa9-5af6-46d5-88c6-6aec8fe7febc" />)

</details>

---

## Summary
- **Top indicators:** Glucose, BMI, Genetic Risk (DPF).  
- **Influencing factors:** Age, pregnancy, insulin levels.  
- **Correlation patterns** highlight key relationships and independent risk factors.  
