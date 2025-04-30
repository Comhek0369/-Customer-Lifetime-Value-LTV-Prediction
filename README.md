# 📈 Customer Lifetime Value (LTV) Prediction

Predicting the lifetime value of customers based on historical transaction behavior to support data-driven marketing, segmentation, and retention strategies.

---

## 🚀 Objective

Develop a regression model to estimate Customer Lifetime Value (LTV) using transaction data. This enables:
- Identification of high-value customers
- Targeted marketing and retention campaigns
- Efficient allocation of customer acquisition budgets

---

## 🧰 Tools & Libraries

- Python 3.11
- pandas, numpy
- scikit-learn
- XGBoost
- matplotlib, seaborn

---

## 🗃️ Dataset Overview

### 1. `transactions.csv`
| Column         | Description                  |
|----------------|------------------------------|
| Customer_id    | Unique ID for each customer  |
| Order_id       | Unique transaction ID        |
| Order_date     | Date of transaction          |
| Order_amount   | Purchase amount              |

### 2. `customers.csv`
| Column         | Description                  |
|----------------|------------------------------|
| Customer_id    | Unique ID for each customer  |
| Demographic fields (if available)             |

---

## 🔨 Feature Engineering

Features derived from historical purchase data:
- **Recency** – Days since last purchase
- **Frequency** – Number of purchases
- **Tenure** – Days between first and last purchase
- **AOV** – Average Order Value (mean spend per order)

---

## 🧠 Model Training

- Model: **XGBoost Regressor**
- Target Variable: Total customer spend (proxy for LTV)
- Split: 80% training / 20% test
- Evaluation Metrics:
  - **MAE**: 32.49
  - **RMSE**: 49.66

---

## 📊 Results & Visualization

- ✅ LTV predicted for all customers (`customer_LTV_predictions.csv`)
- ✅ Segmented customers into tiers:
  - Top 10%
  - High (10–30%)
  - Mid (30–70%)
  - Low (bottom 30%)
- 📈 Included visualizations:
  - Actual vs Predicted LTV
  - LTV Segment Distribution

---

## 🧩 Strategic Recommendations

| Segment | Action Plan |
|---------|-------------|
| **Top** | Loyalty rewards, high-touch engagement |
| **High** | Upselling and cross-selling offers |
| **Mid** | Re-engagement and retention campaigns |
| **Low** | Cost-efficient outreach, churn monitoring |

---

## 📍 Next Steps

- Add behavioral and demographic features
- Explore log-transformed target for reducing outlier impact
- Automate model refresh quarterly
- (Optional) Deploy predictions via dashboard/API

---

## 📁 Deliverables

- ✅ `Python Notebook.ipynb` – Complete Python notebook
- ✅ `customer_LTV_predictions.csv` – LTV predictions for all customers
- ✅ `customer_LTV_segmented.csv` – Segmented customer list based on LTV
- 📊 Visualizations included in notebook

---

## 📬 Contact

For questions or collaboration: **Comhek0369** –  Contact Get it from my profile

---

