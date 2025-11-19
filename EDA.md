# Diabetes Health Insights: Summary EDA

## Overview
Exploratory Data Analysis (EDA) of the Pima Indians Diabetes dataset to understand how health markers relate to diabetes outcomes.

---

### Key Findings from Health Markers

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

### Health Markers by Diabetes Outcome

<details>
<summary>Comparison of Diabetic vs Non-Diabetic</summary>

- Diabetics show **higher glucose, BMI, blood pressure, and insulin**.  
- Non-diabetics maintain lower and more stable marker levels.

**Charts Placeholder:**  
- ![Glucose Outcome](#)  
- ![BMI Outcome](#)

</details>

---

### BMI vs Glucose Relationship

<details>
<summary>Insights</summary>

- Positive correlation between BMI and glucose.  
- Diabetics: **steeper increase** in glucose with BMI.  
- Non-diabetics: mild upward trend.  

**Chart Placeholder:** ![BMI vs Glucose](#)

</details>

---

### Effect of Age

<details>
<summary>Age vs Glucose and BMI</summary>

- Diabetics: **higher glucose and BMI** across all ages; steeper age-related increase.  
- Non-diabetics: stable or moderate increase.  

**Charts Placeholder:**  
- ![Age vs Glucose](#)  
- ![Age vs BMI](#)

</details>

---

### Pregnancy Influence

<details>
<summary>Glucose, BMI, Insulin vs Number of Pregnancies</summary>

- Higher pregnancies: **increase in glucose and BMI**, especially in diabetics.  
- Insulin variability rises with pregnancy count.  

**Charts Placeholder:**  
- ![Glucose](#)  
- ![BMI](#)  
- ![Insulin](#)

</details>

---

### Genetic Risk (DPF) vs Diabetes Outcome

<details>
<summary>Insights</summary>

- Diabetics have **higher Diabetes Pedigree Function scores**.  
- High genetic risk increases likelihood of diabetes but does not guarantee it.

**Chart Placeholder:** ![DPF vs Outcome](#)

</details>

---

### Correlation Between Health Markers

<details>
<summary>Insights</summary>

- **Strong correlations:** Glucose ↔ Outcome, BMI ↔ Insulin.  
- **Weak correlations:** Blood Pressure with most variables.  
- Glucose and BMI are most influential for diabetes risk.

**Chart Placeholder:** ![Correlation](#)

</details>

---

### Summary
- **Top indicators:** Glucose, BMI, Genetic Risk (DPF).  
- **Influencing factors:** Age, pregnancy, insulin levels.  
- **Correlation patterns** highlight key relationships and independent risk factors.  
