# Project Overview

## 📌 Problem Statement

With the growing demand for laptops and dynamic pricing in the e-commerce market, it's crucial to understand the factors that influence laptop prices. This project aims to build an accurate regression model to **predict laptop prices** based on key specifications like **RAM, Processor, Resolution, and Screen Size**.

---

## 🎯 Objective

To predict laptop prices using the following features:
- **RAM (GB):** Amount of memory in gigabytes  
- **Resolution:** Screen resolution (e.g., 1920x1080)  
- **Processor:** Processor type (e.g., Intel i5, AMD Ryzen)  
- **Screen Size (inch):** Laptop display size in inches  

---

## 🧭 Project Workflow

### 1️⃣ Summary Statistics
- Computed central tendency, spread, and distribution of each feature to understand data characteristics.

### 2️⃣ Data Preprocessing
- Handled missing values and outliers
- Applied **categorical encoding** to the `Processor` feature
- Scaled numerical variables where required

### 3️⃣ Exploratory Data Analysis (EDA)
- **Univariate Analysis:** Distribution of individual features  
- **Bivariate Analysis:** Relationship between features and target (Price)  
- **Multivariate Analysis:** Interaction between multiple features  
- **Correlation Matrix:** Visualized correlations to detect multicollinearity  

### 4️⃣ Feature Importance

| Feature             | Importance (%) |
|---------------------|----------------|
| RAM (GB)            | 47.24%         |
| Processor           | 26.42%         |
| Resolution          | 24.21%         |
| Screen Size (inch)  | 2.11%          |

> 📌 *RAM and Processor are the most influential factors in predicting laptop prices.*

### 5️⃣ Model Building and Evaluation
- Implemented 3 regression models:
  - ✅ **Random Forest**
  - ✅ **XGBoost**
  - ✅ **K-Nearest Neighbors (KNN)**
- Used **GridSearchCV** for hyperparameter tuning
- Evaluated using **R² score** and **Root Mean Squared Error (RMSE)**

---

## 📊 Model Performance

| Model         | Train R² (%) | Test R² (%) | Train RMSE | Test RMSE |
|---------------|--------------|-------------|------------|-----------|
| Random Forest | 84.13        | 80.63       | 522.95     | 583.80    |
| XGBoost       | 84.46        | 80.85       | 517.60     | 582.52    |
| KNN           | 83.74        | 80.10       | 529.44     | 593.83    |

> ✅ **XGBoost** outperformed other models with the best balance of training and test performance.

---

## 💡 Key Takeaways

- RAM (GB) and Processor are the most influential features for predicting laptop prices.
- XGBoost outperformed other models, making it the best choice for this problem.
- The model can help customers and retailers make data-driven pricing decisions.


