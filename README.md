# Machine-Learning_DecisionTrees-LASSO-Boosting
# 🔷 Decision Trees, LASSO, and Boosting for Regression

## 🔶 Overview
This project focuses on **interpretable models** such as **decision trees**, as well as **regularized regression techniques** like **LASSO and Ridge regression**, and **boosting methods** for predictive modeling. The dataset includes **Acute Inflammations** and **Communities and Crime**, where we explore model interpretability, feature selection, and predictive performance.

---

## 🔷 Datasets Used
- [UCI Machine Learning Repository - Acute Inflammations](https://archive.ics.uci.edu/ml/datasets/Acute+Inflammations)
- **Acute Inflammations Dataset** 
  - Multi-label dataset for medical diagnosis.
  - Used to build **decision trees** and convert them into **IF-THEN rules**.

- [UCI Machine Learning Repository - Communities and Crime](https://archive.ics.uci.edu/ml/datasets/Communities+and+Crime)
- **Communities and Crime Dataset** 
  - Socio-economic and law enforcement data predicting crime rates.
  - Used to apply **linear models**, **Ridge regression**, **LASSO**, **Principal Component Regression (PCR)**, and **Boosting**.

---

## 🔷 Libraries Used
- `pandas` - Data manipulation and preprocessing.
- `numpy` - Numerical computations.
- `matplotlib` & `seaborn` - Data visualization.
- `sklearn.tree` - Decision tree modeling.
- `sklearn.linear_model` - LASSO, Ridge, and PCR.
- `xgboost` - Boosting models.
- `scipy` - Statistical analysis.

---

## 🔷 Steps Taken to Accomplish the Project

### 🔶 1. Decision Trees for Interpretability
- Built a **decision tree** on the **Acute Inflammations dataset**.
- Visualized the tree structure and extracted **IF-THEN rules**.
- Used **cost-complexity pruning** to improve interpretability.

### 🔶 2. Handling Missing Values and Feature Selection
- Applied **data imputation techniques** to handle missing values in **Communities and Crime dataset**.
- Dropped **non-predictive features** as per the dataset documentation.
- Computed **coefficient of variation (CV)** to rank features by importance.
- Selected **top √128 features** for further modeling.

### 🔶 3. Exploratory Data Analysis (EDA)
- Created a **correlation matrix** to identify relationships between variables.
- Generated **scatter plots** and **box plots** to analyze selected features.
- Examined **feature significance** based on distribution and spread.

### 🔶 4. Regression Modeling
- **Linear Regression**:
  - Trained on selected features and computed **test error**.
- **Ridge Regression**:
  - Optimized **λ (regularization strength)** using **cross-validation**.
  - Compared test errors with standard **linear regression**.
- **LASSO Regression**:
  - Identified **important features** by applying **L1 regularization**.
  - Evaluated model performance **with and without feature standardization**.

### 🔶 5. Principal Component Regression (PCR)
- Applied **Principal Component Analysis (PCA)** to reduce dimensionality.
- Selected **optimal number of components (M)** using **cross-validation**.
- Compared PCR test error with previous regression models.

### 🔶 6. Boosting for Regression
- Implemented **Gradient Boosting Trees** with **L1-penalized regression** at each node.
- Used **XGBoost** to fit the model and tuned **α (regularization term)** via cross-validation.
- Analyzed feature importance from the boosting model.

  ---
## 📌 **Note**
This repository contains a **Jupyter Notebook** detailing each step, along with **results and visualizations**.
