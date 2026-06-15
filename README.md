# 📦 Boxify Customer Churn Analysis
**Business Data Analytics Case Study | Tool: Microsoft Excel**

> Analyzing customer behavior, engagement patterns, and subscription trends to identify churn drivers and recommend retention strategies for a subscription box service.

---

## 📌 Project Overview

Boxify is an online subscription box service delivering lifestyle products on monthly, quarterly, and annual plans. The business was experiencing rising cancellations within the first few months — making revenue unpredictable and slowing growth.

This project conducts a full end-to-end churn analysis on 900 customers to:
- Identify which customer segments are most at risk
- Understand the root causes behind early cancellations
- Quantify the revenue impact of churn
- Recommend data-driven retention strategies

---

## 🗂️ Dataset Overview

| Field | Description |
|---|---|
| CustomerID | Unique customer identifier |
| JoinDate / CancelDate | Subscription start and end dates |
| Age / Gender / Location | Customer demographics |
| SubscriptionType | Monthly, Quarterly, or Annual |
| TotalSpent | Lifetime revenue per customer |
| BoxesReceived | Engagement proxy metric |
| EngagementScore | Platform interaction score (0–100) |
| Churn Status | Active or Churned |
| Subscription Duration | Months as a customer |
| Engagement Group | Low / Medium / High (derived) |
| Age Group | 18–24, 25–34, 35–44, 45+ (derived) |

**Total Records:** 900 customers | **Churned:** 349 | **Active:** 551

---

## 🛠️ Tools & Techniques Used

- **Microsoft Excel** — Primary analysis tool
- Pivot Tables & Pivot Charts
- Calculated Columns (Churn Status, Subscription Duration, Engagement Group, Age Group)
- Conditional Formatting
- Data Cleaning (date formatting, field standardization)
- Bar Charts, Cross-tab Analysis, Churn Risk Matrix
- LTV (Lifetime Value) Calculation using aggregated spend fields

---

## 🔍 Analysis Workflow

```
Raw Data → Data Cleaning & Validation → Feature Engineering
→ Exploratory Data Analysis → Segmentation → Visualization → Recommendations
```

### Step 1 — Data Cleaning & Validation
- Standardized date formats for JoinDate and CancelDate
- Removed inconsistencies in Churn Status field
- Validated all 900 rows for completeness

### Step 2 — Feature Engineering
- Created **Churn Status** column (Active / Churned)
- Calculated **Subscription Duration** (months between join and cancel)
- Derived **Engagement Group** (Low / Medium / High based on EngagementScore)
- Derived **Age Group** buckets for demographic segmentation

### Step 3 — Exploratory Data Analysis
- Overall churn rate across the customer base
- Churn breakdown by subscription type, engagement level, and age group
- Subscription duration comparison between active and churned customers
- Revenue (LTV) gap analysis between retained and lost customers

### Step 4 — Visualization & Reporting
- Pivot charts across 4 behavioral segments
- Churn risk matrix (Engagement Group × Subscription Type)
- Revenue loss breakdown by plan type
- Bar charts for demographic churn patterns

---

## 📊 Key Findings

| Finding | Metric |
|---|---|
| Overall Churn Rate | **38.8%** (349 out of 900 customers) |
| Highest Risk Segment | Low-engagement monthly users — **57% churn rate** |
| Avg. Subscription (Active) | **35 months** |
| Avg. Subscription (Churned) | **6.3 months** |
| Active Customer LTV | **₹12,622** |
| Churned Customer LTV | **₹8,044** |
| LTV Gap | **₹4,578 per customer (36% higher for active)** |
| Revenue Lost to Churn | **₹28.07L total** |
| Biggest Revenue Loss Segment | Monthly plan — **₹15.09L** |
| Highest Risk Group (count) | Low engagement + Monthly = **115 churned customers** |

---

## 💡 Key Insights

- **Churn is not plan-specific** — cancellation rates are similar across Monthly (40%), Annual (39.6%), and Quarterly (36.5%) plans. The issue is behavioral, not structural.
- **Engagement is the strongest churn predictor** — Low-engagement customers churn at 57% vs. only 13% for High-engagement customers.
- **The first 6 months are critical** — 80%+ of cancellations happen within 6.3 months of joining. Customers who cross this window rarely leave.
- **Monthly plan drives the highest revenue loss** — Not because of a higher churn rate, but due to the sheer volume of monthly users churning.
- **Retained customers are worth significantly more** — A ₹4,578 LTV gap means every retained customer adds measurable bottom-line impact.

---

## ✅ Recommendations

| Recommendation | Expected Impact |
|---|---|
| Launch structured onboarding program for new users (Month 1–2) | Reduce early churn by 15–20% |
| Offer ₹100–₹200 discount for first 2 months to new monthly users | Improve retention in highest-risk cohort |
| Re-engage low-activity users with reminders, feedback prompts, and small rewards | Increase engagement score in low group |
| Proactively identify at-risk customers (low engagement + short duration) | Enable early intervention before cancellation |
| Incentivize monthly users to upgrade to quarterly/annual plans | Reduce churn opportunity window |
| Focus retention campaigns exclusively on monthly plan segment | Maximize ROI on retention spend |

---

## 📁 Project Structure

```
boxify-customer-churn-analysis/
│
├── README.md                        ← You are here
├── Case_Study_2_data.xlsx           ← Raw dataset + analysis workbook
└── assets/
    ├── churn_overview.png           ← Overall churn rate chart
    ├── engagement_vs_churn.png      ← Engagement group breakdown
    ├── subscription_duration.png    ← Active vs Churned duration comparison
    ├── ltv_comparison.png           ← Revenue gap visualization
    └── churn_risk_matrix.png        ← Segment risk matrix
```

> 📸 *Add screenshots of your Excel charts to the `/assets` folder and they will render here.*

---

## 🎯 Skills Demonstrated

`Data Cleaning` `Data Validation` `Feature Engineering` `Pivot Tables` `Pivot Charts`
`Customer Segmentation` `Cohort Analysis` `LTV Analysis` `Churn Modeling`
`Data Visualization` `Business Insights` `Retention Strategy` `Microsoft Excel`

---



---

*This project was completed as part of a Data Analytics case study program. All data is fictional and used for learning purposes only.*
