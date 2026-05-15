# Customer Churn Prediction — E-commerce

A machine learning project to predict at-risk customers on an 
e-commerce platform, complete with revenue loss estimation and 
concrete business recommendations per segment.

---

## Problem Statement

> *"Which customers are at risk of not returning, and how much revenue 
> could be lost if they are not addressed?"*

E-commerce platforms face the ongoing challenge of retaining existing 
customers. This project builds an end-to-end pipeline — from data 
cleaning to business insight — that can be directly executed by a 
business team.

---

## Key Results

| | |
|---|---|
| **Model** | Logistic Regression |
| **AUC-ROC** | 0.758 |
| **Recall (churn)** | 72% |
| **Churn rate** | 51.3% of 4,909 customers |
| **Total revenue at risk** | IDR 391.5 million / month |

### Churn risk segmentation

| Segment | Customers | Est. Revenue Loss/Month |
|---------|-----------|--------------------------|
| High (>70%) | 1,001 | IDR 38.4 million |
| Medium (40–70%) | 2,405 | IDR 171.1 million |
| Low (<40%) | 1,503 | IDR 182.0 million |

**Key finding:** The Medium-risk segment is the top priority — 
the largest customer group with the highest recoverable revenue at risk.

---

## Project Pipeline

Raw Data → Data Assessing → Data Cleaning → Feature Engineering
→ Model Selection → Modeling → Business Insight & Segmentation

---

### Pipeline details

1. **Data Assessing** — identifying missing values, duplicates, 
   outliers, and format inconsistencies
2. **Data Cleaning** — handling missing values using business-context 
   strategies, category standardisation, and outlier treatment
3. **Feature Engineering** — aggregating transaction data to customer 
   level, creating 11 behavioural features, and defining the churn label
4. **Modeling** — model selection via 5-fold cross-validation, training 
   Logistic Regression vs Gradient Boosting, evaluation using AUC-ROC 
   and classification report
5. **Business Insight** — churn risk segmentation, revenue loss 
   estimation, and retention campaign recommendations per segment

---

## Folder Structure

customer-churn-prediction/
├── README.md
├── notebook/
│   └── Customer_Churn_Prediction.ipynb
├── data/
│   ├── ecommerce_churn_raw.csv       # raw dataset
│   ├── ecommerce_churn_clean.csv     # cleaned dataset
│   └── customer_churn_table.csv      # customer-level features (FE output)
├── images/                           # visualisation outputs
└── requirements.txt

---

## Tech Stack

![Python](https://img.shields.io/badge/Python-3.10-blue)
![Pandas](https://img.shields.io/badge/Pandas-2.0-blue)
![Scikit--learn](https://img.shields.io/badge/Scikit--learn-1.3-orange)

- **Data manipulation:** pandas, numpy
- **Visualisation:** matplotlib, seaborn
- **Machine learning:** scikit-learn (Logistic Regression,
  Gradient Boosting, cross-validation)

---

## How to Run

1. Clone this repository
2. Install dependencies: `pip install -r requirements.txt`
3. Open `notebook/Customer_Churn_Prediction.ipynb`
4. Run all cells in order

> **Note:** The dataset used is synthetically generated for learning 
> purposes and does not represent real production data.

---

## Author

**Nabilah Yasmin Qasthalani**  
[[LinkedIn](https://www.linkedin.com/in/qasthalani/)] · [[GitHub](https://github.com/qasthalani/)]
