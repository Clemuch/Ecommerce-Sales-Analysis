# E-Commerce Sales Analysis

## Table of Content
- [Introduction](#introduction)
- [Project Overview](#project-overview)
- [Data Source](#data-source)
- 
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

### DataFrame work
1. Pandas.
2. Matplotlib
3. Seaborn.
4. Plotly
5. Sklearn.
6. Scipy

### Data Cleaning/Preparation
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
5. List the top ten product with the highest sales?
6. Which product made the highest sales and which month did they made the highest sales?
7. Does discount increase sales? How does discount affect sales? Does a higher discount result in higher sales?
8. Does Sales differs significantly across region?
9. Which category made the highest sales?
10. Does sales varies significantly across category?
11. Which Customer Segment drives the highest sales?
12. Which sub category caused the highest sales?
### Results/Findings
The analysis result are summarized as follows:
1. There are 528 cities in the dataset. New York City had the highest sales of all the cities in the dataset. It accounted for over 256,000 dollars in sales.
2. California made the highest sales among all the states, while North Dakota made the least sales.
3. The West region has the highest sales, followed by the East, Central, and South regions.
4. The West region accounts for 31.6% of total sales. The East region is second with 29.5%, followed by the Central region with 21.8%, and the South region with 17.1%.
5. Top ten products with the highest sales:
   |Product Name                                                                  | Sales
   Canon imageCLASS 2200 Advanced Copier                                          61599.824
   Fellowes PB500 Electric Punch Plastic Comb Binding Machine with Manual Bind    27453.384
   Cisco TelePresence System EX90 Videoconferencing Unit                          22638.480
   HON 5400 Series Task Chairs for Big and Tall                                   21870.576
   GBC DocuBind TL300 Electric Binding System                                     19823.479
   GBC Ibimaster 500 Manual ProClick Binding System                               19024.500
   Hewlett Packard LaserJet 3310 Copier                                           18839.686
   HP Designjet T520 Inkjet Large Format Printer - 24" Color                      18374.895
   GBC DocuBind P400 Electric Binding System                                      17965.068
   High Speed Automatic Electric Letter Opener                                    17030.312
6. The product that maed the highest sales and month:
   Product Name    Canon imageCLASS 2200 Advanced Copier
   Month_Name                                        Oct
   Sales                                       28699.918
7. 
'''python

df = pd.read_csv('Ecommerce Sales Analysis.csv')

'''


