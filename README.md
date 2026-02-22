---

# Term Deposit Marketing: Predictive Analysis & Optimization

## 📌 Project Overview

In the competitive banking sector, term deposits are crucial for maintaining stable liquidity. This project focuses on analyzing and predicting customer responses to direct marketing campaigns (phone calls).

**The Goal:** Build a robust machine learning system to predict whether a customer will subscribe to a term deposit. By identifying high-potential customers, the bank can optimize its marketing resources, increase conversion rates, and reduce the number of unsuccessful calls.

## 📊 Dataset Description

The dataset consists of **40,000+ customer records** from a European banking institution.

* **Features:** Includes demographic data (age, job, marital status), financial data (balance, housing/personal loans), and campaign data (contact duration, number of contacts).
* **Target Variable (`y`):** Binary classification—Did the client subscribe? (`yes` or `no`).

## 🚀 Project Workflow

The project follows a standard Data Science lifecycle:

### 1. Exploratory Data Analysis (EDA)

* Analyzed class distribution (identified significant class imbalance).
* Visualized correlations between features like `duration`, `balance`, and the target variable.
* Explored demographic patterns (e.g., job types and education levels) to identify customer segments with higher conversion rates.

### 2. Data Preprocessing

* **Cleaning:** Handled outliers in numerical features (e.g., balance and duration) using statistical capping.
* **Encoding:** Transformed categorical variables (Job, Marital Status, Education, etc.) using  Label Encoding.


### 3. Handling Class Imbalance

* Since the majority of customers do *not* subscribe, the dataset was heavily imbalanced.
* Implemented **under sampling techniques (Synthetic Minority under-sampling Technique)** to balance the training set, ensuring the model learns the patterns of the "yes" class effectively.

### 4. Model Development & Selection

* Evaluated multiple classification algorithms:
* **Logistic Regression** (Baseline)
* **Random Forest**
* **KNeighbors Classifier**
* **SVC**
* **Decision Tree Classifier**


* Performed **Hyperparameter Tuning** using `OPTUNA` to optimize the F1-Score and Recall.

### 5. Model Evaluation

* **Primary Metric:** **Recall** and **F1-Score**. In marketing, missing a potential customer (False Negative) is often more costly than calling a non-interested one.
* Achieved a high **AUC-ROC** score, demonstrating the model's strong discriminatory power.

## 📈 Key Insights & Business Impact

* **Call Duration:** The strongest predictor of success. Customers who stay on the line longer are significantly more likely to subscribe.
* **Financial Health:** Customers with higher balances and no existing loans showed a higher propensity to invest in term deposits.
* **Optimization:** By using this model, the bank can prioritize the top 20% of customers most likely to convert, potentially capturing over 80% of total subscribers while reducing total calls by 50%.

## 🛠️ How to Use

1. **Clone the Repo:**
```bash
git clone https://github.com/Ch-Ibrahim/vJBdVG8NtiIf7R4J.git

```


2. **Install Dependencies:**
```bash
pip install pandas numpy scikit-learn matplotlib seaborn xgboost

```


3. **Run the Notebook:**
Open `Term Deposit Marketing Full Project.ipynb` in Jupyter or Google Colab to see the full analysis.

## 🎓 Concluding Remarks for Recruiters

This project demonstrates my ability to handle a **real-world end-to-end Machine Learning pipeline**. My contribution focused on:

* **Strategic Data Handling:** Not just running models, but addressing the real-world issue of class imbalance to prevent biased predictions.
* **Business-Centric Evaluation:** Choosing metrics (Recall/F1) that align with the banking industry's ROI goals rather than just looking at simple accuracy.
* **Actionable Analytics:** Translating complex model coefficients and feature importance into clear business recommendations for marketing teams.

I am passionate about using data to solve complex business problems and am looking for opportunities where I can apply these skills to drive growth.

---

*Created as part of the Apziva AI Residency Program.*
