# Car Price Prediction 🚗  
**Machine Learning Regression Project**

## 📌 Project Overview
This project focuses on building a **machine learning–based system to predict used car prices**
using real-world vehicle listing data.  
Car pricing depends on multiple factors such as **vehicle age, mileage, fuel type, transmission,
and brand**, making manual estimation difficult.

The goal of this project is to develop a **robust regression pipeline** that accurately predicts
car prices and identifies the most influential factors affecting pricing decisions. :contentReference[oaicite:0]{index=0}

---

## 🗂️ Repository Structure
- `honda_car_selling.csv` – Dataset containing used car listings  
- `Car_Price_Prediction.ipynb` – Jupyter Notebook with EDA, preprocessing & modeling  
- `Car_Price_Prediction_Report.pdf` – Detailed academic project report  

---

## 🧠 Problem Statement
Estimating used car prices manually is:
- subjective
- inconsistent
- prone to market bias  

This project uses **machine learning regression models** to automate and standardize
price prediction based on historical data.

---

## 🛠️ Tools & Technologies
- **Python 3.9**
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

---

## 🔍 Methodology
The project follows a complete ML workflow:

### 1️⃣ Data Preprocessing
- Cleaned numeric columns (Price, Kms Driven)
- Handled missing values using:
  - Median imputation (numerical)
  - Mode imputation (categorical)
- Removed outliers using **IQR method**

### 2️⃣ Feature Engineering
- Vehicle **Age** derived from Year
- Log transformation of Kms Driven
- High Mileage indicator
- One-hot encoding for categorical features
- Feature scaling using `StandardScaler`

### 3️⃣ Exploratory Data Analysis (EDA)
- Distribution analysis
- Outlier visualization
- Feature impact on price

---

## 🤖 Machine Learning Models Used
The following regression models were implemented and compared:

1. Linear Regression  
2. Ridge Regression  
3. Lasso Regression  
4. Random Forest Regressor  
5. HistGradientBoosting Regressor  

---

## 📊 Model Evaluation
- Train-test split: **80% / 20%**
- 5-fold Cross Validation
- Evaluation metrics:
  - MAE
  - MSE
  - RMSE
  - R² Score

**Best Performing Models:**
- Random Forest Regressor
- Gradient Boosting Regressor

These models performed best due to their ability to capture **non-linear relationships**
in pricing data. :contentReference[oaicite:1]{index=1}

---

## 📈 Key Insights
- Vehicle **age and mileage** have the strongest impact on price
- Fuel type and transmission significantly influence resale value
- Linear models provide a baseline but fail to capture complex patterns
- Ensemble models generalize better on real-world data

---

## 🚀 How to Run the Project
1. Clone the repository
   ```bash
   git clone https://github.com/your-username/car-price-prediction.git
