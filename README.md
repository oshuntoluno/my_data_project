## Global superstore-sales-analysis
An exploratory data analysis of 5,009 Superstore transactions (2014–2017) reveals that discounts above 20% significantly reduce profitability and frequently generate losses.

# Question

Which product categories and regions drive the most profit for the Superstore, and at what discount level does profitability begin to decline?

# Dataset

* Source: Global Superstore dataset (commonly used retail analytics dataset)

* Size: 5,009 rows × 22 columns

* Time period: January 3, 2014 – December 30, 2017

# Key fields:

* Order Date – Date of transaction

* Region – Sales region (East, West, Central, South)

* Category – Product category

* Sales – Revenue per transaction

* Profit – Net profit per transaction

* Discount – Discount applied (0–0.8)

* Quantity – Units sold

* Profit_Margin – (Profit ÷ Sales)

# Tools Used

* Microsoft Excel (Power Query + Pivot Tables)

* Power Query (data transformation)

* Git

* GitHub

# Key Findings
* The East region generates the highest total profit of 52,445.63, while the West region generates the highest revenue of 332,443.71.
  
* Technology is the primary profit driver with a total of 70,157.57
  
* Furniture has very weak profitability with a total of 7,569.17
  
* Profit becomes negative after 20% discount.

Discounts above 30% cause severe erosion of profitability.
The 50–60% band shows the worst performance (-323.88 average profit).
![Discount_impact_chart](https://github.com/user-attachments/assets/0fe094f9-f782-41e8-b2e2-ea6962c7277d)

Explanation:

The line chart shows a clear downward trend in profitability as the discount increases. The curve crosses below zero at the 30–40% band, indicating a structural loss threshold.

# How to Reproduce

Clone this repository

Open data/raw/global_superstore.csv

Use Power Query to:

Fix data types

Create Profit_Margin column

Extract Order Year

Close & Load to Excel

Create Pivot Table:

Rows → Discount (Grouped by 0.1)

Values → Average Profit, Sum of Profit

Interpret threshold where Avg Profit < 0

## What I’d Do Next

Analyze discount impact by category (Is Furniture driving losses?)

Build a profitability dashboard

Model optimal discount threshold

Investigate regional discount strategies
