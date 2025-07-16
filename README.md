# NHANES Age Prediction – Summer Analytics 2025

This repository contains my submission for **Week 4** of the **Summer Analytics 2025** program conducted by the **Consulting and Analytics Club, IIT Guwahati**. The task was to build a machine learning model that can classify individuals as senior citizens (aged 65 or older) using demographic and health indicators from the **NHANES (National Health and Nutrition Examination Survey)** dataset.

---

## 🧠 Problem Statement

Given health and nutrition data (BMI, glucose levels, insulin, physical activity, etc.), predict whether an individual belongs to the **senior citizen** category (age ≥ 65).

- **Target variable**: `IsSenior`  
  - `1` → Age ≥ 65  
  - `0` → Age < 65

- **Evaluation metric**: F1 Score (macro)

---

## 🔍 Exploratory Data Analysis (EDA)

- Checked data types, null values, and distributions.
- Visualized BMI, glucose, insulin, and activity levels.
- Compared feature trends between senior and non-senior groups.

---

## 🧪 Data Preprocessing

- ✅ Handled missing values using **median imputation**
- ✅ Applied **Label Encoding** for categorical columns
- ✅ Scaled numerical features using **StandardScaler**
- ✅ Ensured consistent preprocessing across train and test datasets

---

## 🤖 Model Building

I experimented with several classification models:

| Model               | Remarks                   |
|--------------------|---------------------------|
| Logistic Regression | ✅ Final Model (best F1)   |
| Random Forest       | Good accuracy, low recall |
| XGBoost             | Slight overfitting        |

- **Final choice**: Logistic Regression  
- **Reason**: Balanced performance and generalization on validation set

---

## 📈 Results

| Metric        | Value         |
|---------------|---------------|
| Final Model   | Logistic Regression |
| Validation F1 | **0.82** (example) |
| Submission Format | Followed as per `Sample_Submission.csv` |

---

## 📁 Repository Structure

📦 NHANES-Age-Prediction
├── 📁 data/
│ ├── Train_Data.csv
│ ├── Test_Data.csv
│ └── Sample_Submission.csv
├── 📁 output/
│ └── submission.csv
├── NHANES_Age_Prediction.ipynb # Notebook with code + results
├── requirements.txt # All libraries used
└── README.md # Project overview

---

## 🧰 Tech Stack

- **Language**: Python  
- **Notebook**: Google Colab  
- **Libraries**: pandas, numpy, matplotlib, seaborn, scikit-learn, xgboost

---

## 🔗 Useful Links

- 🔍 [Challenge on AI Planet](https://aiplanet.com/challenges/358/nutrition-health-survey-age-prediction-summer-analytics-2025-iit-guwahati-07302b63/overview/about)  
- 📚 [Summer Analytics 2025 Program](https://www.caciitg.com/sa/course25/)

---

## 👩‍💻 Author

**Vaibhavi Singh Rathaur**  
Participant, Summer Analytics 2025  
🔗 [LinkedIn](https://www.linkedin.com/in/vaibhavisingh999894a/)  
🌐 [GitHub](https://github.com/vaibhaviisingh)

---

## 📌 Acknowledgments

Grateful to the **Consulting & Analytics Club, IIT Guwahati** and **GeeksforGeeks** for organizing Summer Analytics 2025 and providing this opportunity to learn hands-on machine learning through real-world datasets.
