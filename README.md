# Amcon-The-Healthy-Edge-Group-Makreting-Analysis
This repo preserved all the deliverables of my prior internship at Amcon Distributing company including the EDA analysis and the market basket analysis.

The project scope included all the transactional invoice entires (3GB+) across 2012-2023. And with couple of data minings, our team come up with some key insights that could better help the marketing team to allcoate campaign/promotion resources. Feel free to check out both the EDA analysis and the market Basket Analysis notebooks for further detail!

Data Privacy Disclaimer: For security purpose, all the data from this project is modified with bias and should be remained at the higest privacy level. It is worth noticing that any vioaltion of data leakage should be taken at suer's own risk and shall be subject to legal liabilities.

## **Project Background**

The Healthy Edge Retail Group is a Wholesale distributor of consumer products, operating three natural food and supplement retail chains that represent 3% of the overall business.
The company has significant amounts of data on its product transactions, transaction date, order quantity and value, product price, product category, store name, and loyalty status that remain to be uncovered for critical insights to improve The Healthy Edge's retail excellence. This EDA analysis will concentrate the scope primarily on the Chamberlins Natural Food store banner. 

Insights and recommendations are provided on the following key areas:
**Sales Trends Analysis**: Evaluaiton of historical sales patterns across the three stores, focusing on Revenue, Order volume, and Average ROder Value (AOV)
**Product Level Performance**: An analysis of various product lines, understanding their impact on sales and promotions.
**Loyalty Program Success**: An assessment of the loyalty program on customer purchasing behavior

## **Data Structure**
![Untitled (1)](https://github.com/user-attachments/assets/805fea83-5291-4eeb-8524-384305be85df)

The entity TRANSACTION represents a unqiue item purchase from a customer in store. It emodies as a single line of transaction record from a single receipt. From ERD perspective, a Transaction table use both the Item ID and Customer ID as a combined primary key, with another assimilated representation as the column "Receipt Alias".

## **Executive Summary**

Among all categories, WATER is the most sold one with over  600k in year 2021 and between 1.5-2M in year 2022-2023. Packaged Water is the most sold subcategory, with the Spring Glass water being the most sold product. 

Year 2021 has the sales peaked in July, and the average sale is consistently lower than that of 2022 and 2023. Sale grows tremendously in year 2023 indicating strong financial recovery from the customers. 

In observance of strong seasonalities patterns, March and August tend to have the most sales growth of the year. 

Loyalty tiers have different buying preference when it comes to the Water product. Loyalty member prefers the Spring GLass Water whereas the guest prefer the HEalthy Edge Purified Water.
In terms of revenue generated, loyalty members always have the order volume higher than the guest, as well as the average order value alsohigher than the guest.

**Overall Findings**

Top Categories: From 2021 to 2023, the Water category contributed the largest share of sales, followed by Vitamins & Minerals and Vegetables as the second and third most popular categories.

Seasonality: Sales exhibited strong seasonal trends, with March and August consistently being the highest-performing months across all years.

Customer Behavior: Loyalty customers purchased larger quantities and chose higher-priced products compared to guest customers.

**Sales Month-to-Month by Water Category**

Within the Packaged Water subcategory:
Spring Water was the top-selling item, followed by Alkaline Ionized Water as the second most popular product.
![newplot](https://github.com/user-attachments/assets/6f11a0e3-4b21-4f52-9052-fd6e6cd8cc64)
![newplot (1)](https://github.com/user-attachments/assets/f856822a-c2ca-4cf8-8e5c-4bf3778b1237)
![newplot (2)](https://github.com/user-attachments/assets/ec061c6a-9c35-4705-8733-6c31f3d5d950)
Sales of Spring Glass Water increased steadily during the second half of each year, while Alkaline Ionized Water sales remained relatively constant year-round.
![newplot (3)](https://github.com/user-attachments/assets/eb74892f-41d0-493f-9a70-608d3bcdd8ed)
![newplot (4)](https://github.com/user-attachments/assets/563c1467-2a51-4788-8060-bcebda356b02)

**Total Sales Month-to-Month**
![newplot (5)](https://github.com/user-attachments/assets/b6a3ad4f-54ec-4ed5-a360-522a592644e8)

Seasonality Insights: Sales showed clear seasonal spikes in March and August every year, driven by heightened consumer demand.

Annual Comparison: Sales revenue in 2023 outperformed the previous two years, reflecting strong growth momentum.

**Order Volume Month-to-Month**
![newplot (6)](https://github.com/user-attachments/assets/593469e8-601f-4540-996d-28a4eafc3299)

Yearly Trends: 2023 recorded the highest overall order volume.

Monthly Peak: March consistently had the highest order volume across all three years.

**Average Order Value (AOV) Month-to-Month**
![newplot (7)](https://github.com/user-attachments/assets/94070036-3af5-4925-89b2-f2483712d9a6)

Peak Year: 2022 had the highest AOV, attributed to the economic impact of the COVID-19 pandemic, which shifted purchasing behaviors toward higher-priced products.

**Sales Month-to-Month by Loyalty Tiers**

Loyalty Customers:
Consistently purchased more than guest customers.
Exhibited similar purchasing trends over time.
![newplot (8)](https://github.com/user-attachments/assets/575a7d4a-0c69-4fd4-9723-1da77d3820c6)

Guest Customers:
Showed lower overall purchase quantities compared to loyalty members.
![newplot (9)](https://github.com/user-attachments/assets/da986cd7-d45c-4c9b-a595-bc9cb6f8c93d)

**Average Order Value by Loyalty Tiers**
Higher Spend per Order: Loyalty members consistently spent more on average compared to guest customers, favoring premium-priced products.
![newplot (10)](https://github.com/user-attachments/assets/d58adff7-e008-4c85-8457-ea880b171632)

**Packaged Water Sales by Season and Loyalty Tiers**

Year 2021 and 2023:
The Healthy Edge Purified Water dominated sales among guest customers.
![newplot (11)](https://github.com/user-attachments/assets/301c2266-5b55-4906-bca3-76146afac52a)
![newplot (12)](https://github.com/user-attachments/assets/e53edb06-6162-44d3-9823-40d9ec4d8a41)

Other Periods:
Spring Glass Water led sales for both loyalty and guest customers during non-peak periods.

**Root Cause Analysis: Discount Scale on Product Demand**
Taking the popular Spring Glass Water as an example:
Discount Impact: Larger discounts directly correlated with higher product demand, emphasizing price sensitivity among consumers.
 Year 2022:
 
![newplot (13)](https://github.com/user-attachments/assets/8342ed9e-ba97-4a2d-b7f9-d01b6d9f3938)
![newplot (14)](https://github.com/user-attachments/assets/5f535314-f243-4686-85ce-62f76da4eb0b)

Year 2023:
![newplot (15)](https://github.com/user-attachments/assets/0f685f73-1116-4399-9389-c5fc85d0a5ac)
![newplot (16)](https://github.com/user-attachments/assets/888f133b-c15b-4ae8-8d6c-474ef518c8a8)

## **Recommendations**

Optimize Product Promotion Based on Seasonality:

Focus marketing campaigns and promotional efforts in March and August, as these months consistently show the highest sales volume across all years.
Consider introducing limited-time offers or bundled discounts during these peak months to further capitalize on seasonal demand.

Enhance Loyalty Program Offerings:

Given that loyalty customers spend more and purchase higher-priced products, enhance loyalty program incentives to drive retention and engagement.
Provide exclusive discounts or early access to premium products like Spring Glass Water to encourage additional purchases.

Price Sensitivity Strategy:

For highly popular items such as Spring Glass Water, implement tiered discount strategies to maximize demand while maintaining profitability.
Experiment with personalized pricing or discounts for different customer segments (e.g., loyalty vs. guest customers).

Expand the Packaged Water Subcategory:

Invest in promoting Spring Water and Alkaline Ionized Water, as these subcategories consistently outperform others.
Consider diversifying product offerings in the Packaged Water category, targeting different consumer preferences, such as eco-friendly or luxury packaging options.
Develop Targeted Guest Customer Promotions

Guest customers tend to purchase fewer and lower-priced products. Launch campaigns aimed at converting guest customers into loyalty members through first-purchase discounts or special incentives.

Monitor Demand During Discount Events:

Since larger discounts lead to increased demand, carefully monitor inventory levels for popular items like Spring Glass Water during discount events to avoid stockouts and maintain customer satisfaction.

Capitalize on Post-Pandemic Trends:

Given the higher average order value observed in 2022 during the pandemic, investigate lingering consumer preferences for premium or health-focused products and adjust product positioning accordingly.

Leverage Data for Forecasting:

Use historical data to forecast monthly demand patterns and improve supply chain planning, especially for high-demand items in the Water category.
Employ machine learning models to predict demand fluctuations and optimize inventory allocation.

Strengthen Product Marketing by Subcategories:

Promote The Healthy Edge Purified Water more heavily to guest customers in years where it dominates sales. For loyalty customers, tailor messaging around Spring Glass Water and its premium attributes.

Increase Awareness of Premium Products:

Position premium products, like Spring Glass Water, as aspirational choices through targeted digital marketing campaigns, emphasizing their quality and unique features.
