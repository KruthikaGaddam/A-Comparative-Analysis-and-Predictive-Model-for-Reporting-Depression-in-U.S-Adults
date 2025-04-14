# 🧠 A Comparative Analysis and Predictive Model for Reporting Depression in U.S. Adults

This project investigates discrepancies between **self-reported depression** and **provider-diagnosed depression** among U.S. adults using two national datasets (NHANES and NAMCS). We developed classification models to predict underreporting or misreporting patterns and identify at-risk demographic groups for more targeted screening and policy interventions.

## 📌 Project Overview

Despite rising mental health awareness, depression remains underdiagnosed, especially in underserved communities. This study performs:
- A **comparative statistical analysis** between NHANES (self-reported) and NAMCS (provider-reported) depression data.
- A **binary classification model** to predict depression indicators from demographic and clinical attributes.
- A **feature importance assessment** to identify key risk factors impacting depression reporting.

## 🧪 Methodology

1. **Data Sources**:  
   - `NHANES 2017-18`: National Health and Nutrition Examination Survey  
   - `NAMCS 2017-18`: National Ambulatory Medical Care Survey  
2. **Preprocessing**:
   - Converted `.sas7bdat` and `.xpt` files to CSV
   - Feature engineering across 40+ variables: age, race, comorbidities, insurance, education, etc.
   - Created unified `Depression Indicator (DI)` using PHQ-9, diagnosis codes, and treatment variables
3. **Modeling Techniques**:
   - Models: `XGBoost`, `Random Forest`
   - Techniques: SMOTE balancing, Chi-square feature selection
   - Evaluation Metrics: Accuracy, Precision, Recall, F1 Score, PR Curve, ROC AUC

## 📊 Key Results

### ✳️ Model Performance (After SMOTE)

| Dataset | Model          | Accuracy | F1 Score | AUC (ROC) | Top Features                            |
|---------|----------------|----------|----------|-----------|------------------------------------------|
| NHANES  | XGBoost        | 73.8%    | 0.36     | 0.65      | Private Insurance, Arthritis, Overweight |
| NAMCS   | XGBoost        | 85%      | 0.53     | 0.83      | No Chronic Illness, Heart/Lung Issues, Cancer |
| NHANES  | Random Forest  | 72.9%    | 0.35     | 0.68      | Overweight, Insurance, Arthritis         |
| NAMCS   | Random Forest  | 84.5%    | 0.53     | 0.85      | Surgical Care, No Chronic Illness, Age   |

### ✅ Hypothesis Testing:
- **Chi-square test** showed significant differences in reporting patterns based on age, insurance type, race, comorbidities, and provider specialty.
- **Rejected Null Hypothesis**: Self-reported depression was *less frequently detected* compared to provider diagnoses, indicating underreporting.

## 🧰 Tools & Technologies

- **Languages**: Python (Jupyter, Colab)
- **Libraries**: pandas, NumPy, Seaborn, Matplotlib, SciPy, scikit-learn, imbalanced-learn, XGBoost
- **Data Tools**: phpMyAdmin, MySQL, SAS7BDAT/XPORT conversion
- **Collaboration**: Microsoft Teams, Canvas, Wrike

## 📈 Impact

This model can inform:
- **Policy interventions** to address mental health screening gaps
- **Clinical decision-making tools** for underdiagnosed groups
- **Future research** into stigma-related non-disclosure patterns in mental health

## 👩‍🔬 Team Members

- Kruthika Gaddam  
- Kiran Mai Jaiswal Charpuria  
- Mohith Surya Kiran Kasula  
- Bala Samantula  
- Sri Harsha Sudalagunta  
- April Taylor  
- Alan Varkey

## 📄 Citation

If you reference or reuse this work, please cite.

