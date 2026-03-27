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

*(GRAPHS )*
<img width="1330" height="961" alt="image" src="https://github.com/user-attachments/assets/ed7a6fab-b65f-4449-a4b7-65e1e4434322" /> This is the correlation matrix heatmap of the features with the target 

<img width="580" height="432" alt="image" src="https://github.com/user-attachments/assets/eef44406-fe64-46d4-97ca-2b0f1f22bad0" /> 

Shows the extreme cases during holidays with the boxes representing the quartiles and the median and the extreme cases as the pickups 

<img width="1169" height="525" alt="image" src="https://github.com/user-attachments/assets/2b91fb55-1d2f-4fdc-974d-1fdbec6c3ac7" /> 
Shows trends in cases of extreme rainfall 

<img width="1169" height="525" alt="image" src="https://github.com/user-attachments/assets/e2448dfe-f0e9-40ca-9d2b-379f734d5e6f" /> 
Hourly pickup rates (showing lowest pickups during the 3rd to 5th hour)  

<img width="723" height="470" alt="image" src="https://github.com/user-attachments/assets/f5b8e5f6-c0d2-4bac-97da-70e4034cc528" />
Residuals vs predictions scatterplot for Random Forest regressor .. most values scattered around 0 showing the models arent biased and follows no specific trend 

<img width="585" height="455" alt="image" src="https://github.com/user-attachments/assets/d49835d1-1a91-4d4d-9ebe-3a8ee167c590" /> 
FINAL Q-Q plot of the model error (which represents the model performance) vs a theroretical noraml data .. plotting the data quantiles.. 
shows that model behaves fine and good for normal and data lying in the mid range.. and has errors that is pickups in the extreme range  for too small values or too large values 
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
