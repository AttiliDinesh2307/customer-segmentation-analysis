# Customer Segmentation Project

## Overview
This project analyzes customer data to identify distinct customer segments. By segmenting customers, businesses can gain valuable insights into their customer base, tailor marketing strategies, and improve product offerings to better meet the needs of different groups.

The analysis focuses on both demographic information (age, gender, income) and purchasing behavior (frequency, average spend, product categories, and payment methods).

---

## Data Overview
The dataset includes the following attributes:

- **Customer ID**: Unique identifier for each customer  
- **Age**: Age of the customer  
- **Gender**: Male or Female  
- **Income**: Annual income of the customer  
- **Income Group**: Grouped income category (Low, Medium, High)  
- **Purchase Frequency**: How often a customer makes a purchase (Rarely, Occasionally, Frequently, Monthly)  
- **Average Purchase Amount**: Typical amount spent per purchase  
- **Product Categories Purchased**: List of product categories purchased  
- **Last Purchase Date**: Date of most recent purchase  
- **Purchase Channel**: Channel of purchase (Online/Offline)  
- **Preferred Payment Method**: Credit Card, Debit Card, UPI, or Cash  

---

## Analysis Performed
To understand customer segmentation, the following statistical tests were applied:

1. **ANOVA for Age Groups**  
   - Tested differences in purchase frequency across three age groups: 18–25, 26–35, and 36–45.  
   - **Result**: p-value = 0.093 → No statistically significant difference.

2. **ANOVA for Income Groups**  
   - Tested differences in average purchase amount across income levels: 0–4 Lakhs, 4.1–9 Lakhs, and 9.1 Lakhs or above.  
   - **Result**: p-value = 0.00055 → Statistically significant difference. Income level strongly influences average purchase amount.

3. **T-Test for Gender**  
   - Compared average purchase amount between male and female customers.  
   - **Result**: p-value = 0.690 → No statistically significant difference.

---

## Key Findings
- **Income Level** is the most significant factor influencing customer purchasing behavior.  
- **Age** and **Gender** do not show strong influence on purchase frequency or average purchase amount.  
- Segmenting customers by **income group** is the most effective strategy for designing targeted offers and pricing.

---

## Conclusion
The analysis suggests that businesses should focus on **income-based customer segmentation** to refine marketing strategies, optimize product positioning, and personalize promotional campaigns. Age and gender are less relevant in influencing purchasing behavior in this dataset.
