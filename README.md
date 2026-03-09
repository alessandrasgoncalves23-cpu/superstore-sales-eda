# 🛒 Superstore Sales Analysis & Forecasting

> End-to-end data science project covering exploratory data analysis, profit insights, and machine learning sales forecasting on the Tableau Superstore dataset.

![Python](https://img.shields.io/badge/Python-3.10-14213D?style=flat-square&logo=python&logoColor=FCA311)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-14213D?style=flat-square&logo=scikit-learn&logoColor=FCA311)
![Pandas](https://img.shields.io/badge/Pandas-14213D?style=flat-square&logo=pandas&logoColor=FCA311)
![Matplotlib](https://img.shields.io/badge/Matplotlib-14213D?style=flat-square&logo=plotly&logoColor=FCA311)
![Status](https://img.shields.io/badge/Status-Complete-22c55e?style=flat-square)

---

## 📌 Overview

This project performs a full analysis of a US retail superstore's transactional data from 2014 to 2017, answering key business questions and building predictive ML models to forecast order-level sales.

**Business Questions Answered:**
- Which categories and regions drive the most revenue and profit?
- How does discounting impact profit margins?
- Can we predict order-level sales using machine learning?

---

## 📁 Project Structure

```
superstore-sales-analysis/
│
├── data/
│   └── Sample - Superstore.csv       # Raw dataset
│
├── plots/                             # Generated charts
│   ├── monthly_sales_trend.png
│   ├── sales_by_category.png
│   ├── distributions.png
│   ├── profit_by_region.png
│   ├── profit_heatmap.png
│   ├── yearly_growth.png
│   ├── model_comparison.png
│   ├── actual_vs_predicted.png
│   └── feature_importance.png
│
├── superstore_analysis.ipynb          # Main notebook
└── README.md
```

---

## 📊 Key Findings

| Metric | Value |
|--------|-------|
| Period | 2014 – 2017 |
| Total Revenue | $2,297,201 |
| Total Profit | $286,397 |
| Profit Margin | 12.5% |
| Top Category | Technology |
| Best Region | West |
| Worst Sub-Category (profit) | Tables |

**Insights:**
- **Technology** leads in both sales volume and profit margin
- **Discounts above 20%** consistently result in negative profit — a clear pricing risk
- **Q4 seasonal spikes** appear every year, especially November–December
- The **West region** outperforms all others in profitability
- **Tables** is the only sub-category that consistently loses money across all regions

---

## 🤖 Machine Learning

Three regression models were trained to predict sales at the order level using features such as category, sub-category, region, segment, ship mode, quantity, discount, and time-based variables.

| Model | RMSE | MAE | R² |
|-------|------|-----|----|
| Linear Regression | $752 | $273 | 0.04 |
| Random Forest | $692 | $220 | 0.19 |
| **Gradient Boosting** ✅ | **$690** | **$204** | **0.19** |

**Best model:** Gradient Boosting  
**Top predictive features:** Sub-Category, Quantity, Month, Days to Ship

---

## ⚙️ How to Run

**1. Clone the repository**
```bash
git clone https://github.com/your-username/superstore-sales-analysis.git
cd superstore-sales-analysis
```

**2. Install dependencies**
```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

**3. Add the dataset**

Place `Sample - Superstore.csv` inside the `data/` folder.  
You can download it from [Kaggle](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final).

**4. Run the notebook**
```bash
jupyter notebook superstore_analysis.ipynb
```

---

## 🛠️ Tech Stack

- **Python 3.10**
- **Pandas & NumPy** — data wrangling and feature engineering
- **Matplotlib & Seaborn** — data visualization
- **Scikit-learn** — machine learning (Linear Regression, Random Forest, Gradient Boosting)

---

## 📫 Author

**Alessandra Gonçalves** — Data Scientist & ML Engineer

[![LinkedIn](https://img.shields.io/badge/LinkedIn-14213D?style=flat-square&logo=linkedin&logoColor=FCA311)](https://www.linkedin.com/in/alessandra-souza-gon%C3%A7alves-271750269/)
[![Email](https://img.shields.io/badge/Email-14213D?style=flat-square&logo=gmail&logoColor=FCA311)](mailto:alessandrasgoncalves23@gmail.com)
