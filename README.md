

# Task 1 – Basics of Data Analytics (Sales Data Analysis)

## Getting Started
To get started with the project, clone the repository and open the notebook.


git clone https://github.com/yourusername/sales-intelligence.git
cd sales-intelligence


Install the required dependencies:


pip install -r requirements.txt


Open the Jupyter Notebook:


jupyter notebook Task1_Regression.ipynb



##  Objective

Analyse retail sales data using **linear algebra** and **regression techniques** to identify **trends**, **patterns**, and **predict future sales**.

---

##  Dataset

* **Source:** `Sales_data.csv`
* **Records:** ≥ 200
* **Key Fields:**

  * `Date`
  * `Sales Amount`
  * `Number of Products Sold`
  * `Marketing Expenditure`
  * `Region`

---

##  Process

### **1. Data Preparation**

* Converted `Date` to datetime format
* Checked and handled missing values
* Sorted data by date

### **2. Exploratory Data Analysis (EDA)**

* **Sales Trend:** Time series plot to visualize sales over time
* **Regional Sales:** Bar chart showing total sales by region
* **Correlation:** Heatmap to identify relationships between:

  * Sales Amount
  * Marketing Expenditure
  * Number of Products Sold

### **3. Modelling**

* **Features (X):**

  * `Marketing Expenditure`
  * `Number of Products Sold`
* **Target (y):**

  * `Sales Amount`
* **Model:**

  * Multiple Linear Regression (`scikit-learn`)
* **Evaluation Metrics:**

  * Mean Squared Error (MSE)
  * R² Score

---

##  Results

* **Strong positive correlation** between marketing expenditure, products sold, and sales amount
* Model achieved a **good R² score**, indicating strong predictive capability

---

## 🛠 Tools & Libraries

* **Python**
* **pandas**
* **numpy**
* **matplotlib**
* **seaborn**
* **scikit-learn**

---

##  Conclusion

The regression model provides **insights into factors influencing sales** and can be used for **forecasting** and **optimizing marketing budgets**.

---

# Task 2 – Statistical Decision Making

##  Objective

Analyse production data to identify **factors influencing product quality** using statistical techniques.

---

##  Process

* **Clean and prepare the dataset**
  Removed missing or inconsistent values, standardized column formats.
* **Explore trends and distributions**
  Used descriptive statistics, histograms, and boxplots to understand data spread and detect outliers.
* **Perform statistical tests**

  * **ANOVA** for comparing means across multiple groups.
  * **t-tests** for comparing means between two groups.
* **Fit regression models**
  Built statistical models to quantify relationships between predictors and product quality.
* **Evaluate assumptions and diagnostics**
  Checked for normality, homoscedasticity, and multicollinearity.
* **Suggest strategies for improving quality**
  Provided actionable recommendations based on significant factors.

---

##  Tools & Libraries

* **Python**
* **pandas**
* **numpy**
* **matplotlib**
* **seaborn**
* **scipy**
* **statsmodels**

---

##  Conclusion

Statistical analysis identified key variables that significantly affect product quality.
Findings can be applied to **optimize production processes** and **reduce defect rates**.




