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
  <summary>Distribution of Key Markers</summary>

#### Glucose
- Glucose values show a right-skewed distribution.
- Most individuals fall between 80 and 140 mg/dL, which is typical for fasting glucose.
- A few extreme values above 180 mg/dL indicate possible undiagnosed diabetes or poor glycemic control.
- The presence of zeros suggests missing or unrecorded glucose measurements.

**Insight:**
- Glucose levels vary widely across the population, with a notable portion showing elevated values linked to higher diabetes risk.

#### Blood Pressure
- Blood pressure (Diastolic) is moderately right-skewed.
- Most values cluster between 60 and 90 mmHg, which is within normal to slightly elevated range.
- Several zero or near-zero values reflect missing or invalid clinical measurements.
- Outliers above 100 mmHg indicate potential hypertension.

**Insight:**
While the majority fall in normal ranges, the dataset contains questionable zero readings and a small number of hypertensive cases.

### BMI
- BMI is fairly normally distributed, with a slight right skew.
- Most individuals have a BMI between 25 and 35, representing overweight to obese categories.
- Outliers above 50 indicate severe obesity.
- The distribution highlights high obesity prevalence in this population.

**Insight:**
- BMI trends show that excess body weight is common, reinforcing its role as a major diabetes risk factor.

### Insulin
- Insulin has the heaviest right skew among all variables.
- A large concentration of values lies below 100 µU/mL.
- Many individuals have insulin = 0, indicating missing or uncollected laboratory data.
- Extreme outliers range from 200 to 800+ µU/mL, which is far beyond typical clinical ranges.

**Insight:**
- Insulin values require careful preprocessing due to extreme skewness and biologically improbable outliers.

</details>

<details>
  <summary>All Key Marker Images</summary>

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
**Insight:** 
- Diabetic individuals show a substantially higher glucose distribution compared to non-diabetics — with a right-skewed histogram, a higher median in the box plot, and more high‑glucose outliers.
  
#### Blood Pressure
**Insight:** 
- Blood pressure tends to be elevated in diabetic individuals compared to non-diabetics, with a broader distribution and higher median, reflecting how hypertension often coexists with diabetes.

#### BMI
**Insight:** 
- BMI is generally higher in the diabetic population, with a right-skewed distribution indicating more individuals in overweight or obese ranges. The higher median and greater IQR suggest BMI is a key risk factor.

#### Insulin 
**Insight:** 
- Insulin levels in diabetics tend to be higher and more variable, suggesting compensatory hyperinsulinemia in response to insulin resistance.

</details>

<details>
  <summary>All Distribution Charts by Outcomes</summary>

[Glucose](<img width="1103" height="360" alt="Glucose Dist  by Outcome" src="https://github.com/user-attachments/assets/794871a6-0290-4937-939b-9b9f43a2f50e" />)
[Blood Pressure](<img width="1103" height="360" alt="BloodPressure Dist  by Outcomes" src="https://github.com/user-attachments/assets/04952e23-4553-449f-99f7-7336e79e5caa" />)
[BMI](<img width="1103" height="360" alt="BMI Dist  by Outcomes" src="https://github.com/user-attachments/assets/520339fd-3d99-404e-832a-c5f39cd8ab6b" />)
[Insulin](<img width="1103" height="360" alt="Insulin Dist  by Outcome" src="https://github.com/user-attachments/assets/c45de211-e5c4-488c-88ea-702a40445c6d" />)

</details>

---

### 3. **Relationship between BMI & glucose levels between diabetic and non-diabetic individuals(outcomes)**
The aim of this analysis is to examine how **BMI correlates with glucose levels** differently for diabetic vs non‑diabetic individuals, shedding light on potential risk patterns and metabolic differences.

<details>
<summary>Insights</summary>

- There is a **positive relationship** between BMI and glucose levels overall.
- **Non-diabetic individuals** show a mild upward trend: glucose increases gradually with BMI, suggesting early metabolic strain but generally stable glucose levels.
- **Diabetic individuals** exhibit a much **steeper increase** in glucose with rising BMI, with higher glucose values at almost all BMI levels.
- Diabetics also show **greater variability**, and some maintain high glucose even at lower BMI values, indicating metabolic heterogeneity (e.g., lean diabetes).
- These patterns support the role of **insulin resistance**: as BMI increases, insulin sensitivity decreases, raising glucose—an effect that appears stronger in diabetics.

</details>

<details>
<summary>BMI vs Glucose Chart</summary>
[BMI vs Glucose](<img width="1103" height="360" alt="Relationship btw BMI   Glucose" src="https://github.com/user-attachments/assets/ab503489-54f0-4750-b58e-bc922e62e651" />)

</details>

---

### 4. **How does age affect glucose and BMI levels between diabetes outcomes**
The aim of this analysis is to investigate how age influences glucose and BMI levels in individuals with different diabetes outcomes (diabetic vs non-diabetic), exploring potential interactions between age and diabetes status on these health markers. 

<details>
<summary><strong>Click to expand insights</strong></summary>

#### 🔹 Age vs Glucose
- Glucose levels are **consistently higher** in diabetic individuals across all ages.
- As age increases, diabetics show a **more noticeable upward trend** in glucose, indicating reduced glucose tolerance over time.
- Non-diabetic individuals maintain **lower and more stable glucose levels**, with only slight increases in older ages.

**Insight:**  
Age amplifies glucose differences between diabetic and non-diabetic individuals.

#### 🔹 Age vs BMI
- Diabetic individuals generally show **higher BMI** across nearly all age groups.
- BMI tends to **increase through early and middle adulthood**, especially among diabetics.
- In older ages, BMI may level off or slightly decline due to muscle loss, but diabetics still remain higher overall.
- Non-diabetics show **less aggressive changes** in BMI with age.

**Insight:**  
BMI increases with age for both groups, but diabetics maintain noticeably higher values.

#### 🔹 Overall Pattern
- Age magnifies metabolic differences between diabetic and non-diabetic groups.
- Both glucose and BMI show **steeper age-related changes** in diabetic individuals.
- Older diabetic individuals exhibit the **highest glucose and BMI values**, reflecting greater metabolic risk.

**Conclusion:**  
Age is a key factor influencing metabolic health, with diabetic individuals showing stronger upward trends in glucose and BMI as they age.

</details>

<details>
  <summary>Click here to view charts</summary>
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

**Insight:**  
Higher pregnancy history is associated with elevated glucose, especially in diabetic women.

#### 🔹 BMI Levels
- Diabetic individuals generally have **higher BMI** across pregnancy groups.  
- BMI shows a mild **upward trend with more pregnancies** among diabetics.  
- Non-diabetic BMI values remain more moderate and consistent.

**Insight:**  
Multiple pregnancies may contribute to long-term weight gain, especially among diabetic individuals.

#### 🔹 Insulin Levels
- Insulin levels show **greater variability** in diabetic individuals.  
- Diabetics display **higher median insulin values**, reflecting metabolic imbalance.  
- Non-diabetic insulin values remain lower and stable.

**Insight:**  
Increasing pregnancy count may indicate rising insulin resistance in diabetic women.

#### 🔹 Overall Pattern
- The metabolic gap between diabetic and non-diabetic individuals **widens** as pregnancy count increases.  
- Even at **0–1 pregnancies**, diabetics already show elevated metabolic markers.  
- More pregnancies amplify differences in glucose, BMI, and insulin.

**Overall Conclusion:**  
Pregnancy history plays a meaningful role in metabolic health, with diabetic women showing greater sensitivity to higher pregnancy counts.

</details>

<details>
<summary>Click here to view charts</summary>
[Glucose_levels](<img width="1103" height="360" alt="Glucose levels" src="https://github.com/user-attachments/assets/80848c46-9652-44d3-a5eb-9afb102d4173" />)
[BMI_levels](<img width="1103" height="360" alt="BMI levels" src="https://github.com/user-attachments/assets/66d0d016-e968-47ec-8dd1-bc4e3b4f66ab" />)
[Insulin_levels](<img width="1103" height="360" alt="Insulin levels" src="https://github.com/user-attachments/assets/a94e1184-4496-4234-8cfe-8e05027d41e1" />)

</details>

---
## 6. **How does genetic risk (Diabetes Pedigree Function) relate to diabetes outcomes?**
To examine how genetic predisposition, measured through the Diabetes Pedigree Function (DPF), differs between diabetic and non-diabetic individuals, and to determine whether higher genetic risk scores are associated with a greater likelihood of diabetes.

  <details>
<summary><strong>Click to expand insights</strong></summary>

#### 🔹 Key Insights
- Diabetic individuals tend to have **higher DPF values** compared to non-diabetics.  
- The distribution for diabetics shows a **shift toward the right**, indicating stronger genetic influence for many individuals.  
- Non-diabetic individuals cluster around **lower genetic risk scores**, with fewer high-DPF cases.

#### 🔹 Interpretation
- A higher Diabetes Pedigree Function indicates a **stronger family history and higher inherited risk** for diabetes.
- The wider spread of DPF among diabetics suggests that:
  - Some individuals have **very high genetic risk**, while  
  - Others develop diabetes primarily due to **non-genetic factors** (age, BMI, glucose, lifestyle).

#### Overall Conclusion
Higher DPF scores are associated with a **greater likelihood of being diabetic**, highlighting the role of genetic predisposition.  
However, genetics alone does not determine diabetes status—environmental and lifestyle factors also play critical roles.

</details>

<details>
<summary>DPF by Outcome Chart</summary>
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

### Findings
- **Glucose** is the strongest indicator of diabetes; higher levels are closely linked to diabetic outcomes.  
- **BMI** shows a moderate positive association with diabetes; higher BMI increases risk.  
- **Insulin** exhibits variability and missing values, but elevated levels are observed in diabetics.  
- **Genetic Risk (Diabetes Pedigree Function)** tends to be higher in diabetics, indicating hereditary influence.  
- **Age** and **pregnancy count** influence metabolic markers, with older age and higher pregnancies linked to higher glucose and BMI.  
- **Blood Pressure** and **Skin Thickness** show weak or moderate correlations with diabetes outcome.  
- **Correlation analysis** highlights relationships such as Glucose ↔ Insulin and BMI ↔ Skin Thickness, while other variables operate more independently.

### Recommendations
- **Predictive Modeling:** Focus on glucose, BMI, and DPF as primary predictors for diabetes classification.  
- **Health Interventions:** Monitor glucose and BMI regularly, especially for individuals with higher genetic risk or older age. Lifestyle interventions (diet, exercise) are recommended.  
- **Early Screening:** Women with multiple pregnancies or strong family history should be prioritized for early diabetes screening.  
- **Data Improvements:** Consider imputing missing insulin values or collecting more complete data for better analysis.

### Conclusion
- Glucose, BMI, and genetic risk are the **most informative markers** for assessing diabetes risk.  
- Age, pregnancy count, and BMI influence metabolic health, amplifying diabetes risk in susceptible individuals.  
- Correlation patterns help identify linked features and independent risk factors, guiding future modeling and analysis.  
- Overall, diabetes outcomes are shaped by a **combination of metabolic, genetic, and demographic factors**, reinforcing the importance of a multifactorial approach to risk assessment and prevention.




6. 
