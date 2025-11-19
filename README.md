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
- Python (Pandas, Numpy, Plotly Express)
## Key Findings
- **Glucose** is the strongest indicator of diabetes; higher levels are closely linked to diabetic outcomes.  
- **BMI** shows a moderate positive association with diabetes; higher BMI increases risk.  
- **Insulin** exhibits variability and missing values, but elevated levels are observed in diabetics.  
- **Genetic Risk (Diabetes Pedigree Function)** tends to be higher in diabetics, indicating hereditary influence.  
- **Age** and **pregnancy count** influence metabolic markers, with older age and higher pregnancies linked to higher glucose and BMI.  
- **Blood Pressure** and **Skin Thickness** show weak or moderate correlations with diabetes outcome.  
- **Correlation analysis** highlights relationships such as Glucose ↔ Insulin and BMI ↔ Skin Thickness, while other variables operate more independently.
## Recommendations
- **Predictive Modeling:** Focus on glucose, BMI, and DPF as primary predictors for diabetes classification.  
- **Health Interventions:** Monitor glucose and BMI regularly, especially for individuals with higher genetic risk or older age. Lifestyle interventions (diet, exercise) are recommended. 
- **Early Screening:** Women with multiple pregnancies or strong family history should be prioritized for early diabetes screening.  
- **Data Improvements:** Consider imputing missing insulin values or collecting more complete data for better analysis.
## Conclusion
- Glucose, BMI, and genetic risk are the **most informative markers** for assessing diabetes risk.  
- Age, pregnancy count, and BMI influence metabolic health, amplifying diabetes risk in susceptible individuals.  
- Correlation patterns help identify linked features and independent risk factors, guiding future modeling and analysis.  
- Overall, diabetes outcomes are shaped by a **combination of metabolic, genetic, and demographic factors**, reinforcing the importance of a multifactorial approach to risk assessment and prevention.
## Detailed EDA
For the **full exploratory data analysis**, including all charts and insights, see [EDA Details](EDA.md)
