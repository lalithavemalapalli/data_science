# Credit Card Consumption Prediction

## Problem Statement

Banks have transactional and demographic data for 20,000 customers, but credit card consumption (`cc_cons`) is unavailable for a subset of customers. The objective of this project is to analyze customer behavior and build a machine learning model that predicts credit card consumption using demographic, behavioral, and transactional features.

---

## Dataset

| File                       | Description                                                                |
| -------------------------- | -------------------------------------------------------------------------- |
| CustomerDemographics.xlsx  | Customer age, gender, income, occupation, and demographic details          |
| CustomerBehaviorData.xlsx  | Credit/debit transactions, investments, EMI, loans, and banking activities |
| CreditConsumptionData.xlsx | Credit card consumption values (`cc_cons`)                                 |

### Dataset Summary

* Total Customers: 20,000
* Total Features After Merging: 50+
* Target Variable: `cc_cons`
* Problem Type: Regression

---

## Project Objectives

* Analyze customer spending behavior.
* Identify factors affecting credit card consumption.
* Perform exploratory data analysis (EDA).
* Create meaningful business insights.
* Build machine learning models to predict customer spending.

---

## Project Workflow

### 1. Data Merging & Preprocessing

* Merged all datasets using Customer ID.
* Handled missing values.
* Removed duplicates.
* Corrected data types.

**Notebook:** `data_merging_preprocessing.ipynb`

---

### 2. Exploratory Data Analysis (EDA)

Performed analysis on:

* Customer demographics
* Income distribution
* Spending patterns
* Transaction behavior
* Investment trends
* Loan analysis

Visualizations:

* Histograms
* Bar Charts
* Scatter Plots
* Correlation Heatmaps

**Notebook:** `eda_analysis.ipynb`

---

### 3. Feature Engineering

Created new features such as:

* Total Credit Card Spend
* Total Debit Card Spend
* Total Transactions
* Total Investments
* Customer Spending Metrics

**Notebook:** `feature_engineering.ipynb`

---

### 4. Machine Learning Modeling

Models Implemented:

| Model                   | Purpose               |
| ----------------------- | --------------------- |
| Linear Regression       | Baseline Model        |
| Decision Tree Regressor | Non-linear Prediction |
| Random Forest Regressor | Ensemble Learning     |

**Notebook:** `ml_modeling.ipynb`

---

## Model Evaluation

| Model             | R² Score |
| ----------------- | -------- |
| Linear Regression | 0.6590      |
| Decision Tree     | 0.3121      |
| Random Forest     | 0.6509      |


---

## Technologies Used

### Programming

* Python

### Libraries

* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn

### Visualization

* Power BI

### Development Tools

* Jupyter Notebook
* VS Code
* GitHub

---

## Key Business Insights

* Customers with higher income generally spend more on credit cards.
* Transaction frequency strongly influences credit card consumption.
* Investment behavior correlates with spending patterns.
* Certain customer segments contribute significantly to overall revenue.
* Banking activity can be used to predict future customer spending.

---

## Power BI Dashboard

Dashboard includes:

* Customer Overview
* Spending Analysis
* Transaction Analysis
* Demographic Insights
* Machine Learning Predictions

---

## How to Run

Install required libraries:

```bash
pip install -r requirements.txt
```

Run notebooks in the following order:

```text
1. data_merging_preprocessing.ipynb
2. eda_analysis.ipynb
3. feature_engineering.ipynb
4. ml_modeling.ipynb
```

---

## Project Outcome

Successfully analyzed customer behavior and developed a machine learning model to predict credit card consumption. The project demonstrates skills in data cleaning, exploratory data analysis, feature engineering, machine learning, and business intelligence visualization.

