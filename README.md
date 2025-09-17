# E-commerce Transaction Analysis

### Project Overview

From different branches of this retail company, a 7000-row e-commerce transaction dataset was given to me. This report was written to guide the company through statistical insights to make better decisions with regards to what product to sell, which products generates the most revenue, what region they make the most sales and generate the most income at.

### Data Source

Copy of August Data Challenge: The primary dataset used for this analysis was the "Copy of August Data Challenge.xlsx" containing detailed information about the company's transaction and sales

### Tools

- Excel - Data Cleaning & Transformation
- Excel - Data Analysis
- Power Bi - Visualization

### Data Cleaning/Preparation

In the initial data preparation phase, I performed the following tasks:
1. Data loading & Inspection
2. Handling missing values
3. Removing duplicates
4. Data cleaning and formatting
5. Analysis
6. Visualization

### Exploratory Data Analysis (EDA)

EDA involved exploring the data to answer key questions such as:
- What is the total number of unique customers?
- What is the highest-selling product by revenue (USD)?
- What is the Region with the highest total profit?
- What is the total sales for 2024 (USD)?
- What is the average quantity sold (in kg) after cleaning?

### Data Analysis

Revenue is calculated by multiplying the Quantity (Kg) by the UnitPrice (USD) per customer. The Total Sales is gotten by summing up the Revenue. Profit is gotten by multiplying the Total Sales by the percentage margin. To get the total price, subtract the product of the Discount and Revenue from the Revenue (Revenue-(Discount * Revenue)). I used Pivot Tables to find the SUM of the Revenue, Quantity and Profit. To find the number of unique customers, use the UNIQUE formular to find them then use the COUNTA to count them

```excel
=COUNTA(UNIQUE(E_commerce[CustomerName]))
```

### Results/Findings

The analysis results are summarized as follows:
1. There are a total of 334 unique customers
2. Electronics > Mobile Phones > Feature Phones was the highest selling product by Revenue
3. Kano had the highest total Profit
4. 442,900,553.94 was the total sales for 2024
5. 5.41 is the average quantity sold

### Recommendations

Based on the analysis, I recommend the following actions:
- More products can be supplied to regions with low sale. Regions like Kano and Lagos 
- General sales of Beauty & Personal Care > Skincare products is low, this product can be supplied to regions where it has low sales. Specifically Oyo and Kaduna
- Electronics > Mobile Phones > Smartphones is low in sales too, FCT and Anambra can be be supplied with more of this product to increase sales

### Limitations

There where a lot of missing values in this dataset. Missing values can be found in the Discount and the Delivery date coulumns. These empty cells were replaced with "N/A" 

### References

None
