# Student-Social-Media-Addiction-Prediction
# 📱 Student Social Media Addiction Prediction using XGBoost

This project analyzes student behavior data to predict social media addiction levels (Low, Moderate, High) using machine learning. The aim is to understand how digital habits—like daily usage, sleep, and mental health—relate to addiction patterns among students.

---

## 📊 Project Objective

- Explore and visualize patterns of social media usage among students.
- Predict addiction level using features such as:
  - Average Daily Usage Hours
  - Sleep Hours per Night
  - Mental Health Score
- Evaluate model performance using classification metrics and confusion matrix.

---

## 🧠 Technologies & Libraries

- Python (Pandas, NumPy, Matplotlib, Seaborn)
- Scikit-learn
- XGBoost
- Jupyter Notebook

---

## 🗂️ Dataset Overview

The dataset contains the following columns:

| Column                     | Description                                      |
|---------------------------|--------------------------------------------------|
| `Student_ID`              | Unique ID for each student                       |
| `Age`                     | Student age                                      |
| `Gender`                  | Gender                                           |
| `Academic_Level`          | Education level (e.g., High School, College)     |
| `Avg_Daily_Usage_Hours`   | Average hours spent on social media daily        |
| `Most_Used_Platform`      | Primary platform (Instagram, TikTok, etc.)       |
| `Sleep_Hours_Per_Night`   | Average sleep per night                          |
| `Mental_Health_Score`     | Self-reported mental health (scale 1–10)         |
| `Addicted_Score`          | Composite addiction score                        |
| `Addiction_Level`         | Classified label: Low, Moderate, High            |

---

## 📈 Exploratory Data Analysis (EDA)

- Histograms of daily usage and mental health
- Bar charts of most used platforms
- Box plots comparing gender-based usage
- Correlation heatmap of numeric features

> 🔍 **Insight**: Higher daily usage and lower sleep are strongly associated with higher addiction scores.

---

## 🤖 Model: XGBoost Classifier

- Target Variable: `Addiction_Level` (Low / Moderate / High)
- Features Used: 
  - `Avg_Daily_Usage_Hours`
  - `Sleep_Hours_Per_Night`
  - `Mental_Health_Score`

### 🔢 Model Accuracy: **91%**

### 📊 Classification Report:
| Class     | Precision | Recall | F1-score |
|-----------|-----------|--------|----------|
| High      | 93%       | 89%    | 91%      |
| Moderate  | 92%       | 93%    | 92%      |
| Low       | 82%       | 88%    | 85%      |

### 📉 Confusion Matrix
- Visual breakdown of model's predictions vs actual labels
- Most misclassifications occurred between adjacent classes (e.g., Low → Moderate)

---

## 🔍 Feature Importance

`Avg_Daily_Usage_Hours` and `Mental_Health_Score` were the most influential features in predicting addiction levels.
