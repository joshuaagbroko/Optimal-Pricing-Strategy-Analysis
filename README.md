# 💸 Optimal Pricing Based on Demand Elasticity

This project analyzes historical sales data to estimate price elasticity of demand for different product categories and recommends optimal pricing strategies to maximize revenue. The work combines economic theory with data science techniques and presents results through Python-based modeling and an interactive Tableau dashboard.

---

## 📊 Project Overview

**Aim:**  
Determine the optimal price for each product category by estimating demand elasticity and simulating revenue under various pricing scenarios.

**Dataset Features:**
- Transaction ID
- Date
- Customer demographics (ID, gender, age)
- Product category
- Quantity sold
- Price per unit
- Total transaction amount

---

## 🔧 Tools & Technologies

- **Python:** pandas, numpy, statsmodels, scikit-learn, matplotlib, seaborn  
- **Jupyter Notebook:** For model development and simulation  
- **Microsoft Word:** For technical report generation

---

## 🧹 Data Preparation

- Cleaned missing values and handled outliers
- Aggregated sales data by product category
- Created features for elasticity modeling:
  - Price per unit
  - Quantity sold
  - Total revenue

---

## 📈 Price Elasticity Analysis

For each product category:
- Fitted log-log regression models to estimate demand elasticity
- Interpreted elasticity coefficients (elastic vs. inelastic)
- Evaluated model performance using R²

---

## 🧠 Optimization Strategy

Simulated revenue at varying price points to find the price that maximizes revenue using the demand function:
  
**Revenue = Price × Estimated Demand**

---

## 💼 Key Results

| Product Category | Estimated Elasticity | Model R² | Optimal Price | Max Simulated Revenue |
|------------------|----------------------|----------|---------------|------------------------|
| Beauty           | 0.02                 | 0.27     | $500.00       | $1,292.21              |
| Clothing         | 0.00                 | 0.01     | $500.00       | $1,277.53              |
| Electronics      | 0.02                 | 0.22     | $500.00       | $1,272.89              |

---

## 📌 Recommendations

- **Beauty & Electronics:** Adopt a premium pricing strategy as demand is inelastic.
- **Clothing :** Model performance was low; recommend real-world A/B testing to validate findings.
- **General:** Enhance dataset and re-train models periodically for better accuracy.

---

## 📂 Project Structure

```bash
optimal-pricing-project/
│
├── data/
│   └── retail_sales_data.csv
├── notebooks/
│   └── price_elasticity_modeling.ipynb
├── report/
│   └── Optimal_Pricing_Report.docx
├── tableau/
│   └── pricing_dashboard.twbx
├── README.md
└── requirements.txt
