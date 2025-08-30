# Customer Segmentation Using Hypothesis Techniques

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



Customer Segmentation Project using K-Means Clustering

Overview

This project applies K-Means clustering to customer data in order to identify distinct customer segments. By grouping customers based on demographics and purchasing behavior, businesses can better understand their customer base, design targeted marketing strategies, and improve loyalty and retention.

The analysis focuses on three key features:
	•	Age (demographics)
	•	Annual Income (spending power)
	•	Purchase Frequency (engagement/behavior)

⸻

Data Overview

The dataset includes the following attributes:
	•	Customer ID: Unique identifier for each customer
	•	Age: Age of the customer
	•	Income: Annual income (converted from ranges into numeric midpoints)
	•	Purchase Frequency: Number of purchases made in a given period

⸻

Methodology
	1.	Data Cleaning
	•	Removed symbols (₹, ,).
	•	Converted income ranges (e.g., 410000 - 655999) into midpoints.
	•	Ensured all features were numeric.
	2.	Feature Selection
	•	Selected Age, Income, and Purchase Frequency as the main features.
	•	These provide a balance of demographic and behavioral information.
	3.	Standardization
	•	Used StandardScaler to scale features so no single feature (like Income) dominates clustering.
	4.	K-Means Clustering
	•	Applied K-Means with n_clusters = 4.
	•	Customers were grouped into four segments based on similarities.
	5.	Visualization
	•	Scatterplot with Annual Income vs. Purchase Frequency was used to visualize clusters.
	•	Each cluster was color-coded for clear interpretation.

⸻

Results: Cluster Profiles

The K-Means clustering produced 4 distinct customer groups:

Cluster	  Avg Age	     Avg Income	       Avg Purchase Freq	                   Profile & Insights
  0	     ~38 yrs       	~10.7 lakh	              3	                   Older, high-income, moderate buyers. Good candidates for premium products and loyalty rewards.
  1	     ~27 yrs       	~5.25 lakh	            1.75	                  Younger, mid-income, low-frequency shoppers. Need promotions/discounts to increase engagement.
  2	     ~28 yrs       	~5.33 lakh	             5	                    Younger, mid-income, frequent shoppers. Already engaged. Focus on retention through rewards and personalization.
  3	     ~26 yrs       	~5.33 lakh	             12                	Very young, mid-income, super frequent buyers. Your core champions. Keep them loyal with exclusive offers and early access.


⸻

Key Findings
	•	Income is not the only differentiator — customers with similar income levels show very different shopping frequencies.
	•	Cluster 0 shows that high-income individuals do not always purchase frequently, suggesting potential for targeted upselling.
	•	Clusters 2 & 3 highlight younger customers with strong engagement, making them critical for long-term loyalty strategies.
	•	Cluster 1 represents occasional shoppers who may need targeted campaigns to increase spending.

⸻

Conclusion

The clustering analysis provides a more behavior-driven view of customers compared to a demographic-only analysis. Businesses can:
	•	Design personalized strategies for frequent vs. occasional shoppers.
	•	Create premium programs for high-income but low-frequency customers.
	•	Focus on retention and loyalty for engaged younger buyers.

⸻

Technologies Used
	•	Python: Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn
	•	Excel: Initial dataset preparation
	•	Clustering Method: K-Means


