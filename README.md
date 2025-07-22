# 🩺 Heart Attack Risk Prediction

[![Made with 💻 Colab](https://img.shields.io/badge/Made%20With-Colab-yellow?style=for-the-badge&logo=googlecolab)](https://colab.research.google.com/github/aashwika25/Risk-Of-Heart-Disease-Prediction-Models/blob/main/Risk_Of_Heart_Disease_in_Patients_Aashwika.ipynb)
[![Python](https://img.shields.io/badge/Python-3.10-purple?style=for-the-badge&logo=python)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge)](LICENSE)
[![Open Issues](https://img.shields.io/github/issues/aashwika25/Risk-Of-Heart-Disease-Prediction-Models?style=for-the-badge)](https://github.com/aashwika25/Risk-Of-Heart-Disease-Prediction-Models/issues)


---

### 👩‍💻 Created by [Aashwika Khurana](https://github.com/aashwika25)

This notebook analyzes the Heart Attack Prediction dataset using a structured machine learning pipeline. Multiple models—Logistic Regression, Random Forest (baseline and tuned), and Gradient Boosting—are trained and evaluated to compare predictive performance.

---

## 💡 Dataset Overview

- Dataset: `heart_attack_prediction_dataset.csv.zip`  
- Target: `Heart Attack Risk` (0 = Low Risk, 1 = High Risk)  
- Includes numerical and categorical features  
- No missing values detected

---

## 🧼 Preprocessing Pipeline

- One-Hot Encoding for categorical variables  
- Feature scaling with StandardScaler  
- Train-test split with 70%-30% ratio, stratified on target

---

## 📊 Data Visualizations

- Correlation heatmap  
- Histograms for feature distributions  
- Boxplots for outlier detection  
- Bar chart of target class distribution

---

## 🤖 Models Applied

| Model                    | Accuracy | Pros                                                  | Cons                                |
|-------------------------|----------|--------------------------------------------------------|-------------------------------------|
| Logistic Regression      | ~48%     | Fast, interpretable, baseline for binary classification | Poor for nonlinear relationships    |
| Baseline Random Forest   | ~64%     | Handles complex patterns, robust to noise              | May overfit without tuning          |
| Gradient Boosting        | ~67%     | Efficient performance with fewer trees                 | Longer training time                |
| Tuned Random Forest      | ~70%+    | Optimized via RandomizedSearchCV, strongest results    | More computationally intensive      |

All models were evaluated using:
- ✅ Accuracy Score  
- ✅ Confusion Matrix (heatmap)  
- ✅ Classification Report (precision, recall, F1-score)

---

## 📈 Feature Importance

Top 15 features by importance (from tuned Random Forest):

![Feature Importance](images/feature_importance.png)

---

## 📌 Open in Colab

Launch the notebook directly in Google Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/aashwika25/Risk-Of-Heart-Disease-Prediction-Models/blob/main/Risk_Of_Heart_Disease_in_Patients_Aashwika.ipynb)

---

## 📦 Requirements

```txt
pandas  
numpy  
matplotlib  
seaborn  
scikit-learn  
tabulate
These libraries cover preprocessing, visualization, modeling, and performance comparison.
```
---
## 📄 License
This project is licensed under the MIT License.

---
## 🤝 Contributions Welcome
Have ideas to optimize performance, add more insights, or deploy this into a web app? You're welcome to contribute!

Steps to get started:
- 🔱 Fork the repo
- ✍️ Create a feature branch
- 📮 Submit a pull request
