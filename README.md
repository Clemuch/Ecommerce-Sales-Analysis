# E-Commerce Sales Analysis

## Table of Content
- [Introduction](#introduction)
- [Project Overview](#project-overview)
- [Data Source](#data-source)
- [Tools](#tools)
- [Frame work](#frame-work)
- [Data Cleaning and Preparation](#data-cleaning-and-preparation)
# Introduction

The CSV file contains data related to e-commerce sales, comprising 9,994 rows and 22 columns. Each row represents an order with details such as:

- **Order Information**: `Row ID`, `Order ID`, `Year`, `Order Date`, `Ship Date`, `Ship Mode`.
- **Customer Details**: `Customer ID`, `Customer Name`, `Segment`.
- **Location Details**: `Country`, `City`, `State`, `Postal Code`, `Region`.
- **Product Information**: `Product ID`, `Category`, `Sub-Category`, `Product Name`.
- **Sales Metrics**: `Sales`, `Quantity`, `Discount`, `Profit`.

This dataset provides an overview of orders, shipping details, customer segments, product categories, and financial metrics, which can be useful for analyzing sales performance, customer trends, and profitability.

## Project Overview
The e-commerce sales data document consists of 22 attributes, capturing various details about each transaction, from order specifics to customer demographics and financial performance. Here’s a summary of each section:

1. Order and Shipping Details:

- Order ID, Row ID: Unique identifiers for each order and row entry.
- Year, Order Date, Ship Date: The year and dates when the orders were placed and shipped.
- Ship Mode: Delivery methods (e.g., Standard Class, Second Class).
2. Customer Information:

- Customer ID, Customer Name: Identifiers and names of customers.
- Segment: Customer segmentation into categories like Consumer, Corporate, etc.
3. Geographical Data:

- Country, City, State, Postal Code, Region: Location information indicating where customers are based.
4. Product and Category Information:

- Product ID, Category, Sub-Category, Product Name: Unique product identifiers, main categories (e.g., Furniture, Office Supplies), sub-categories (e.g., Bookcases, Chairs), and detailed product names.
5. Sales Performance Metrics:

- Sales, Quantity, Discount, Profit: Financial attributes indicating the sales amount, quantity sold, discount applied, and profit generated for each order.

The dataset is well-suited for analysis on topics such as sales trends, customer behavior, regional performance, and profitability analysis across products and customer segments.

## Data Source
The primary dataset used in this analysis is gotten from kaggle. You can also get the dataset direct from kaggle [here](https://www.kaggle.com/datasets/abhishekchauhan001/ecommerce-sales) or make use of the one uploaded in here.

### Tools 
Python language was used for;
1. Data Cleaning
2. Exploratory Data Analysis (EDA)
3. Visualization (Matplotlib library)

### Frame work
1. Pandas.
2. Matplotlib
3. Seaborn.
4. Plotly
5. Sklearn.
6. Scipy

### Data Cleaning and Preparation
During the data preparation phase, we performed the following task;
1. Data loading using pandas
2. Data validation
   - Handling for missing values
   - Handling inconsistency in data type
   - Handling duplicates
### Exploratory Data Analysis (EDA)
1. How much sales are made by city?

![salesByCity](https://github.com/user-attachments/assets/ffe26e29-8e63-479b-8023-f3485fba29d4)
There are 528 cities in the dataset. New York City had the highest sales of all the cities in the dataset. It accounted for over 256,000 dollars in sales.

2. How much sales are made by state?
   
![SalesByState](https://github.com/user-attachments/assets/e62c476a-3fca-4e55-a6ea-a6e89d0af27c)
California made the highest sales among all the states, while North Dakota made the least sales.

3. How much sales are made by region?
   
![SalesByRegion](https://github.com/user-attachments/assets/7991d625-3e9f-4836-a64d-9ee379b85e08)
The West region has the highest sales, followed by the East, Central, and South regions.

4. What percentage are made by each region?
   
![SalesPercentageByRegion](https://github.com/user-attachments/assets/d18864a9-6ff1-4ebb-8666-261397908559)
The West region accounts for 31.6% of total sales. The East region is second with 29.5%, followed by the Central region with 21.8%, and the South region with 17.1%.

5. List the top ten product with the highest sales?
   
![TopTenProducts](https://github.com/user-attachments/assets/657d58be-02d6-4079-a026-6fd638d08ead)
The bar graph indicates that the Canon ImageClass 2200 Advanced Copier has the highest sales of $61599.824

6. Which product made the highest sales and which month did they made the highest sales?
   
   |Product Name|Month Name|Sales|
   |------------|----------|-----|
   |Canon imageCLASS 2200 Advanced Copier|October|$28699.918|

7. Does discount increase sales? How does discount affect sales? Does a higher discount result in higher sales?

![CorrDiscount](https://github.com/user-attachments/assets/361590de-76e7-451a-a183-237dc1e3b595)

Let's plot the distribution curve of Yeo-Johnson transformed data  
![transformedKdePlot](https://github.com/user-attachments/assets/bf4a14ec-f8c9-4078-b8b3-687e543d958b)

Let's see the scatter plot for the transformed discount sales
![discountSalesYeoJohnson](https://github.com/user-attachments/assets/e7ef769f-1e3f-404f-8569-1fafce598eda)

- After transforming the data, we can see that there is no relationship between sales and discount.
- Discount does not cause increase in sales.
- Higher discount does not result in higher sales.
  ### Recommendation
- To keep the profit margins high and ensure a healthy bottom line, the discount rate should be reduced to a minimum.

8. Does Sales differs significantly across region?
   
|ANOVA Result|
|------------|
|F-statistic: 0.8006|
|p-value: 0.4933|
Sales does not differs significantly across region. 

9. Which category made the highest sales?
    
![SalesByCategory](https://github.com/user-attachments/assets/48e0cafd-7e89-4765-8c35-7a74bebc28d7)
Technology has the highest sales, followed by furniture and office supplies. The difference between the highest and lowest sales categories exceeds 10%.

10. Does sales varies significantly across category?

|Category ANOVA Result:|
|----------------------|
|F-statistic: 265.4898|
|p-value: 0.0000|
Sales varies significantly across categories.

 The significant result implies that product categories play a critical role in determining sales patterns. Businesses can leverage this insight by:

- Customizing marketing strategies for each category to capitalize on its strengths.
- Optimizing discount levels to maximize sales without compromising profits in high- or low-value categories.
- Segmenting customers further within each category to better understand their purchasing behaviors.
  
11. Which Customer Segment drives the highest sales?
    
![CustomerSegmentSales](https://github.com/user-attachments/assets/e2c0617d-b5d5-4c27-90ac-6e2e614c6d54)

Consumer drives the highest sales for the company.

12. Which sub category caused the highest sales?

![subCat](https://github.com/user-attachments/assets/f2badf99-1aeb-4ef6-b928-33b9ba620881)

Phones had the highest sales among the technology products. Phones also had the highest sales among the subcategories.



