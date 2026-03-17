# Amazon Product Pricing & Customer Behavior Analysis

## **1. Project Description**

This project analyzes an Amazon product dataset to uncover insights into pricing strategies, discount patterns, customer ratings, and product popularity.

The goal is to understand how pricing and discounting influence customer perception and engagement, and whether higher-priced products deliver better perceived quality.

Key focus areas include:

* Price vs discount relationships
* Price vs rating correlation
* Category-level pricing and engagement trends
* Detection of misleading discount strategies

The analysis follows a structured approach including data cleaning, validation, exploratory analysis, and business insight generation.

## **2. Problem Statement**

E-commerce platforms often use discounts and pricing strategies to influence customer behavior. However, it is unclear whether these strategies truly reflect product value or customer satisfaction.

This project aims to answer:

* Do higher discounts actually provide meaningful savings?
* Do expensive products have better ratings?
* Are ratings reliable indicators of product quality?
* How do pricing and discounts vary across categories?

## **3. Data Cleaning**

The dataset required significant preprocessing:

* Converted price columns from string (₹, commas) to numeric
* Converted discount percentage from string to float
* Fixed rating parsing errors and ensured valid numeric values
* Cleaned rating_count column by removing commas
* Extracted top-level product categories for better aggregation

This step was critical to ensure accurate analysis and avoid misleading results.

## **4. Key Analysis & Findings**

### **i. Pricing vs. Discount**
* Discount percentage is not a reliable indicator of actual savings
* High discount percentages often appear in low-cost products
* Expensive products can offer greater absolute savings even at lower discount rates

➡️ **Conclusion:** Discount percentages can be misleading and may reflect marketing strategies rather than true value.

**ii. Price vs. Discount Relationship**
* Weak negative correlation (-0.11) between price and discount
* Discounts are not strongly dependent on product price

➡️ **Conclusion:** Discount strategies are not systematically tied to product value.

**iii. Price vs. Rating**
* Weak positive correlation (0.12) between price and rating
* Higher-priced products do not significantly outperform cheaper ones in ratings

➡️ **Conclusion:** Price is not a strong indicator of product quality.

**iv. Rating Behavior**
* Ratings are heavily concentrated between 4.0 and 4.3
* Very low variation across products

➡️ **Conclusion:** Rating inflation reduces the effectiveness of ratings as a decision-making metric.

**v. Category-Level Insights**
* Electronics dominate the premium price segment
* Office products and toys are low-cost, low-discount categories
* High-value categories offer aggressive discounts
* Customer engagement is highest in Electronics and Computers

➡️ **Conclusion:** Pricing and discount strategies are strongly influenced by product category.

## **5. Final Business Insights**

* Discount percentages alone are misleading and should not be used to assess value
* Customer ratings are inflated and provide limited differentiation
* Product price does not strongly correlate with perceived quality
* High-value categories combine high discounts and high engagement, suggesting strategic promotional pricing

## **6. Tech Stack**

* Python
* Pandas
* Matplotlib
* Jupyter Notebook / Google Colab

## **7. Conclusion**
* Performed exploratory data analysis on Amazon product dataset to uncover pricing and customer behavior patterns
* Cleaned and transformed raw data including currency, percentages, and rating fields for accurate analysis
* Identified weak correlation between product price and customer ratings, challenging the assumption that higher price implies better quality
* Analyzed discount strategies and found that discount percentages are often misleading indicators of actual savings
* Derived category-level insights revealing how pricing and promotional strategies vary across product segments
