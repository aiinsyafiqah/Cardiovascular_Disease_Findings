# Cardiovascular Disease Prediction Using Machine Learning

## 📌 Project Overview

This project explores the use of **Machine Learning techniques to predict cardiovascular disease** based on patient health-related features.

The project was developed as part of **BIT 34303 – Machine Learning** at the Faculty of Computer and Information Technology, Universiti Tun Hussein Onn Malaysia (UTHM).

The analysis focuses on understanding the dataset, preprocessing the data, identifying important features, and comparing several machine learning models to determine which model provides the most reliable prediction performance.

---

## 🎯 Objectives

The main objectives of this project are to:

* Analyze the Cardiovascular Disease dataset.
* Identify and handle irrelevant or abnormal data.
* Explore the relationship between different health-related features and cardiovascular disease.
* Investigate which features have the greatest impact on cardiovascular disease prediction.
* Train and compare multiple machine learning models.
* Evaluate model performance using **Accuracy** and **F1 Score**.

---

## 📊 Dataset

The project uses the **Cardiovascular Disease Dataset** obtained from Kaggle.

**Dataset:** Cardiovascular Disease Dataset
**Source:** Kaggle – sulianova/cardiovascular-disease-dataset

The dataset was imported into **Google Colab** for analysis and model development. The initial analysis showed that the dataset contained **no null values**.

---

## 🔍 Data Preprocessing

Although there were no missing values, the dataset contained some abnormal blood pressure readings.

The `ap_lo` (diastolic blood pressure) column contained values ranging from **-150 to 16020**, which were considered irrelevant or unrealistic for the analysis.

To improve the quality of the dataset:

* Negative blood pressure values were removed.
* The maximum blood pressure value was restricted to **250**.
* Boxplots were used to examine the blood pressure distribution before and after cleaning.

These preprocessing steps helped reduce the effect of unrealistic blood pressure values on the machine learning models.

---

## 🧪 Feature Engineering

Three types of input features were explored to investigate their potential relationship with cardiovascular disease:

### 1. BMI

The analysis examined the relationship between **Body Mass Index (BMI)** and cardiovascular disease.

### 2. Age Group

Patients were grouped based on age to investigate how age-related differences were associated with cardiovascular disease.

### 3. Pulse Pressure

The distribution of **pulse pressure** was also analyzed to investigate its relationship with cardiovascular disease.

These analyses were used to better understand how different patient characteristics may contribute to the prediction task.

---

## 📈 Correlation Analysis

A **correlation heatmap** was used to investigate the relationships between the features and cardiovascular disease.

This analysis provided an overview of how the different variables were related to each other and to the target cardiovascular disease variable.

---

## 🌳 Feature Importance

Feature importance was evaluated using both:

* **Random Forest**
* **Decision Tree**

The results showed that **BMI was identified as the highest-impact factor** affecting cardiovascular disease in both model-based feature importance analyses.

This suggests that BMI was an important feature within the dataset for the models used in this project.

---

## 🤖 Machine Learning Models

Four machine learning algorithms were compared:

| Model               | Performance     |
| ------------------- | --------------- |
| Decision Tree       | 🥇 Best overall |
| Logistic Regression | 🥈 Second       |
| Random Forest       | 🥉 Third        |
| Naïve Bayes         | Lowest          |

The models were evaluated using:

* **Accuracy Score**
* **F1 Score**

Based on the final comparison, the **Decision Tree model achieved the most reliable and accurate results**, followed by Logistic Regression and Random Forest. Naïve Bayes produced the lowest F1 score among the models evaluated.

---

## 🏆 Key Findings

The main findings from this project were:

1. The dataset initially contained **no missing values**.
2. Abnormal blood pressure values were identified and cleaned during preprocessing.
3. BMI, age group, and pulse pressure were explored as potential factors related to cardiovascular disease.
4. **BMI was identified as the most important feature** in both Random Forest and Decision Tree feature importance analysis.
5. Among the four tested models, **Decision Tree achieved the best overall performance** based on the project's accuracy and F1 score comparison.
6. **Naïve Bayes had the lowest F1 score** among the models tested.

---
## Results / Visualization 

1. Heatmap correlation figure shows how each of the categories effects on the other cardio disease. 
<img width="916" height="836" alt="heatmap correlation result" src="https://github.com/user-attachments/assets/c2880310-e704-4dd7-8598-23913350f3c1" />

2. Figure shows how Random Forest Classifier Model predict the Healthy and Sick People
<img width="683" height="547" alt="Matrix Confusion_Random Forest" src="https://github.com/user-attachments/assets/fb448956-b566-4da7-bc8b-bddc94527fff" />

3. Findings shows that whether using Random Forest or Decision Tree Model both conclude that BMI is the main factor
of affecting heart disease.

### Feature Importance of Random Forest 
<img width="904" height="547" alt="Feature Importance_Random Forest" src="https://github.com/user-attachments/assets/d739da2b-b91e-40a8-9a12-d6d15a18f7b8" />

### Feature Importance of Decision Tree
<img width="904" height="547" alt="feature Importance_Decision Tree" src="https://github.com/user-attachments/assets/9929889a-ea81-4b39-b7e6-cbdc2ba0f459" />

4. Overall results using F1-Score vs Accuracy
In medical problems, the F1-Score is more important than accuracy because it balances precision for not marking healthy people as sick and recall means not missing sick patients. A higher F1-Score means the model is better at correctly finding patients with heart disease while still being accurate.

<img width="841" height="525" alt="Accuracy vs F1 Final Result" src="https://github.com/user-attachments/assets/62b5a2ff-946b-4e0a-a65c-c0592fb3c1d1" />

---
## 🛠️ Technologies Used

* **Python**
* **Google Colab**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Seaborn**
* **Scikit-learn**
* **Jupyter Notebook (`.ipynb`)**

---

## 📂 Project Structure

```text
cardiovascular-disease-prediction/
│
├── README.md
├── cardiovascular_disease.ipynb
└── dataset/
    └── cardiovascular_disease.csv
```

> The dataset may not be included in this repository depending on its licensing and redistribution conditions.

---

## 📚 Academic Context

**Course:** BIT 34303 – Machine Learning
**Project:** Group Project 2 – Full Result of Cardiovascular Disease
**Institution:** Universiti Tun Hussein Onn Malaysia (UTHM)

### 👥 Project Team

* Nur Ain Syafiqah Binti Nor Azlan
* Nur Syahindah Afiqah Binti Yusaidi
* Uthman Bin Hasfizal
* Syed Mohamad Zharfan Bin Syed Robart

---

## 💡 Conclusion

This project demonstrates how machine learning can be applied to a cardiovascular disease dataset through **data preprocessing, exploratory analysis, feature engineering, feature importance analysis, and predictive modelling**.

The comparison of multiple algorithms showed that the **Decision Tree model provided the strongest overall performance for this dataset**, while BMI was identified as an important feature in the model-based feature importance analysis.

The project provided practical experience in applying machine learning techniques to a real-world healthcare-related dataset and evaluating different models based on their predictive performance.
