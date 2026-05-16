# 📊 Customer Churn Analysis Dashboard

> A business case-based practical project analyzing customer churn behavior in subscription-based fitness and wellness services using **SQL** and **Excel**.

---

## 🖼️ Dashboard Preview

![Dashboard Screenshot](Screenshots/7.png)

---

## 📁 Project Structure

```
Standalone_Business_Case-Based_Practical/
│
├── 📄 CustomerSubscriptions.csv       ← Original dataset
├── 📊 CustomerSubscriptions.xlsx      ← Excel dashboard
├── 📄 ChurnedVsActive.csv             ← SQL query output
├── 📄 ChurnRateByType.csv             ← SQL query output
├── 📝 ChurnSummary.txt                ← Final insights
│
└── 📂 Screenshots/
    ├── 1.png   ← Query 1 output
    ├── 2.png   ← Query 2 output
    ├── 3.png   ← Query 3 output
    ├── 4.png   ← Query 4 output
    ├── 5.png   ← Query 5 output
    ├── 6.png   ← Query 6 output
    └── 7.png   ← Dashboard screenshot
```

---

## 🎯 Project Objective

Analyze customer churn risk and identify retention patterns in subscription-based fitness and wellness services.

**Key questions answered:**
- Which subscription type has the highest churn rate?
- Are inactive customers more likely to leave?
- Does feedback score impact churn probability?
- Does session attendance affect customer retention?

---

## 🛠️ Technologies Used

| Tool | Purpose |
|---|---|
| MySQL Workbench | SQL analysis and querying |
| SQL | Data extraction and aggregation |
| Microsoft Excel | Dashboard and data visualization |

---

## 🗂️ Dataset Overview

**File:** `CustomerSubscriptions.csv`

| Column | Type | Description |
|---|---|---|
| `CustomerID` | INT | Unique customer identifier |
| `Name` | VARCHAR | Customer full name |
| `Age` | INT | Age of the customer |
| `Gender` | VARCHAR | Male / Female / Other |
| `SubscriptionType` | VARCHAR | Monthly / Quarterly / Yearly |
| `SubscriptionDate` | DATE | Subscription start date |
| `LastLoginDate` | DATE | Most recent login date |
| `TotalSessions` | INT | Total sessions attended |
| `FeedbackScore` | FLOAT | Customer rating (1–10 scale) |
| `IsChurned` | BIT | 1 = Churned, 0 = Active |

---

## 📌 SQL Queries

### ✅ Query 1 — Active vs Churned by Subscription Type
Counts active and churned customers grouped by subscription type.

![Query 1](Screenshots/1.png)

---

### ✅ Query 2 — Average Feedback Score by Subscription Type & Gender
Calculates average feedback scores segmented by subscription type and gender.

![Query 2](Screenshots/2.png)

---

### ✅ Query 3 — At-Risk Customers
Identifies customers with low engagement:
- `TotalSessions < 5`
- `FeedbackScore < 5`

![Query 3](Screenshots/3.png)

---

### ✅ Query 4 — Inactive Customers (Last 60 Days)
Flags customers who have not logged in for 60+ days.

![Query 4](Screenshots/4.png)

---

### ✅ Query 5 — Churn Rate by Subscription Type
Calculates churn percentage per subscription category.

![Query 5](Screenshots/5.png)

---

### ✅ Query 6 — Top 10 Longest Subscriptions
Lists the top 10 customers with the longest active subscription tenure.

![Query 6](Screenshots/6.png)

---

## 📊 Excel Dashboard

The interactive Excel dashboard provides a complete visual summary of churn behavior.

### 📈 KPI Cards
| KPI | Description |
|---|---|
| Total Customers | Overall customer count |
| % Churned | Overall churn percentage |
| Avg Feedback Score | Mean customer satisfaction rating |
| Avg Days Since Last Login | Average inactivity window |

### 📉 Charts

| Chart Type | Insight |
|---|---|
| 🍩 Donut Chart | Active vs Churned distribution |
| 📊 Bar Chart | Churn rate by subscription type |
| 📈 Line Chart | Monthly churn trend over time |
| 🔵 Scatter Plot | Feedback Score vs Total Sessions |

---

## 📊 Churn Data Summary

### Active vs Churned by Subscription Type

| Subscription Type | Active | Churned | Total |
|---|---|---|---|
| Monthly | 561 | 462 | 1,023 |
| Quarterly | 387 | 202 | 589 |
| Yearly | 262 | 126 | 388 |

### Churn Rate by Subscription Type

| Subscription Type | Total Customers | Churned | Churn Rate |
|---|---|---|---|
| Monthly | 1,023 | 462 | **45.16%** 🔴 |
| Quarterly | 589 | 202 | **34.30%** 🟡 |
| Yearly | 388 | 126 | **32.47%** 🟢 |

---

## 🔍 Key Insights

- 🔴 **Monthly subscribers** had the highest churn rate at **45.16%**, nearly 1 in 2 customers.
- 🟢 **Yearly subscribers** were the most loyal with a churn rate of only **32.47%**.
- 📉 Customers with **low feedback scores** showed significantly higher churn probability.
- 🏋️ **Lower session attendance** was strongly linked to higher churn rates.
- ⏰ **Inactive customers** (no login in 60+ days) had elevated churn risk.

---

## 💡 Recommendations

| Area | Action |
|---|---|
| Monthly Subscribers | Launch targeted engagement campaigns and offer upgrade incentives |
| Session Attendance | Send reminders and personalized workout suggestions |
| Low Feedback Customers | Trigger follow-up surveys and offer support proactively |
| Inactive Users | Automate re-engagement emails for users inactive 30+ days |
| Loyal Customers | Introduce loyalty rewards and referral programs for yearly subscribers |

---

## ✅ Conclusion

This project successfully analyzed customer churn patterns using SQL queries in MySQL Workbench and visualized the results in an interactive Excel dashboard.

Key churn indicators identified:
- **Subscription type** (Monthly = highest risk)
- **Customer inactivity** (60+ days without login)
- **Feedback score** (low satisfaction → high churn)
- **Session participation** (low attendance → higher dropout)

The dashboard provides actionable visual insights for business stakeholders to reduce churn and improve customer retention.

---

## 👨‍💻 Developed By

**Devan Patel**

---

*Feel free to ⭐ this project if you found it useful!*