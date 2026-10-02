# Customer Segmentation


## Company Overview
A UK-based e-commerce firm focused on unique gifts for various occasions. The business functions via an online e-commerce platform and serves clients throughout the United Kingdom and various global markets. Its customers consist of both individual shoppers and wholesale purchasers who buy items in large quantities.


## Business Problem
The firm regards all clients in the same way, even though there are considerable variations in their buying habits. A limited number of clients contribute significantly to revenue, whereas numerous customers buy rarely or eventually become inactive. Without customer segmentation, marketing initiatives, retention strategies, and promotional funds cannot be aimed effectively.


## Business Question
What customer segments can be identified through purchasing patterns using RFM analysis and K Means clustering, and in what ways can these segments enhance customer retention, engagement, and revenue generation?




# Insights

Champions: They make up only 1.3% of the total, yet generate around 1.62 million in revenue, indicating great customer value and robust purchasing 
           activity.

VIP:      They represent only 0.12% of the clientele, but they produce more than 1.08 million in revenue, boasting the greatest average 
          frequency (113.6 purchases) and monetary value (215,535) compared to all segments.

Regular: They make up the largest customer sector, accounting for 74.3% of the overall customer base and contributing the highest total income 
         of 5.48 million.

At Risk: With an average recency of 243 days, At Risk clients make up 24.28% of all customers, indicating a lengthy time since their last purchase.





# Segment & Recommendations 

Champions:      Offer VIP service, Provide initial access to upcoming product, Create unique loyalty incentives

VIP:            Implement loyalty programs, Offer personalized discounts, Motivate them to move into the Champion category

Regular:        Implement cross-selling and upselling strategies, Suggest additional products that enhance the original, Promote repeat buying by offering                      incentives

At Risk:        Send re-engagement emails, Provide discount coupons, Run win-back marketing initiatives
  
            




# Customer Segmentation using RFM Analysis & K-Means

## Project Overview

This project focuses on customer segmentation for a UK-based e-commerce company that sells unique gifts through an online platform.

The goal was to understand customer purchasing behavior and divide customers into meaningful groups based on their buying patterns.

I used **RFM Analysis** and **K-Means Clustering** to identify different customer segments and then developed business recommendations for each segment.



##  Company Overview

A UK-based e-commerce firm focused on unique gifts for various occasions.

The company sells through an online e-commerce platform and serves customers in the UK and other global markets. Its customers include individual shoppers as well as wholesale purchasers.



##  Business Problem

The company treats all customers in a similar way, even though their purchasing behavior can be very different.

Some customers purchase frequently and generate high revenue, while others purchase rarely or have become inactive.

Without customer segmentation, it is difficult to target marketing campaigns, retention strategies and promotional activities effectively.



##  Business Question

What customer segments can be identified from purchasing behavior using **RFM Analysis and K-Means Clustering**, and how can these segments help improve customer retention, engagement and revenue?



##  Data Cleaning

Before performing the analysis, I cleaned and prepared the dataset.

The main cleaning steps included:

- Checked missing values
- Removed records with missing customer IDs
- Removed records with missing product descriptions
- Removed negative quantity and price values
- Checked and removed duplicate transactions
- Classified stock codes into Product, Voucher and Non-Product
- Converted the invoice date into datetime format



## Feature Engineering

I created additional features to prepare the data for analysis:

- Total Amount = Quantity × Price
- Extracted Year from Invoice Date
- Extracted Month from Invoice Date
- Created a customer-level RFM table



## RFM Analysis

RFM was used to understand customer purchasing behavior based on three dimensions:

### Recency
How recently a customer made a purchase.

### Frequency
How often a customer made a purchase.

### Monetary
How much revenue a customer generated.

The final RFM dataset contained **4,312 customers**. :contentReference[oaicite:4]{index=4}



##  K-Means Clustering

After creating the RFM features, I used **StandardScaler** to scale Recency, Frequency and Monetary values before applying K-Means clustering. :contentReference[oaicite:5]{index=5}

I used the **Elbow Method** to help determine the number of clusters and then applied K-Means with **4 clusters**.

The four customer segments were:

- Champions
- VIP
- Regular
- At Risk



## Customer Segments & Insights

### Champions

- **1.30%** of customers
- Generated approximately **1.62M** in revenue
- Show strong purchasing activity and high customer value

### VIP

- **0.12%** of customers
- Generated approximately **1.08M** in revenue
- Highest average frequency: **113.6 purchases**
- Highest average monetary value: approximately **215,535**

### Regular

- **74.30%** of customers
- Largest customer segment
- Generated approximately **5.48M** in revenue

###  At Risk

- **24.28%** of customers
- Average recency of approximately **243 days**
- Indicates customers who have not purchased for a long period

The segment percentages and revenue values were calculated from the final RFM dataset. :contentReference[oaicite:8]{index=8}



## Business Recommendations

| Segment | Recommendations |
|---|---|
| **Champions** | Offer VIP service, early access to new products and exclusive loyalty rewards |
| **VIP** | Introduce loyalty programs, personalized discounts and encourage movement into the Champion segment |
| **Regular** | Use cross-selling and upselling, recommend related products and encourage repeat purchases |
| **At Risk** | Send re-engagement emails, provide discount coupons and run win-back campaigns |

These recommendations are based on the purchasing behavior identified through the customer segments. :contentReference[oaicite:9]{index=9}


##  Tools & Techniques

### Tools

- Python
- Jupyter Notebook
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

### Techniques

- Data Cleaning
- Exploratory Data Analysis
- Feature Engineering
- RFM Analysis
- Feature Scaling
- Elbow Method
- K-Means Clustering
- Customer Segmentation
- Data Visualization
- Business Insight Generation

---

## Project Workflow

Raw E-commerce Data
        ↓
Data Cleaning
        ↓
Feature Engineering
        ↓
RFM Analysis
        ↓
Feature Scaling
        ↓
Elbow Method
        ↓
K-Means Clustering
        ↓
Customer Segmentation
        ↓
Business Insights
        ↓
Marketing Recommendations



