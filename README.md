# uber-demand-forecasting
End-to-end machine learning project to predict Uber ride demand using time-based features, lag variables, and Random Forest. Includes data preprocessing, feature engineering, and model evaluation.
# 🚖 Uber Demand Forecasting

## 📌 Overview

This project focuses on predicting Uber ride demand using machine learning techniques.
The goal is to model demand patterns based on time-based features and historical trends.

---

## 🎯 Problem Statement

Accurately predicting ride demand is crucial for:

* Optimizing driver allocation
* Reducing wait times
* Improving customer experience

---

## 📊 Dataset & Features

The dataset includes:

* ⏰ Hour of the day
* 📅 Day of the week
* 📆 Holidays / weekends
* 🔁 Lag features (previous demand values)
* 🌦️ (Planned) Weather data integration

---

## 🧠 Feature Engineering

Key transformations:

* Created **lag variables** to capture time dependencies
* Extracted **temporal features** (hour, weekday)
* Handled missing values and outliers
* Explored feature distributions using KDE plots
* Applied rolling mean features to smoothen the fluctuating trends 

---

## 🤖 Model Used

### Random Forest Regressor 
### XGBOOST

Why?

* Handles non-linearity well
* Robust to outliers
* Works well without heavy scaling
* XGBOOST is  much more robust and also has auto regularization

---

## ⚙️ Workflow

1. Data Cleaning
2. EDA performed (univariate and bivariate analysis)
3. Correlation tests
4. Feature Engineering
5. Train-Test Split
6. Model Training
7. Evaluation

---

## 📈 Results

* Model captures peak demand trends effectively
* Performs well on time-based variations

*(Add graphs here later)*
<img width="1330" height="961" alt="image" src="https://github.com/user-attachments/assets/ed7a6fab-b65f-4449-a4b7-65e1e4434322" />
<img width="580" height="432" alt="image" src="https://github.com/user-attachments/assets/eef44406-fe64-46d4-97ca-2b0f1f22bad0" /> 
Shows the extreme cases during holidays with the boxes representing the quartiles and the median and the extreme cases as the pickups 




---

## 🚀 Future Improvements

* 🔥 Integrate real-time weather API
* 📊 Deploy using Streamlit
* ⚡ Try XGBoost / LightGBM
* 📉 Hyperparameter tuning

---

## 🛠 Tech Stack

* Python
* Pandas, NumPy
* Scikit-learn
* Matplotlib / Seaborn

---

## 📌 How to Run

```bash
git clone https://github.com/YOUR_USERNAME/uber-demand-forecasting.git
cd uber-demand-forecasting
pip install -r requirements.txt
```

---

## 👨‍💻 Author

**Srijato Banerjee**
