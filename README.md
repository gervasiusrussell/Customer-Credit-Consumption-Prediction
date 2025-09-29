# 💳 Customer Credit Consumption Prediction

## 📖 Project Overview

This repository contains a **machine learning regression project** designed to predict customer credit card consumption (`cc_cons`) based on customer demographics, behavior, and credit usage patterns.

The project demonstrates the **end-to-end ML pipeline**:

* Data integration from multiple sources
* Exploratory Data Analysis (EDA)
* Data preprocessing and feature engineering
* Outlier detection and handling
* Feature selection with Random Forests
* Model training and evaluation (Random Forest Regressor)

---

## ⚙️ Technologies Used

* **Python 3**
* **Jupyter Notebook**
* **Pandas, NumPy** – Data manipulation and preprocessing
* **Matplotlib, Seaborn** – Visualization and EDA
* **SciPy** – Statistical analysis (normality tests, correlation)
* **Scikit-learn** – Preprocessing, feature selection, modeling, metrics
* **mlxtend** – Sequential Feature Selector (optional)

---

## 📊 Workflow

1. **Data Loading & Integration**

   * Merge **Customer Demographics**, **Customer Behavior**, and **Credit Consumption** datasets on unique `ID`.

2. **Exploratory Data Analysis (EDA)**

   * Dataset structure, missing values, duplicates
   * Distribution checks (histograms, boxplots)
   * Normality test with `scipy.stats.normaltest`
   * Correlation analysis with Spearman’s rank correlation

3. **Preprocessing & Feature Engineering**

   * Label encoding for categorical variables (`account_type`, `gender`, `Income`)
   * Dropping redundant/irrelevant features (`loan_enq`, quasi-constant features)
   * Handling outliers with **Winsorization (5%)**
   * Log-transform of target variable `cc_cons` for normalization

4. **Feature Selection**

   * Removed quasi-constant features using **VarianceThreshold**
   * Feature importance ranking via **Random Forest Regressor**

5. **Modeling**

   * **Random Forest Regressor** trained on selected features
   * Evaluated on train-test split (80-20)

6. **Evaluation Metrics**

   * **Mean Squared Error (MSE)**
   * **Mean Absolute Error (MAE)**
   * **R² Score**

---

## 🚀 How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/<your-username>/<repo-name>.git
   cd <repo-name>
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Launch Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

---

## 📈 Results

* Random Forest achieved promising results with:

  * **MSE:** (to be filled after training)
  * **MAE:** (to be filled after training)
  * **R² Score:** (to be filled after training)
* Top 10 most important features were identified, providing insights into key drivers of credit consumption.

---

✍️ **Author**: Gervasius Russell
🎓 **Major**: Data Science, BINUS University
