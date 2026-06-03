# 💳 AtliQo-CardBoost

**AtliQo-CardBoost** is a complete data analytics project for **AtliQo Bank’s new credit card launch**, focused on identifying the best customer segment and validating the card’s impact through data-driven experimentation. The project combines **data cleaning, customer segmentation, exploratory analysis, and A/B testing** to measure real business outcomes.

---

## 📘 Project Overview

- **Objective:** Identify the right customer segment for a new credit card and evaluate its impact on spending using a pilot A/B test.  
- **Duration:** 2 Phases (Data Analysis & Pilot Testing)  
- **Tools:** Python (Pandas, NumPy, Matplotlib, Seaborn), SQL, Excel  
- **Techniques:** Data Cleaning, Feature Engineering, Segmentation, Statistical Hypothesis Testing  

---

## 📊 Dataset Summary

| Dataset | Rows | Columns | Description |
|----------|------|----------|-------------|
| Customers | 1,000 | 8 | Demographic and financial data |
| Credit Profiles | 1,000 | 7 | Credit limit, outstanding debt, and score |
| Transactions | 500,000 | 7 | Transaction-level data including platform and amount |

---

## 🧹 Data Cleaning & Preparation

- Filled **50 missing annual incomes** using occupation-wise median values.  
- Corrected invalid ages (1–135) → restricted to **18–64**.  
- Removed **4 duplicate credit profiles** and filled **65 missing credit limits** using score-based mode mapping.  
- Replaced **4,734 zero-amount transactions** with median of (platform, category, payment_type) group.  
- Validated that `outstanding_debt` ≤ `credit_limit` for all customers.

---

## 🔎 Exploratory Data Analysis (Phase 1)

- Majority of customers fall in the **26–48 age group (56.7%)**, followed by **18–25 (24.6%)**.  
- Strong positive correlation between:
  - `credit_limit` & `credit_score` → **0.85**  
  - `credit_limit` & `annual_income` → **0.68**  
- **18–25 segment** identified as under-utilized with high potential — lower income and credit history but strong activity in **Electronics, Fashion & Beauty** categories.  

---

## 🧪 Pilot A/B Test (Phase 2)

- **Sample:** 100 customers selected from 18–25 cohort (balanced test & control).  
- **Duration:** 2-month pilot.
- **Metric:** Average transaction amount per day.

| Group | Mean (₹) | Std. Dev. |
|--------|-----------|-----------|
| Control | 221.18 | 21.36 |
| Test | 235.98 | 36.66 |

**Statistical Test:**  
- Two-sample Z-test (right-tailed)  
- **Z = 2.75**, **p = 0.003** → *Reject null hypothesis* ✅  
- Result: **Significant uplift (~6.7%)** in average transactions for test group.

---

## 📈 Key Outcomes

- Identified **18–25 age group** as the prime target for the new credit card.  
- Verified **statistically significant uplift** during pilot (Z = 2.75, p = 0.003).  
- Provided a **clear framework** for data-driven decision-making in credit product launches.  
- Demonstrated practical expertise in **data analysis, A/B testing, and business insight generation**.

---

## 🏁 Outcome (in Simple Words)

The new credit card campaign for the **18–25 age group** was **successful**.  
During the 2-month pilot, users who received the new card **spent about 7% more on average** than those who didn’t.  
This means the new card design and offers **effectively increased customer spending**, confirming that **this young segment is the right target** for the full launch.


---

## 🧠 Learnings & Skills Demonstrated

- Advanced **data cleaning and preprocessing** on large datasets (500k+ rows).  
- Strong understanding of **A/B testing and hypothesis testing**.  
- **Customer segmentation** and data-driven marketing insights.  
- Visualization & storytelling for business presentation.

---

## 🧩 Tech Stack

**Languages:** Python 
**Libraries:** Pandas, NumPy, Matplotlib, Seaborn, SciPy  
**Visualization:**  Matplotlib  
**Version Control:** Git, GitHub

---


