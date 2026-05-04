# 📊 User Metrics and Marketing Costs Analysis – Showz

## 📝 Project Description
Comprehensive analysis of user behavior and profitability of marketing strategies for Showz, an event ticket sales platform. The project evaluates how users interact with the service, when they make their first purchase, and how profitable each customer acquisition channel is.

---
## 🎯 Objectives
- Analyze user behavior and activity on the platform
- Determine the time between registration and first purchase
- Calculate customer lifetime value (LTV) by cohort
- Evaluate the profitability of marketing channels using CAC and ROMI

---
## 📌 Problem

The analytics department of **Showz** needed to understand:

- How do users interact with the service?
- When do they start purchasing after registering?
- How much value does each customer generate over time?
- When does revenue cover the customer acquisition cost?
--- 
## 🛠️ Tools and Libraries

| Library | Usage |
|---|---|
| `Pandas` | Data manipulation and analysis |
| `NumPy` | Numerical operations and metric calculation |
| `Matplotlib` | Visualization |

## 📐 Methodology

### 1. 🔧 Data Cleaning and Preprocessing
- Standardization of columns to snake_case format
- Conversion of date columns to datetime format
- Calculation of derived variables: session duration, start month and year

### 2. 👥 User Behavior Analysis
Metrics calculated to understand platform activity:

| Metric | Value |
|---|---|
| DAU (Daily Active Users) | ~907 |
| WAU (Weekly Active Users) | ~5,716 |
| MAU (Monthly Active Users) | ~23,228 |
| Stickiness Factor (DAU/MAU) | ~3.9% |

> The low stickiness factor indicates that users do not visit the platform consistently. The highest concentration of sessions occurs in the **first 3 months** and the **last 3 months** of the year.

### 3. Session Duration
- Most sessions last between **17 and 23 hours** from first contact to purchase.
- This suggests that the purchase decision process is not immediate.
  <img width="790" height="490" alt="image" src="https://github.com/user-attachments/assets/40d8c021-c3f2-4698-9834-c1a8fff6376a" />
---
  <img width="990" height="490" alt="image" src="https://github.com/user-attachments/assets/70f26c74-bfc0-4e2a-9f4a-e59e5931e9f7" />

### 4. Life Time Value
LTV (Life Time Value) measures how much revenue a customer generates for the company throughout their entire relationship with the service.
- The retention rate in the first months remains stable.
- At the end of each cohort, the retention variation is approximately **2%**, indicating moderate but sustained customer loyalty.
  <img width="1261" height="374" alt="image" src="https://github.com/user-attachments/assets/eeafe1d8-9c55-4baa-89b3-d59e5ac8791e" />

  
### 5.  Marketing Analysis

#### 💵 Customer Acquisition Cost (CAC)
Marketing spend was tracked across 9 acquisition sources (source_id 1–9) from January 2017 to December 2018.
- Calculation of CAC by acquisition source
- Classification of users as **profitable** or **non-profitable** based on LTV vs CAC
- 97.7% of users generated more revenue than it cost to acquire them.
- Only 2.3% of users did not recover their acquisition cost.
  <img width="640" height="509" alt="image" src="https://github.com/user-attachments/assets/61989722-dc7e-4033-ab70-318f141ffb14" />
---
  <img width="918" height="590" alt="image" src="https://github.com/user-attachments/assets/76909f22-c61b-4a64-95d1-9bb68118b30d" />


#### 📈 Return on Marketing Investment (ROMI)
ROMI (Return On Marketing Investment) measures how efficient marketing spend is relative to the revenue it generates.
- Calculation of ROMI = LTV / CAC by cohort and lifecycle
- ROMI was positive across the majority of cohorts, confirming that marketing campaigns at Showz are profitable.
  ![Uploading image.png…]()

---

## 📊Conclusions 
1. **Low stickiness**  Users do not interact consistently. Reactivation strategies are recommended.
2. **Marked seasonality** Activity peaks at the beginning and end of the year, coinciding with event seasons.
3. **Long decision cycle**  The time between first visit and purchase is 17–23 hours; onboarding could shorten it.
4. **High profitability**  With **97.7%** of users being profitable and a positive ROMI, current acquisition sources are efficient.
5. **Acceptable loyalty**  Retention varies by **±2%** across cohorts, showing a solid but improvable customer relationship.

---

## ✅ Recommendations
- Implement reactivation strategies to improve the stickiness factor
- Optimize investment in acquisition channels with the highest ROMI
- Design incentives to convert non-profitable users into repeat customers
- Reinforce campaigns during low-activity periods (February to August)
