# 📊 Ecommerce Sales Dashboard (Power BI)

## 🚀 Project Overview
This project presents an end-to-end business intelligence solution built using Power BI to analyze ecommerce performance from 2023 to 2025.

The goal is to transform raw transactional data into actionable insights for business decision-making across sales, profitability, customer behavior, and regional performance.

---

## 🎯 Business Objectives
- Track overall sales and profit performance
- Identify top-performing products and categories
- Analyze customer contribution to revenue
- Evaluate regional profitability
- Understand payment behavior trends

---

## 📊 Dashboard Preview

![Dashboard Overview](images/dashboard-overview.png)

## 📈 Detailed Analysis
![Analysis](images/dashboard-analysis.png)

---

## 📈 Key Metrics
| Metric            | Value   |
|------------------|--------|
| Total Sales       | $485K  |
| Total Profit      | $159K  |
| Profit Margin     | 32.79% |
| Total Orders      | 2,000  |
| Total Customers   | 1,534  |

---

## 🔍 Key Insights

### 🪑 Product Performance
- Furniture generates the highest revenue (~$250K)
- Technology maintains strong profit margins (~34.6%)
- Office Supplies underperform in both sales and profitability

### 🌍 Regional Analysis
- Europe and North America contribute the highest profits
- Emerging markets show lower but growing potential

### 💳 Payment Trends
- Credit Cards dominate transaction volume
- Cash on Delivery has minimal contribution

### 👥 Customer Insights
- A small group of customers contributes disproportionately to total profit
- Opportunity to build loyalty programs for top customers

---

## 🛠️ Tools & Technologies
- Power BI (Data Visualization)
- DAX (Data Analysis Expressions)
- Excel / CSV (Data Source)

---

## 🧠 Data Modeling
- Star schema approach
- Fact table: Sales data
- Dimension tables: Customer, Product, Region, Date

---

## ⚙️ Key DAX Measures

```DAX
Total Sales = SUM(Sales[Sales Amount])

Total Profit = SUM(Sales[Profit])

Profit Margin % = DIVIDE([Total Profit], [Total Sales], 0)

Total Orders = DISTINCTCOUNT(Sales[Order ID])

Total Customers = DISTINCTCOUNT(Sales[Customer ID])
