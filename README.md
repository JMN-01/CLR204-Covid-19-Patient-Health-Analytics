# CLR204-Covid-19-Patient-Health-Analytics
#### A machine learning study evaluating and comparing classification models including a Boosted Random Forest architecture to predict clinical outcomes and recovery/mortality status for COVID-19 patients based on demographic and clinical feature
---
## 📌 Project Overview
- This project was completed as part of the **CLR204 Classification and Regression** coursework. It reproduces and expands upon clinical predictive modeling techniques (referencing study methodology by *Iwendi et al., 2020*) to assess patient mortality risk.
- By analyzing patient demographics, symptom timelines, geographical data, and health indicators, multiple classification algorithms were trained, tuned, and benchmarked to identify the most accurate model for clinical decision support.
---
## Dataset source
####  The original dataset was taken from: https://www.kaggle.com/sudalairajkumar/novel-corona-virus-2019-dataset
---
## 🛠️ Key Technical Steps & Pipeline

1. **Data Preprocessing & Cleaning:**
   - Handled missing and non-standard values across key features (e.g., symptom onset, hospitalization dates, location data).
   - Engineered temporal features including `symptom_to_hospital_days`.
   - Categorized symptoms and encoded categorical clinical variables.
   - Addressed class imbalance between recovered and deceased patient outcomes.

2. **Model Training & Comparison:**
   Evaluated **5 Machine Learning Algorithms**:
   - **Boosted Random Forest Classifier** (Primary focus)
   - **Logistic Regression**
   - **Decision Tree Classifier**
   - **Support Vector Machine (SVM)**
   - **Gaussian Naive Bayes**

3. **Evaluation Metrics:**
   - Models were benchmarked using **Accuracy**, **Precision**, **Recall**, and **F1-Score** to ensure balanced assessment under class imbalance.

---
