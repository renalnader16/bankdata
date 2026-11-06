# 🏦 Bank Customer Churn Analysis | Power BI Dashboard

An end-to-end Data Analytics project that analyzes why bank customers leave, using Microsoft Power BI.

The dashboard breaks churn down by demographics, products, finances, and customer satisfaction to show which customer groups are at the highest risk.

* * *

## 📌 Project Overview

The goal is to measure customer churn among 10,000 retail bank customers and identify the segments that drive it. The dashboard has three pages, each focused on one angle of the problem.

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
![Overview](Screenshots/Screenshot%202026-10-26%20225204.png)

### Page 2 – Demographics
![Demographics](Screenshots/Screenshot%202026-10-26%20225232.png)

### Page 3 – Products & Finance
![Products & Finance](Screenshots/Screenshot%202026-10-26%20225256.png)

* * *

## 💡 Key Findings

- The overall churn rate is **20.4%**: about 2,000 of 10,000 customers left.
- **Age is the strongest driver.** Customers aged 50–59 churn at **56.0%**, which is **2.75x** the overall risk. Churn is lowest at 18–29 (7.6%) and 30–39 (10.9%).
- **Germany** has double the churn of the other countries (**32.4%** vs 16.7% in Spain and 16.2% in France).
- **Women** churn more than men (**25.1%** vs 16.5%).
- **Number of products matters a lot.** Customers with 3 products churn at **82.7%** and those with 4 products at **100%**, while customers with 2 products churn at only **7.6%**.
- **Inactive members** churn at **26.9%**, almost twice the rate of active members (**14.3%**).
- Churned customers took **186M** of the **765M** total balance (about 24%). The 40–49 age band accounts for the largest share (**73M**).
- Card type, credit score, and satisfaction score show little difference in churn.

## ⚠️ Data Note

In this dataset, almost every customer who filed a complaint also left (**99.5%** churn among complainers), and the complaint rate (20.4%) equals the churn rate. This suggests the `Complain` field may be recorded after the customer has left, so it should not be treated as an early warning signal.

## 📈 Business Recommendations

1. **Focus retention on customers aged 40–59**, the highest-risk group and the largest source of lost balance.
2. **Investigate the German market** to find out why churn is double that of France and Spain.
3. **Review the 3-4 product bundles**, since customers holding them almost always leave.
4. **Re-engage inactive members** early, before they decide to leave.
5. **Prioritize high-balance customers** in retention campaigns, since their loss costs the most.

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
