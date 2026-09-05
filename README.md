# Insurance Charges Prediction using Machine Learning

## 📌 Project Overview

This project predicts medical insurance charges using machine learning regression algorithms.

The project compares multiple models and identifies the best-performing model based on MAE, RMSE, and R² score.

---

## 🎯 Objectives

- Predict medical insurance charges using customer information
- Preprocess numerical and categorical features
- Train multiple regression models
- Compare model performance
- Select the best-performing model

---

## 📊 Dataset & Features

The dataset contains information about individuals and their medical insurance charges.

| Feature | Description |
|---|---|
| `age` | Age of the individual |
| `sex` | Gender of the individual |
| `bmi` | Body Mass Index |
| `children` | Number of children/dependents |
| `smoker` | Smoking status |
| `region` | Residential region |
| `charges` | Medical insurance charges — target variable |

---

## ⚙️ Data Preprocessing

The target variable `charges` is separated from the input features. Categorical features are converted using One-Hot Encoding, while numerical features are standardized using StandardScaler. The dataset is then divided into training and testing sets using an 80/20 split.

---

## 🤖 Models Used

The following regression models were trained and compared:

- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor
- Gradient Boosting Regressor
- XGBoost Regressor
- Tuned XGBoost Regressor

---

## 📈 Model Comparison

| Model | MAE | RMSE | R² Score |
|---|---:|---:|---:|
| Linear Regression | 4181.19 | 5796.28 | 0.7836 |
| Decision Tree | 3114.15 | 6387.12 | 0.7372 |
| Random Forest | 2549.01 | 4572.84 | 0.8653 |
| Gradient Boosting | 2454.47 | 4335.04 | 0.8790 |
| XGBoost | 2440.07 | 4254.78 | 0.8834 |
| Tuned XGBoost | **2369.99** | **4244.56** | **0.8840** |

---

## 🏆 Final Model

The **Tuned XGBoost Regressor** achieved the best overall performance.

- **MAE:** 2369.99
- **RMSE:** 4244.56
- **R² Score:** 0.8840

The model explains approximately **88.4% of the variation** in medical insurance charges on the test dataset.

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Jupyter Notebook

---

## 📁 Project Structure

```text
Insurance-Charges-Prediction/
│
├── insurance.csv
├── insurance_charges_prediction.ipynb
├── README.md
└── requirements.txt
