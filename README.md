# 🧠 A Comparative Analysis and Predictive Model for Reporting Depression in U.S. Adults

This project investigates discrepancies between **self-reported depression** and **provider-diagnosed depression** among U.S. adults using two national datasets (NHANES and NAMCS). We developed classification models to predict underreporting or misreporting patterns and identify at-risk demographic groups for more targeted screening and policy interventions.

## 📌 Project Overview

Despite rising mental health awareness, depression remains underdiagnosed, especially in underserved communities. This study performs:
- A **comparative statistical analysis** between NHANES (self-reported) and NAMCS (provider-reported) depression data.
- A **binary classification model** to predict depression indicators from demographic and clinical attributes.
- A **feature importance assessment** to identify key risk factors impacting depression reporting.

## 🧪 Methodology

1. **Data Sources**:  
   - `NHANES 2018`: National Health and Nutrition Examination Survey  
   - `NAMCS 2018`: National Ambulatory Medical Care Survey  
2. **Preprocessing**:
   - Converted `.sas7bdat` and `.xpt` files to CSV
   - Feature engineering across 40+ variables: age, race, comorbidities, insurance, education, etc.
   - Created unified `Depression Indicator (DI)` using PHQ-9, diagnosis codes, and treatment variables
3. **Modeling Techniques**:
   - Models: `XGBoost`, `Random Forest`
   - Techniques: SMOTE balancing, Chi-square feature selection
   - Evaluation Metrics: Accuracy, Precision, Recall, F1 Score, PR Curve, ROC AUC

## 📊 Key Results

🔍 **Achieved 85% accuracy and 0.83 AUC** using XGBoost on provider-diagnosed depression data (NAMCS), successfully modeling clinical recognition patterns.

🔍 **Identified critical risk indicators** (e.g., lack of chronic illness, insurance status, cancer history) by analyzing 40+ features, revealing disparities in depression diagnosis and access.

🔍 **Exposed inconsistencies in self-reporting**: Lower predictive performance on self-reported depression (NHANES) highlights the complexity of mental health disclosure, suggesting underreporting trends and the need for improved public health screening tools.

## 🧰 Tools & Technologies

- **Languages**: Python (Jupyter, Colab)
- **Libraries**: pandas, NumPy, Seaborn, Matplotlib, SciPy, scikit-learn, imbalanced-learn, XGBoost
- **Data Tools**: phpMyAdmin, MySQL, SAS7BDAT/XPORT conversion, Advanced Excel
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

