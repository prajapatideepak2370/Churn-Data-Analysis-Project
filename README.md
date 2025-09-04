# 📊 Customer Churn Data Analysis

## 📌 Project Overview

Customer churn is a critical challenge for subscription-based businesses. This project focuses on exploratory data analysis (EDA) of customer churn data to uncover patterns, highlight key factors influencing churn, and provide actionable business insights.  
Using Python, Pandas, Seaborn, and Matplotlib, this notebook investigates demographic, contractual, and service usage features to understand why customers leave and how businesses can improve retention.

---

## 📂 Dataset Description

- **Source**: Customer Churn.csv  
- **Records**: Customer details including demographics, contract type, services, tenure, billing, and churn status.  
- **Target Variable**: Churn (Yes/No)  

**Key fields:**  
- `gender`, `SeniorCitizen`, `tenure`, `Contract`, `PaymentMethod`  
- Services: `PhoneService`, `InternetService`, `OnlineSecurity`, `StreamingTV`, etc.  
- `TotalCharges` (cleaned and converted from string to float)

---

## 🔎 Exploratory Data Analysis (EDA)

### 1. Data Cleaning
- Replaced blanks in `TotalCharges` with `0`, converted to float.  
- Converted `SeniorCitizen` from numeric (0/1) → categorical (`Yes/No`).  
- Checked for missing values and duplicates.  

### 2. Univariate Analysis
- **Churn distribution**: Visualized counts and percentages of churned vs retained customers.  
- **Gender impact**: Compared churn rates across male and female.  
- **Senior citizen status**: Higher churn observed in senior customers.  
- **Tenure**: Short-tenure customers showed much higher churn.  

### 3. Bivariate Analysis
- **Contract type**: Month-to-month contracts have the highest churn.  
- **Payment method**: Customers using *Electronic Check* churn the most.  
- **Services**: Lack of Online Security, Tech Support, or multiple add-ons increases churn likelihood.  

### 4. Visualizations
- Countplots, stacked bar charts, histograms, and pie charts for intuitive exploration.  
- Subplot grid to analyze multiple service features simultaneously.  

---

## 💡 Key Insights

### High risk groups:
- Month-to-month contract users  
- Customers paying via electronic check  
- Senior citizens without tech support/online security  

### Retention opportunities:
- Encourage longer contracts with incentives.  
- Provide bundled services (Tech Support, Online Security).  
- Offer personalized retention plans to senior customers.  

---

## 🛠️ Tools & Libraries
- **Python 3.x**  
- **Pandas** → data handling  
- **Seaborn & Matplotlib** → visualization  
