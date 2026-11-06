# 🏦 Bank Customer Churn Analysis | Power BI Dashboard

An end-to-end Data Analytics project that analyzes why bank customers leave, using Microsoft Power BI.

The dashboard breaks churn down by demographics, products, finances, and customer satisfaction to show which customer groups are at the highest risk.

* * *

## 📌 Project Overview

The goal is to measure customer churn in a retail bank and identify the segments that drive it. The dashboard has three pages, each focused on one angle of the problem.

## 🎯 Business Objectives

- Measure the overall churn rate and the number of churned customers.
- Identify the age groups, countries, and genders with the highest churn.
- Understand the impact of products, card type, and account activity on churn.
- Measure how much balance is lost through churned customers.
- Examine the link between complaints, satisfaction score, and churn.

## ❓ Business Questions

1. What is the overall churn rate?
2. Which age bands carry the highest churn risk?
3. How does churn differ by country and gender?
4. Does the number of products or card type affect churn?
5. Are inactive members more likely to leave?
6. How do complaints and satisfaction scores relate to churn?
7. Which credit-score and balance bands churn the most?

* * *

## 🛠️ Tools & Technologies

| Tool | Purpose |
|------|---------|
| Microsoft Power BI | Dashboard development and visualization |
| Power Query | Data cleaning and transformation |
| DAX | Measures (Churn Rate, Churn Risk Index, Complaint Rate, ...) |
| Data Modeling | Dedicated `_Measures` table, calculated bands |

* * *

## 🧹 Data Preparation

- Source: `Customer-Churn-Records.csv`
- Checked data types and missing values in Power Query.
- Created grouped fields: **Age Band**, **Credit Band**, **Balance Band**.
- Built a dedicated `_Measures` table to keep all DAX in one place.

## 🧮 Key DAX Measures

| Measure | Description |
|---------|-------------|
| Total Customers | Number of customers |
| Churned Customers / Retained Customers | Split by exit status |
| Churn Rate | Churned ÷ Total |
| Churn Rate vs Overall | Segment churn compared to the overall rate |
| Churn Risk Index | Relative risk of a segment |
| Complaint Rate | Share of customers who complained |
| Active Member Rate | Share of active customers |
| Avg Balance / Avg Credit Score / Avg Products | Customer profile averages |
| Churned Balance | Total balance of churned customers |

* * *

## 📊 Dashboard Preview

### Page 1 – Overview
![Overview](Screenshots/01-overview.png)

### Page 2 – Demographics
![Demographics](Screenshots/02-demographics.png)

### Page 3 – Products & Finance
![Products & Finance](Screenshots/03-products-finance.png)

* * *

## 💡 Key Findings

> ⚠️ Replace with the real numbers from your dashboard
- Overall churn rate is **X%** (X churned out of X customers).
- The age band **X–X** has the highest churn rate (**X%**).
- **[Country]** has the highest churn rate among countries.
- Customers with **X products** churn the most.
- Inactive members churn **X times** more than active ones.
- Churned customers took **X** in balance with them.

## 📈 Business Recommendations

1. **Target high-risk age groups** with retention offers.
2. **Re-engage inactive members** before they leave.
3. **Review the product mix** for the segments with the highest churn.
4. **Act fast on complaints** and track satisfaction scores.
5. **Protect high-balance customers** first, since their loss costs the most.

* * *

## 📁 Project Structure

```
Bank-Customer-Churn-Analysis/
├── Screenshots/
├── bankdata.pbix
└── README.md
```

## 🚀 How to Explore

1. Clone or download this repository.
2. Open `bankdata.pbix` in Power BI Desktop.
3. Use the slicers (Gender, Age, Geography, Card Type, Complain, IsActiveMember) to explore.

## 👩‍💻 Author

**Renal Salah**
- **GitHub:** [renalnader16](https://github.com/renalnader16)
- **LinkedIn:** [Renal Salah](https://linkedin.com/in/renal-salah/)
