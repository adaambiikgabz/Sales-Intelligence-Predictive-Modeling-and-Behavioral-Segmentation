

````markdown
# Sales Intelligence Project

## Getting Started
To get started with the project, clone the repository and open the notebook.

```bash
git clone https://github.com/yourusername/sales-intelligence.git
cd sales-intelligence
````

Install the required dependencies:

```bash
pip install -r requirements.txt
```

Open the Jupyter Notebooks:

```bash
jupyter notebook
```



# Task 1 – Basics of Data Analytics (Sales Data Analysis)

## Objective

Analyse retail sales data using **linear algebra** and **regression techniques** to identify **trends**, **patterns**, and **predict future sales**.

## Dataset

* **Source:** `Sales_data.csv`
* **Records:** ≥ 200
* **Key Fields:**

  * `Date`
  * `Sales Amount`
  * `Number of Products Sold`
  * `Marketing Expenditure`
  * `Region`

## Process

### 1. Data Preparation

* Converted `Date` to datetime format
* Checked and handled missing values
* Sorted data by date

### 2. Exploratory Data Analysis (EDA)

* **Sales Trend:** Time series plot to visualize sales over time
* **Regional Sales:** Bar chart showing total sales by region
* **Correlation:** Heatmap to identify relationships between:

  * Sales Amount
  * Marketing Expenditure
  * Number of Products Sold

### 3. Modelling

* **Features (X):**

  * `Marketing Expenditure`
  * `Number of Products Sold`
* **Target (y):**

  * `Sales Amount`
* **Model:** Multiple Linear Regression (`scikit-learn`)
* **Evaluation Metrics:**

  * Mean Squared Error (MSE)
  * R² Score

## Results

* **Strong positive correlation** between marketing expenditure, products sold, and sales amount
* Model achieved a **good R² score**, indicating strong predictive capability

## Tools & Libraries

* Python
* pandas
* numpy
* matplotlib
* seaborn
* scikit-learn

## Conclusion

The regression model provides **insights into factors influencing sales** and can be used for **forecasting** and **optimizing marketing budgets**.



# Task 2 – Statistical Decision Making

## Objective

Analyse production data to identify **factors influencing product quality** using statistical techniques.

## Process

* **Clean and prepare the dataset** – removed missing or inconsistent values, standardized column formats.
* **Explore trends and distributions** – descriptive statistics, histograms, and boxplots to understand spread and detect outliers.
* **Perform statistical tests:**

  * **ANOVA** – comparing means across multiple groups
  * **t-tests** – comparing means between two groups
* **Fit regression models** – statistical models to quantify relationships between predictors and product quality
* **Evaluate assumptions and diagnostics** – checked normality, homoscedasticity, multicollinearity
* **Suggest strategies for improving quality** – provided actionable recommendations based on significant factors

## Tools & Libraries

* Python
* pandas
* numpy
* matplotlib
* seaborn
* scipy
* statsmodels

## Conclusion

Statistical analysis identified key variables that significantly affect product quality.
Findings can be applied to **optimize production processes** and **reduce defect rates**.

---

# Task 3 – Fraud Detection with Machine Learning

## Objective

Build a **fraud detection system** using supervised machine learning models to classify transactions as **fraudulent** or **legitimate**.

## Dataset

* **Source:** `synthetic_fraud_dataset.csv`
* **Records:** \~500
* **Key Fields:**

  * `transaction_id`
  * `amount`
  * `transaction_type`
  * `location`
  * `device`
  * `is_fraud` (target variable: 0 = legitimate, 1 = fraud)

## Process

### 1. Data Preparation

* Dropped irrelevant fields (e.g., `transaction_id`)
* Encoded categorical variables (`transaction_type`, `location`, `device`) using **LabelEncoder**
* Scaled numerical values (`amount`) with **StandardScaler**

### 2. Modelling

* **Features (X):**

  * Transaction amount
  * Transaction type
  * Location
  * Device
* **Target (y):**

  * Fraud label (`is_fraud`)
* **Models Tested:**

  * Logistic Regression
  * Random Forest Classifier
* **Evaluation Metrics:**

  * Accuracy
  * Precision
  * Recall
  * F1-score
  * ROC-AUC

### 3. Model Deployment

* Saved the trained Random Forest model as `fraud_detection_model.pkl` using **joblib**

## Results

* Logistic Regression – provided baseline performance
* Random Forest – achieved **higher recall** and **better F1-score**, making it more suitable for fraud detection where catching fraudulent cases is critical
* ROC-AUC indicated strong discriminatory power

## Tools & Libraries

* Python
* pandas
* numpy
* scikit-learn
* joblib

## Conclusion

The fraud detection model successfully classified fraudulent transactions with **high accuracy and recall**.
This system can be integrated into **real-time fraud monitoring pipelines** for financial services.



# Overall Project Takeaways

* **Task 1:** Regression for sales forecasting → helped optimize marketing spend
* **Task 2:** Statistical tests for quality improvement → informed production strategies
* **Task 3:** Machine learning for fraud detection → built predictive fraud monitoring system

The project demonstrates how **data analytics + statistical decision making + machine learning** can solve **real-world business problems** across multiple domains.




