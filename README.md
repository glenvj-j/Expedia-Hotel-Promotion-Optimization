# Expedia Hotel Analysis and Booking Promotion Prediction Model

![Cover](https://github.com/user-attachments/assets/dc617fa3-e298-4d75-a203-8cb4a17de1ce)


Data Period : Nov 2012 - Jun 2013 | [Data Set Source](https://www.kaggle.com/datasets/vijeetnigam26/expedia-hotel)

📊 *Data Analysis & Processing by:*  [Glen Valencius Joydi](https://github.com/glenvj-j)

## 📌 Overview

This project explores user behavior and booking patterns on Expedia to build a predictive model for targeted hotel promotion distribution. The goal is to increase booking conversion rates and maximize profitability by identifying users most likely to redeem promotional offers.

---

## 🏨 1. Context

### 1.1 Background

Expedia Group, Inc. is a major player in the online travel industry, providing services to both consumers and small businesses. For this analysis, we focus on hotel bookings as the primary revenue source, allocating 10% of overall revenue as the analytical baseline.

> ⚠️ **Disclaimer**: All financial figures and revenue proportions used in this project (e.g., the 10% revenue allocation and cost savings) are **hypothetical** and used solely to support modeling, framing, and feasibility of analysis.

### 1.2 Data Structure

Each row in the dataset represents a user session with hotel search behavior, capturing a wide array of user and property-level features.

Total data row is 9 Million and column 53


---

## 🎯 2. Problem Statement

Historically, Expedia has used broad coupon distributions for hotel promotions, which often resulted in wasted marketing spend. This project aims to optimize coupon allocation by predicting which users are most likely to convert, thereby maximizing cost-efficiency and profit.

---

## 🔍 3. Analytical Approach

Our strategy centers on understanding user preferences and behaviors through three perspectives:

### 3.1 User Intent & Booking Preferences

- Only **19%** of users book hotels in their **home country**.
- Built **Top 5 Hotel Recommendations** by user country.
- `Property_116942` is the **most booked** hotel overall.
- **Higher star ratings** and **branded properties** drive higher booking rates.
- **Saturday stays**, **longer travel distances**, and **longer booking windows** correlate with increased bookings.
- 📌 **Recommendation**: Promote larger rooms and longer stays using targeted discounts.

### 3.2 User Behavior

- **Position bias** significantly affects booking (top listings get more bookings).
- **Random placement** reduces booking probability.
- **Higher prices** relative to average reduce booking likelihood.
- **Promotions increase conversion**, suggesting future work in optimizing discount levels.

### 3.3 Business Effectiveness

- Identified top **revenue-generating websites** and **high-potential segments**.
- Analyzed **top 10 hotels** by order volume and revenue.
- Evaluated **revenue per click** and **conversion funnels** to assess platform efficiency.

---

## 🤖 4. Machine Learning Approach

We trained a logistic regression model using a 100,000-row sample, oversampled to a **23% booking rate** (vs. real 2.8%) to allow meaningful model training within compute constraints.

### ✅ Results

Despite false positives, the model shows clear business benefits:

| Metric                | Value            |
|----------------------|------------------|
| Cost Without Model   | $433,060.00      |
| Cost With Model      | $5,845.11        |
| **Total Savings**    | **$427,214.89**  |

> ⚠️ **Disclaimer**: The cost-benefit values above are **estimates based on assumptions** to illustrate model effectiveness in a business context. They do **not reflect real-world Expedia data or internal metrics**.

### 🔭 Next Steps

- Train on the full dataset to reflect real-world class imbalance.
- Fine-tune cost-sensitive strategies for scalable coupon distribution.

---

## 🛠️ Technologies Used

- **Python**
- **pandas**
- **scikit-learn**
- **Logistic Regression**

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

## 👤 Author

Developed by Glen Valencius
