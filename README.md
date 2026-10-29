# CLR204-Covid-19-Patient-Health-Statistical-Analytics

A machine learning study evaluating and comparing classification models including a Boosted Random Forest architecture to predict clinical outcomes and recovery/mortality status for COVID-19 patients based on demographic and clinical feature


## 📌 Project Overview
- This project was completed as part of the **CLR204 Classification and Regression** coursework. It reproduces and expands upon clinical predictive modeling techniques (referencing study methodology by *Iwendi et al., 2020*) to assess patient mortality risk.
- By analyzing patient demographics, symptom timelines, geographical data, and health indicators, multiple classification algorithms were trained, tuned, and benchmarked to identify the most accurate model for clinical decision support.


## Acknowledgements & References
- **Original Dataset & Repository:**
Based on the work by Atharva Peshkar [Covid-19-Patient-Health-Analytics GitHub Repository](https://github.com/Atharva-Peshkar/Covid-19-Patient-Health-Analytics).
- **Research Methodology:** 
Iwendi, C., Bashir, A. K., Peshkar, A., et al. (2020). *COVID-19 patient health prediction using boosted random forest algorithm*. Frontiers in Public Health, 8, 357.


## Dataset source
####  The original dataset was taken from: https://www.kaggle.com/sudalairajkumar/novel-corona-virus-2019-dataset


## Key Technical Steps & Pipeline

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

## 📊 Results & Model Comparison

The evaluation metrics of the 5 machine learning models revealed that the **Boosted random forest** was the best ML model
<div align="center">
   
| Model | Accuracy | Precision | Recall | F1-Score |
| :--- | :---: | :---: | :---: | :---: |
| **Boosted Random Forest** | **0.89** | **0.75** | **0.82** | **0.78** |
| Support Vector Machine (SVM) | 0.82 | 0.67 | 0.67 | 0.67 |
| Logistic Regression | 0.84 | 0.67 | 0.73 | 0.69 |
| Decision Tree Classifier | 0.87 | 0.86 | 0.55 | 0.67 |
| Gaussian Naive Bayes | 0.78 | 0.54 | 0.64 | 0.58 |

</div>


<div align="center">
<img width="625" height="550" alt="comparison of various models performances" src="https://github.com/user-attachments/assets/6177e2da-13a4-4766-b721-2213a9f69b1b" />
</div>

## How to Run Locally

To explore or execute the notebooks on your local machine/operating system, follow these steps:

### 1. Clone the repository
```bash
git clone https://github.com/JMN-01/CLR204-Covid-19-Patient-Health-Statistical-Analytics.git
```
### 2. Install dependencies

Ensure you have Python installed, then install the required data science libraries:
```bash
pip install pandas numpy scikit-learn matplotlib jupyter
```
### 3. Launch Jupyter Notebook
```bash
jupyter notebook
```



