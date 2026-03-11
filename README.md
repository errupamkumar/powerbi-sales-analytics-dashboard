# Power BI Sales Analytics Dashboard

## Overview

This project presents an interactive **Sales Analytics Dashboard** built using Microsoft Power BI. The dashboard provides comprehensive insights into sales performance, customer behavior, product performance, and geographic distribution.

It is designed to help business stakeholders monitor KPIs, analyze trends, and make data-driven decisions.

---

## Key Features

- Executive level KPI dashboard
- Revenue trend analysis
- Geographic sales distribution
- Product performance analysis
- Customer insights and segmentation
- Interactive filtering and drill-down capabilities

---

## Dashboard Pages

### 1. Executive Dashboard

The executive dashboard provides high-level business KPIs including:

- Total Revenue
- Total Profit
- Total Orders
- Return Rate

Additional insights include:

- Revenue trending over time
- Orders by product category
- Top 10 performing products
- Monthly revenue, orders, and returns comparison
- Most ordered and most returned product types

---

### 2. Geographic Sales Map

This page visualizes sales distribution across different regions using an interactive map.

Key features:

- Sales by region
- Geographic distribution of customers
- Interactive filters for:
  - Europe
  - North America
  - Pacific region

This allows users to quickly identify high-performing markets.

---

### 3. Product Detail Analysis

This page focuses on analyzing the performance of individual products.

Key insights:

- Monthly orders vs target
- Monthly revenue vs target
- Monthly profit vs target
- Price adjustment simulation
- Profit comparison (Actual vs Adjusted)
- Product metric selection (Orders, Revenue, Profit, Returns)

This helps evaluate product-level performance and pricing strategies.

---

### 4. Customer Detail Analysis

This dashboard provides insights into customer behavior.

Key insights:

- Total unique customers
- Revenue per customer
- Customer revenue trend over time
- Top 100 customers by revenue
- Orders by income level
- Orders by occupation
- Identification of top revenue generating customer

---

## Technologies Used

- Microsoft Power BI Desktop
- DAX (Data Analysis Expressions)
- Data Modeling
- Interactive Data Visualization
- Bing Maps Integration

---

## Key KPIs

The dashboard tracks several important metrics:

- Revenue
- Profit
- Orders
- Return Rate
- Revenue per Customer
- Customer Distribution
- Product Performance

---

## How to Use

1. Download the `.pbix` file from the `report` folder.
2. Open the file using **Microsoft Power BI Desktop**.
3. Refresh the dataset if required.
4. Interact with filters, slicers, and visuals to explore insights.

---

## Project Screenshots

### Executive Dashboard : 

<img width="2067" height="1165" alt="image" src="https://github.com/user-attachments/assets/e012bfa3-327e-4a1c-b6f1-1d90e1fc6cdc" />


### Geographic Map
<img width="2073" height="1161" alt="image" src="https://github.com/user-attachments/assets/7288ba18-b647-4809-a431-8f351213eb41" />


### Product Detail :
<img width="2073" height="1165" alt="image" src="https://github.com/user-attachments/assets/d34a56a8-3365-46bf-a7fe-4fce15f1c5ca" />


### Customer Detail :
<img width="2041" height="1164" alt="image" src="https://github.com/user-attachments/assets/e2f7363f-c799-46e4-a66c-53ae4bae1f30" />

---
## Data Model

The Power BI report is built using a **Star Schema Data Model** to ensure optimized performance and scalable analytics.

The model consists of **fact tables** that store transactional data and **dimension tables** that provide descriptive attributes for analysis.

### Fact Tables

**Sales Data**
- CustomerKey
- OrderDate
- OrderLineItem
- OrderNumber
- OrderQuantity
- ProductKey
- Retail Price
- Revenue
- StockDate

**Returns Data**
- ProductKey
- ReturnDate
- ReturnQuantity
- TerritoryKey

---

### Dimension Tables

**Customer Lookup**
- CustomerKey
- Customer Full Name
- Annual Income
- Birth Year
- Customer Priority

**Product Lookup**
- ProductKey
- Product Name
- Product Color
- Product Cost
- Price Point
- Discount Price

**Product Subcategories Lookup**
- ProductSubcategoryKey
- SubcategoryName
- ProductCategoryKey

**Product Categories Lookup**
- ProductCategoryKey
- CategoryName

**Territory Lookup**
- SalesTerritoryKey
- Country
- Region
- Continent

**Calendar Lookup**
- Date
- Day Name
- Day of Week
- Month
- Month Name
- Month Number

**Rolling Calendar**
- Date
- Start of Month
- Start of Quarter
- Year

---

### Supporting Tables

**Price Adjustment (%)**
Used to simulate pricing changes and analyze their impact on revenue and profit.

**Measure Table**
Stores calculated measures created using DAX for cleaner model organization.

---

### Data Model Diagram :

Below is the relationship model used in the Power BI report.

<img width="1820" height="1073" alt="image" src="https://github.com/user-attachments/assets/8f86b5c3-093b-4e7a-82a1-90f98f1765fc" />


---

### Model Design

The data model follows best practices:

- Star schema structure
- Dimension tables connected to central fact tables
- Optimized relationships for fast filtering
- Separate measure table for DAX calculations
- Lookup tables used for hierarchical analysis

This structure ensures high performance and scalable reporting.
---

## Business Value

This dashboard enables business users to:

- Monitor overall business performance
- Identify high-performing products
- Analyze customer purchasing behavior
- Understand geographic sales trends
- Make strategic decisions based on data insights
  
## Author

**Rupam Kumar**

Power BI Developer | Data Analytics Enthusiast
