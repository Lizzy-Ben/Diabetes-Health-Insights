# Diabetes Health Insights: Summary EDA

## Overview
Exploratory Data Analysis (EDA) of the Pima Indians Diabetes dataset to understand how health markers relate to diabetes outcomes.
---
### 1.**How are key health markers distributed?**
To understand the general health patterns in the Pima Indians Diabetes dataset, we explored the distribution of four important clinical markers: **Glucose, Blood Pressure, BMI and Insulin.** These variables play major roles in assessing metabolic health and identifying diabetes risk.

<details>
  <summary>Distribution of Key Markers</summary>

#### Glucose
- Glucose values show a right-skewed distribution.
- Most individuals fall between 80 and 140 mg/dL, which is typical for fasting glucose.
- A few extreme values above 180 mg/dL indicate possible undiagnosed diabetes or poor glycemic control.
- Glucose levels vary widely across the population, with a notable portion showing elevated values linked to higher diabetes risk.
#### Blood Pressure
- Blood pressure (Diastolic) is moderately right-skewed.
- Most values cluster between 60 and 90 mmHg, which is within normal to slightly elevated range.
- Outliers above 100 mmHg indicate potential hypertension.
- While the majority fall in normal ranges, the dataset contains a small number of hypertensive cases.
### BMI
- BMI is fairly normally distributed, with a slight right skew.
- Most individuals have a BMI between 25 and 35, representing overweight to obese categories.
- Outliers above 50 indicate severe obesity.
- The distribution highlights high obesity prevalence in this population.
### Insulin
- Insulin has the heaviest right skew among all variables.
- A large concentration of values lies below 100 µU/mL.
- Many individuals have insulin = 0, indicating missing or uncollected laboratory data.
- Extreme outliers range from 200 to 800+ µU/mL, which is far beyond typical clinical ranges.
**Chart Placeholders**
- ![Glucose](<img width="989" height="360" alt="Distribution of Glucose" src="https://github.com/user-attachments/assets/e050e1ce-15d7-4051-9799-7b2b147561c3" />)  
- ![Blood Pressure](<img width="1101" height="360" alt="Distribution of Blood Pressure" src="https://github.com/user-attachments/assets/f83dea99-5376-4bca-971d-6d2fa5fa00f9" />)  
- ![BMI](<img width="1101" height="360" alt="Distribution of BMI" src="https://github.com/user-attachments/assets/d05674ff-2f17-4c47-850b-2ef89cceb8e9" />)  
- ![Insulin](<img width="1101" height="360" alt="Distribution of Insulin" src="https://github.com/user-attachments/assets/c48d8e2e-0484-45df-bdd9-2573cd7bb173" />)

</details>

---

### 2. **How do these markers differ between diabetic and non-diabetic individuals? (Outcome)**
The aim of this analysis is to gain insights into the characteristics of diabetic and non-diabetic individuals by comparing their health markers, ultimately informing strategies for diabetes risk assessment, prevention, and management.
<details>
  <summary>Outcome-Based Health Marker Comparison"</summary>

#### Glucose 
- Diabetic individuals show a substantially higher glucose distribution compared to non-diabetics — with a right-skewed histogram, a higher median in the box plot, and more high‑glucose outliers.
#### Blood Pressure
- Blood pressure tends to be elevated in diabetic individuals compared to non-diabetics, with a broader distribution and higher median, reflecting how hypertension often coexists with diabetes.
#### BMI
- BMI is generally higher in the diabetic population, with a right-skewed distribution indicating more individuals in overweight or obese ranges. The higher median and greater IQR suggest BMI is a key risk factor.
#### Insulin 
- Insulin levels in diabetics tend to be higher and more variable, suggesting compensatory hyperinsulinemia in response to insulin resistance.

** Chart Placeholders**
[Glucose](<img width="1103" height="360" alt="Glucose Dist  by Outcome" src="https://github.com/user-attachments/assets/794871a6-0290-4937-939b-9b9f43a2f50e" />)
[Blood Pressure](<img width="1103" height="360" alt="BloodPressure Dist  by Outcomes" src="https://github.com/user-attachments/assets/04952e23-4553-449f-99f7-7336e79e5caa" />)
[BMI](<img width="1103" height="360" alt="BMI Dist  by Outcomes" src="https://github.com/user-attachments/assets/520339fd-3d99-404e-832a-c5f39cd8ab6b" />)
[Insulin](<img width="1103" height="360" alt="Insulin Dist  by Outcome" src="https://github.com/user-attachments/assets/c45de211-e5c4-488c-88ea-702a40445c6d" />)

</details>

---

### 3. **Relationship between BMI & glucose levels between diabetic and non-diabetic individuals(outcomes)**
- There is a **positive relationship** between BMI and glucose levels overall.
- **Non-diabetic individuals** show a mild upward trend: glucose increases gradually with BMI, suggesting early metabolic strain but generally stable glucose levels.
- **Diabetic individuals** exhibit a much **steeper increase** in glucose with rising BMI, with higher glucose values at almost all BMI levels.
- Diabetics also show **greater variability**, and some maintain high glucose even at lower BMI values, indicating metabolic heterogeneity (e.g., lean diabetes).
- These patterns support the role of **insulin resistance**: as BMI increases, insulin sensitivity decreases, raising glucose—an effect that appears stronger in diabetics.

**Chart Placeholder**
[BMI vs Glucose](<img width="1103" height="360" alt="Relationship btw BMI   Glucose" src="https://github.com/user-attachments/assets/ab503489-54f0-4750-b58e-bc922e62e651" />)

---

### 4. **How does age affect glucose and BMI levels between diabetes outcomes**
<details>
<summary><strong>Click to expand insights</strong></summary>

#### 🔹 Age vs Glucose
- Glucose levels are **consistently higher** in diabetic individuals across all ages.
- As age increases, diabetics show a **more noticeable upward trend** in glucose, indicating reduced glucose tolerance over time.
#### 🔹 Age vs BMI
- Diabetic individuals generally show **higher BMI** across nearly all age groups.
- In older ages, BMI may level off or slightly decline due to muscle loss, but diabetics still remain higher overall.
- Non-diabetics show **less aggressive changes** in BMI with age.
#### 🔹 Overall Pattern
- Age magnifies metabolic differences between diabetic and non-diabetic groups.
- Both glucose and BMI show **steeper age-related changes** in diabetic individuals.
- Older diabetic individuals exhibit the **highest glucose and BMI values**, reflecting greater metabolic risk.

** Check Placeholders**
[Age vs BMI](<img width="1103" height="360" alt="Age vs Glucose" src="https://github.com/user-attachments/assets/dd99b9cc-bd7a-4158-870a-6add19366c37" />)
[Age vs Glucose](<img width="1103" height="360" alt="Age vs BMI" src="https://github.com/user-attachments/assets/ab10bfe0-2244-476e-9299-d14d3a6a4318" />)

<details>

---

### 5. **Compare Glucose, BMI and Insulin distributions by number of pregnancies**
This section explores how key metabolic markers vary across different pregnancy counts for diabetic and non-diabetic individuals.

<details>
<summary><strong>Click to expand insights</strong></summary>

#### 🔹 Glucose Levels
- Diabetic individuals consistently show **higher glucose levels** across all pregnancy counts.  
- Glucose values tend to **increase slightly as pregnancy count increases**.  
- Non-diabetic individuals maintain **lower and stable** glucose values.
#### 🔹 BMI Levels
- Diabetic individuals generally have **higher BMI** across pregnancy groups.  
- BMI shows a mild **upward trend with more pregnancies** among diabetics.  
- Multiple pregnancies may contribute to long-term weight gain, especially among diabetic individuals.
#### 🔹 Insulin Levels
- Insulin levels show **greater variability** in diabetic individuals.  
- Diabetics display **higher median insulin values**, reflecting metabolic imbalance.  
- Increasing pregnancy count may indicate rising insulin resistance in diabetic women.

** Chart Placeholders**
[Glucose_levels](<img width="1103" height="360" alt="Glucose levels" src="https://github.com/user-attachments/assets/80848c46-9652-44d3-a5eb-9afb102d4173" />)
[BMI_levels](<img width="1103" height="360" alt="BMI levels" src="https://github.com/user-attachments/assets/66d0d016-e968-47ec-8dd1-bc4e3b4f66ab" />)
[Insulin_levels](<img width="1103" height="360" alt="Insulin levels" src="https://github.com/user-attachments/assets/a94e1184-4496-4234-8cfe-8e05027d41e1" />)

</details>
---
## 6. **How does genetic risk (Diabetes Pedigree Function) relate to diabetes outcomes?**
To examine how genetic predisposition, measured through the Diabetes Pedigree Function (DPF), differs between diabetic and non-diabetic individuals, and to determine whether higher genetic risk scores are associated with a greater likelihood of diabetes.
<details>
<summary>Insights</summary>

- Diabetics have **higher Diabetes Pedigree Function scores**.  
- High genetic risk increases likelihood of diabetes but does not guarantee it.

** Chart Placeholder**
[DPF](<img width="989" height="360" alt="DPF" src="https://github.com/user-attachments/assets/c587d466-8f87-42af-ad41-3e449c4dcb8f" />)

</details>

---
### 7. Correlation between the different health markers. Are some linked?
The aim of this section is to explore the relationships between key health indicators—such as glucose levels, blood pressure, BMI, insulin, age, and genetic risk—to identify whether some markers tend to rise or fall together. By examining their correlations, we can uncover patterns that may contribute to diabetes risk and understand which variables have the strongest associations. This helps highlight which health metrics might be the most influential in predicting diabetes outcomes.

<details>
<summary><strong>Health markers insights summary</strong></summary>

#### 🔹 Glucose Levels and Diabetes Outcome
- Higher glucose levels are strongly associated with diabetes.  
- Diabetic individuals show much higher concentrations of elevated glucose compared to non-diabetic individuals.

#### 🔹 Blood Pressure Distribution
- Blood pressure does not show a strong separation between diabetic and non-diabetic individuals.  
- Most values cluster in a similar range, suggesting it is not a major standalone predictor.

#### 🔹 BMI and Diabetes Risk
- Diabetic individuals tend to have higher BMI values.  
- Suggests a positive relationship between body weight/obesity and diabetes likelihood.

#### 🔹 Insulin Levels
- Insulin contains many zeros, indicating missing or unrecorded values.  
- Among valid entries, diabetic individuals tend to show higher insulin levels, though insights are limited due to missing data.

#### 🔹 Genetic Risk (Diabetes Pedigree Function)
- Higher genetic risk scores are more common among diabetic individuals.  
- There is overlap between groups, but diabetics generally show slightly higher DPF distribution.

#### 🔹 Correlation Between Health Markers
- **Strongest positive correlation:** Glucose and Outcome  
- **Moderate correlations:** BMI with Skin Thickness, BMI with Insulin  
- **Weak or no correlations:** Blood pressure with most other variables  
- **Age shows mild correlation** with pregnancies and glucose

**Overall Insight:**  
Glucose and BMI appear to be the most influential health markers related to diabetes risk in this dataset.

</details>

<details>
<summary>Click here to view charts</summary>
[Correlation_between_health_markers](<img width="1103" height="360" alt="Correlation" src="https://github.com/user-attachments/assets/6d344fa9-5af6-46d5-88c6-6aec8fe7febc" />)

</details>

---

