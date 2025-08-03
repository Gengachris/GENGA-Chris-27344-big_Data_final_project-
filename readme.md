# Credit Card Default Analysis
**Capstone Project – Introduction to Big Data Analytics**  
**Name:** GENGA Chris  
**Student ID:** 27344  

---

## 📚 Table of Contents
1. [Project Overview](#project-overview)  
2. [Sector & Problem Statement](#sector--problem-statement)  
3. [Dataset Description](#dataset-description)  
4. [Python Analytics](#python-analytics)  
   - [Data Cleaning](#1-data-cleaning)  
   - [Exploratory Data Analysis](#2-exploratory-data-analysis-eda)  
   - [Feature Engineering](#3-feature-engineering)
   - [Machine Learning Model](#4-machine-learning-model)  
   - [Evaluation Metrics](#5-evaluation-metrics)  
   - [Innovation](#6-innovation)  
5. [Power BI Dashboard](#power-bi-dashboard)  
   - Visualizations and Their Purpose  
6. [Findings & Recommendations](#findings--recommendations)  
7. [Future Work](#future-work)  
8. [Screenshots Reference](#screenshots-reference)  
9. [Project Structure](#project-structure)  
10. [How to Run This Project](#how-to-run-this-project)

---

## 🧠 Project Overview
This project analyzes credit card client data to predict the likelihood of default in the next month using data analytics and machine learning techniques. A Power BI dashboard is used to communicate insights interactively.

---

## 🏢 Sector & Problem Statement
**Sector:** Finance  

**Problem Statement:**  
Can we predict whether a credit card customer will default on their payment next month using historical customer and billing data?

---

## 📊 Dataset Description

- **Dataset Title:** Default of Credit Card Clients Dataset
- **Source:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/default+of+credit+card+clients)
- **Number of Rows:** 30,000  
- **Number of Columns:** 24  
- **Structure:** Structured (CSV format)  
- **Status:** Required preprocessing  

---

## 🐍 Python Analytics

The Python analysis was performed using Jupyter Notebook. The notebook is well-commented and includes markdown cells for clarity.

### 🔹 1. Data Cleaning

- Removed null or duplicate records  
- Converted categorical variables (e.g., `SEX`, `EDUCATION`, `MARRIAGE`) using label encoding  
- Replaced incorrect or inconsistent values  
- Outliers detected and handled

📌 **Screenshots**: 
- Data cleaning process: `screenshots/datacleaning1.0.png`
- Cleaned dataset summary: `screenshots/datacleaning1.1.png`

---

### 🔹 2. Exploratory Data Analysis (EDA)

Used seaborn and matplotlib for visualizations:

- Distribution of default clients  
- Default rates by gender, education, and marriage status  
- Correlation heatmap  

📌 **Screenshots**: 
- EDA visualizations: `screenshots/eda1.0.png`
- Distribution analysis: `screenshots/eda1.1.png`
- Correlation heatmap: `screenshots/eda1.2.png`
- Additional EDA insights: `screenshots/eda1.3png.png`

---

### 🔹 3. Feature Engineering

- Applied feature scaling and normalization
- Created derived features for better model performance
- Analyzed feature importance and selection

📌 **Screenshots**: 
- Feature engineering process: `screenshots/feature engineering1.0.png`

---

### 🔹 4. Machine Learning Model

- Chose **Logistic Regression** for classification  
- Split data into training and test sets (80/20)  
- Trained model and tested predictions  

📌 **Screenshots**: 
- Model training process: `screenshots/machine learning1.0.png`
- Model performance metrics: `screenshots/machine learning1.1.png`  

---

### 🔹 5. Evaluation Metrics

- Accuracy Score  
- Confusion Matrix  
- Precision, Recall, F1-score  

📌 **Screenshots**: 
- Model evaluation results: `screenshots/model evaluation.png`

---

### 🔹 6. Innovation

- Developed a function to automatically classify new input data  
- Included feature importance analysis using model coefficients  
- Implemented data export functionality for further analysis

📌 **Screenshots**: 
- Innovation implementation: `screenshots/innovation.png`
- Data export process: `screenshots/exporting data.png`  

---

## 📈 Power BI Dashboard

The Power BI dashboard visualizes key aspects of credit card default patterns. It includes:

### 📊 Visual 1: Default Rate by Gender
- **Purpose:** Shows gender imbalance in default likelihood  

### 📊 Visual 2: Default Rate by Education Level
- **Purpose:** Explores correlation between education level and default rate  

### 📊 Visual 3: Default by Marital Status
- **Purpose:** Assesses financial behavior across relationship types  

### 📊 Visual 4: Credit Limit Distribution
- **Purpose:** Understands how credit limits vary among defaulters vs non-defaulters  

### 📊 Visual 5: Payment Behavior (PAY_1 - PAY_6)
- **Purpose:** Tracks late payments across months  

### 📊 Visual 6: Age Distribution of Defaulters
- **Purpose:** Finds age groups more likely to default  

### 📊 Visual 7: Balance & Bill Amount Over Months
- **Purpose:** Shows trends in financial obligations  

📌 **Screenshot Suggestion**: Insert individual visuals from Power BI dashboard:  

*Note: Screenshots can be taken from the Power BI dashboard and saved in the screenshots folder*

---

## 📌 Findings & Recommendations

- Males showed slightly higher default rates than females  
- Clients with lower education levels defaulted more  
- Single clients had higher default risk than married ones  
- Past payment history (`PAY_X`) is a strong predictor of default  
- Logistic Regression performed well with ~80% accuracy  

📌 **Recommendation**: Focus marketing or risk management efforts on high-risk profiles (e.g., young single clients with poor repayment records).

---

## 🔮 Future Work

- Use ensemble models (e.g., Random Forest, XGBoost)  
- Apply feature engineering to derive new indicators  
- Connect Power BI to live databases for real-time dashboards  
- Use DAX measures for deeper KPI monitoring

---

## 🖼️ Screenshots Reference

### Python Analytics Screenshots
| Process | File Path |
|---------|-----------|
| Data Cleaning Process | `screenshots/datacleaning1.0.png` |
| Cleaned Dataset Summary | `screenshots/datacleaning1.1.png` |
| EDA Visualizations | `screenshots/eda1.0.png` |
| Distribution Analysis | `screenshots/eda1.1.png` |
| Correlation Heatmap | `screenshots/eda1.2.png` |
| Additional EDA Insights | `screenshots/eda1.3png.png` |
| Feature Engineering | `screenshots/feature engineering1.0.png` |
| Machine Learning Process | `screenshots/machine learning1.0.png` |
| Model Performance | `screenshots/machine learning1.1.png` |
| Model Evaluation | `screenshots/model evaluation.png` |
| Innovation Implementation | `screenshots/innovation.png` |
| Data Export Process | `screenshots/exporting data.png` |

### Power BI Dashboard Screenshots
*To be added when dashboard screenshots are captured*

---

## 📁 Project Structure

```plaintext
📂 big data final version/
│
├── 📊 credit_card_default_analysis.ipynb    # Main Python analysis notebook
├── 📈 GENGA CHRIS 27344 FINAL EXAM.pbix     # Power BI dashboard file
├── 📄 README.md                             # Project documentation
├── 📋 default of credit card clients.csv    # Original dataset
├── 🧹 cleaned_credit_card_data.csv          # Processed dataset
├── 🔧 credit_card_features.csv              # Engineered features
├── 🎯 model_predictions.csv                 # Model output results
└── 📸 screenshots/                          # Visual documentation
    ├── datacleaning1.0.png
    ├── datacleaning1.1.png
    ├── eda1.0.png
    ├── eda1.1.png
    ├── eda1.2.png
    ├── eda1.3png.png
    ├── exporting data.png
    ├── feature engineering1.0.png
    ├── innovation.png
    ├── machine learning1.0.png
    ├── machine learning1.1.png
    └── model evaluation.png
```

## 🚀 How to Run This Project

### Prerequisites
- Python 3.7+ with Jupyter Notebook
- Required libraries: pandas, numpy, scikit-learn, seaborn, matplotlib
- Microsoft Power BI Desktop (for dashboard viewing)

### Steps
1. **Clone/Download** this repository
2. **Open** `credit_card_default_analysis.ipynb` in Jupyter Notebook
3. **Run** all cells sequentially to reproduce the analysis
4. **Open** `GENGA CHRIS 27344 FINAL EXAM.pbix` in Power BI Desktop to view the dashboard
5. **Review** screenshots in the `screenshots/` folder for visual reference

## 📞 Contact
**Student:** GENGA Chris  
**ID:** 27344  
**Course:** Introduction to Big Data Analytics  

---
*This project demonstrates end-to-end data analytics workflow from data cleaning to machine learning and business intelligence visualization.*
