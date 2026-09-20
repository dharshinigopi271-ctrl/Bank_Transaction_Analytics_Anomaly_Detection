# 🏦 Bank Transaction Analytics and Anomaly Detection Using Machine Learning

## 📌 Project Overview

This project focuses on analyzing bank transaction data and identifying **unusual transaction patterns** using Machine Learning.

The project uses the **Isolation Forest** algorithm for unsupervised anomaly detection. The complete workflow includes data cleaning, Exploratory Data Analysis (EDA), feature engineering, feature scaling, anomaly detection, visualization, business insights, and deployment using **Streamlit**.

> **Note:** An anomaly does not automatically mean fraud. It indicates that a transaction has characteristics that differ from the patterns learned from the available data and may require further investigation.

---

## 🎯 Project Objectives

* Analyze bank transaction records
* Clean and preprocess transaction data
* Perform Exploratory Data Analysis (EDA)
* Create meaningful transaction features
* Scale features for Machine Learning
* Detect unusual transactions using Isolation Forest
* Analyze and visualize detected anomalies
* Generate business-oriented insights
* Deploy the Machine Learning model using Streamlit

---

## 📊 Dataset

The project uses bank account transaction records containing fields such as:

* **Date**
* **Description**
* **Withdrawal (Dr.)**
* **Deposit (Cr.)**
* **Balance**
* **Reference Number**

The dataset contains both **debit and credit transactions**, allowing different transaction behaviors to be analyzed.

---

## 🔍 Exploratory Data Analysis

The project performs EDA to understand transaction behavior, including:

* Debit vs. Credit transaction distribution
* Monthly transaction amounts
* Frequently occurring transaction descriptions
* Account balance distribution
* Transaction amount distribution
* Correlation analysis
* Year-wise transaction analysis

---

## 🛠️ Data Cleaning & Feature Engineering

The transaction data is processed and transformed into machine-learning-ready features.

### Features created include:

* Transaction Amount
* Transaction Type
* Month
* Quarter
* Is Weekend
* High Value Transaction
* Balance Difference
* Transaction Amount Category

These features help represent transaction behavior more effectively for anomaly detection.

---

## 🤖 Machine Learning Model

### Isolation Forest

The project uses **Isolation Forest**, an unsupervised Machine Learning algorithm designed to identify observations that differ from the majority of the dataset.

The model produces two types of results:

```text
Normal
Anomaly
```

Anomaly detection is useful when reliable fraud labels are not available.

---

## 📈 Anomaly Detection

The processed transaction data is passed through the Isolation Forest model.

The model identifies transactions that are unusual compared with the learned transaction patterns.

The project includes visualizations such as:

* Normal vs. Anomalous Transactions
* Anomaly Distribution
* Anomaly Visualization
* Monthly Anomaly Count

---

## 💡 Business Insights

The project can help analysts investigate questions such as:

* Which transactions appear unusual?
* Are unusually large transactions being detected?
* Are anomalies concentrated during particular periods?
* Which transactions require additional review?

The system is intended as a **decision-support mechanism** that can help analysts prioritize transactions for investigation.

---

## 🌐 Streamlit Deployment

The project includes a **Streamlit web application**.

The application supports:

### Single Transaction Analysis

Users can enter transaction information and receive:

* Normal/Anomaly prediction
* Anomaly score

### Batch Transaction Analysis

Users can:

* Upload a CSV file
* Process multiple transactions
* Generate anomaly predictions
* Download the analysis results

---

## 🗂️ Project Structure

```text
Bank-Transaction-Analytics-Anomaly-Detection/
│
├── Bank_Transaction_Analytics_Anomaly_Detection_Completed.ipynb
├── app.py
├── requirements.txt
├── IsolationForest_BankTransaction_Model.pkl
├── StandardScaler.pkl
├── Bank_Transaction_Analytics_Final.csv
└── README.md
```

---

## 💻 Technologies Used

| Technology       | Purpose                   |
| ---------------- | ------------------------- |
| Python           | Programming               |
| Pandas           | Data processing           |
| NumPy            | Numerical operations      |
| Matplotlib       | Data visualization        |
| Seaborn          | Statistical visualization |
| Scikit-learn     | Machine Learning          |
| Isolation Forest | Anomaly detection         |
| StandardScaler   | Feature scaling           |
| Jupyter Notebook | Development and analysis  |
| Streamlit        | Application deployment    |

---

## 🔄 Project Workflow

```text
Raw Bank Transaction Data
          ↓
Data Cleaning
          ↓
Exploratory Data Analysis
          ↓
Feature Engineering
          ↓
Feature Scaling
          ↓
Isolation Forest
          ↓
Anomaly Detection
          ↓
Visualization & Business Insights
          ↓
Streamlit Deployment
```

---

## 🚀 How to Run the Project

### 1. Clone the repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

### 2. Navigate to the project folder

```bash
cd Bank-Transaction-Analytics-Anomaly-Detection
```

### 3. Install the required libraries

```bash
pip install -r requirements.txt
```

### 4. Open the Jupyter Notebook

```bash
jupyter notebook
```

Open:

```text
Bank_Transaction_Analytics_Anomaly_Detection_Completed.ipynb
```

Run the notebook cells from top to bottom.

### 5. Run the Streamlit application

```bash
streamlit run app.py
```

The application will normally open at:

```text
http://localhost:8501
```

---

## 📌 Key Learning Outcomes

Through this project, I gained practical experience in:

* Data Cleaning
* Exploratory Data Analysis
* Feature Engineering
* Feature Scaling
* Unsupervised Machine Learning
* Isolation Forest
* Anomaly Detection
* Data Visualization
* Business-oriented Data Analysis
* Streamlit Deployment

---

## 🔮 Future Improvements

Possible future improvements include:

* Local Outlier Factor
* One-Class SVM
* Autoencoder-based anomaly detection
* Customer-level behavioral analysis
* Merchant category information
* Transaction location analysis
* Fraud risk scoring
* Power BI or Tableau dashboards
* Real-time transaction monitoring
* Cloud deployment

---

## ⚠️ Important Note

This project demonstrates **anomaly detection**, not automatic fraud confirmation.

A transaction classified as an anomaly should be reviewed by an appropriate analyst or investigation process before any conclusion is made.

---

## 👩‍💻 Author

**Dharshini G**

M.Sc. Data Analytics

Interested in **Data Analytics, Machine Learning, Power BI, SQL, and Data Science**.
