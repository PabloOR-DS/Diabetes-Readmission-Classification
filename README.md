# Diabetes Readmission Prediction Project

## Project Title
A Machine Learning Approach to Predict Readmissions among Diabetic Inpatients (1999–2008)

## Description
This project aims to predict hospital readmissions among diabetic patients using real-world clinical data from 130 U.S. hospitals spanning the years 1999–2008. The dataset includes 101,766 hospital stays and 47 features covering demographics, clinical measurements, treatments, and prior healthcare utilization.

### Goals:
- **Primary**: Build a predictive model to classify whether a diabetic inpatient will be readmitted within or after 30 days of discharge.
- **Secondary**: 
  - Conduct exploratory data analysis (EDA) to understand variable distributions, missingness, and inter-feature relationships
  - Perform feature engineering (encoding categorical variables, handling missing values, mapping codes to categoricals)
  - Compare performance of multiple classification algorithms (logistic regression, random forest, LightGBM)
  - Select the most robust, scalable and high-performing model based on precision, recall, and ROC-AUC metrics
  - Identify the most important features for predicting hospital readmission
  - Interpret model outputs to provide actionable insights for healthcare providers

## Dataset
The dataset used is the **Diabetes 130-US Hospitals for Years 1999–2008**, curated by researchers from Virginia Commonwealth University. It is publicly available through the [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/296/diabetes+130-us+hospitals+for+years+1999-2008).

### Dataset Highlights:
- **Instances**: 101,766 hospital stays
- **Features**: 47 distinct features covering categorical and numeric data
- **Tasks**: Binary classification (predicting readmission)
- **Missing Values**: Present in several columns (weight, payer_code, medical_specialty, max_glu_serum, A1Cresult)

### Key Features:
- Patient demographics (age, gender, race)
- Admission details (type, source, length of stay)
- Clinical measurements and lab procedures
- Treatments (medications, diabetic-specific drugs)
- Prior healthcare utilization (outpatient, emergency, inpatient visits)
- Diagnostic information (primary, secondary, and additional diagnoses)

### Target Variable:
- `readmitted`: Binary classification (0 = not readmitted, 1 = readmitted within or after 30 days)

## Installation
To set up the environment and install required dependencies, run:

```bash
pip install -r requirements.txt
