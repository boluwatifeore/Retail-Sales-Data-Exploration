# Retail-Sales-Data-Exploration

## Table of Contents

- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Project Goals and Objectives](#project-goals-and-objectives)
- [Tools Used](#tools-used)
- [Data Cleaning and Preparation](#data-cleaning-and-preparation)
- [Data Analysis](#data-analysis)
- [Findings](#findings)
- [Recommendations](#recommendations)
- [Limitations](#limitations)


## Project Overview

This analysis focuses on providing an understanding on how various factors such as sales revenue, discount percentages, marketing spend, product category, and store location impact sales performance. By analyzing the retail sales data, the project seeks to identify trends, gain valuable insights on sales performance, and make data driven recommendations.

### Data Sources

The primary datasets used for this project analysis is the "Retail_sales.csv" file which contains detailed information on features such as; Sales Revenue (USD), Units Sold, Discount Percentage, Marketing Spend (USD), Store ID, Product Category, Date, Store Location, Day of the Week, and Holiday Effect.

### Project Goals and Objectives

The project main goals and objectives include;
- To evaluate the effectiveness of Marketing Spend and Discount Strategies.
- To examine how different Seasons and Holidays impact Sales.

### Tools Used

- Microsoft Excel - Data Cleaning, Data Formatting, Data Analysis, and Data Visualization [download here](https://microsoft.com)

### Data Cleaning and Preparation

After the data has been downloaded and imported into Ms Excel, I prepared the data for analysis by carrying out the following tasks;
1. Create a New Working Sheet - This is to able to keep the original data intact, allow for mutiple analyses and also enable reusability when neccesary.
2. Check for and Remove Dupiclates.
3. Format date column into 'Short Date' in the home tab.
4. Format Sales Revenue into 'Currency' and remove decimal places.
5. Format Discount Percentage column into actual percentages instaed of numbers "Discount% Fixed"
6. Create categories for Discount% and Marketing Spend for a clearer and better understandable analysis.
7. Create Year Quarter column.

### Data Analysis

```Excel
=IF(G2>10%,"High Discount",IF(G2>=1%,"Low discount","No Discount"))
```
```Excel
=IF(I2>=150,"Very High Spend",IF(I2>=100,"High Spend",IF(I2>=50,"Medium Spend",IF(I2<50,"Low Spend"))))
```
```Excel
=TEXT(C2:C30001,"mmm")
```

### Findings

After analysis, I came up with the following findings;

- With a maximum spend of $199 on marketing, the low spend category ($0-49) yielded the highest sales revenue of $51,481,352, making up a substantial portion of the total sales revenue. On the other hand, the medium($50-99), high($100-149), and very high($150-199) spend yielded relatively similar sales revenue of $10,430,323, $10,328,823, and $10,244,789, respectively which demonstrates that investing a high amount of money in marketing may not be as efficient compared to a lower marketing budget.

  
- I also found that the highest sales revenue was generated when no discount was applied to products, with $280,072 in total sales, followed by low discounts(1-10%) generating $54,303, while  the high discount(10-20%) category had the lowest sales revenue of $32,583 which suggests that giving high discounts on products may not neccessarily boost revenueand customers may be purchasing more items without discounts, or discounts may be applied to less profitable products.


- Another finding was that in Q1, Q2,and Q3, the average sales revenue is consistent with $18,032,144, $19,960,587, and $21,814,665 respectively for each season, with no holiday effect impacting these quarters. However, In Q4, sales show an increase, especially when there is a holiday effect with a total of $22,677,922 in sales revenue. This suggests that holidays during this quarter (mostly around major end-of-year events) significantly generate higher sales.

- Electronics happens to be the highest-performing product category, generating $29,414,541, making up the largest share of the total sales revenue. Furniture followed with $22,913,106, and Clothing at $19,952,025. However, Groceries was the least-performing product category with $10,205,617 in sales revenue.


### Recommendations

Based on my findings, I recommend the following;

- Apply discounts more strategically, for example, giving more targetted discount to low-performing categories like Groceries, which is more likely to bring about interest in consumers and thereby increasing sales without having to give discounts to products that are already selling well.

- Strategize with marketing spend budget by highly focusing on efficient spending and targetted campaigns, e.g, since more sales are made during Q4, run special promotions and campaigns on best selling products like electronics and furnitures in the months leading up to the holiday season which will most likely lead to even more sales revenue.

- Consider selling products that are related to product categories that already generate the most sales revenue which futher boosts sales revenue.

- Consider staying updated with trends, mostly regarding least performing product categories like Groceries, for example, taking notes and adopting strategies taken by competitors who do exceptionally well with such kind of product.


### Limitations

While trying to input the month and year slicers in my visualization dashboard to further gain insights into my analysis, I had realized there were some other values that aren't supposed to be included in each slicers, for example, the slicer for months of the year had Jan to Dec including values such as '21/09/22*'in two fields, which got me very confused and even after trying sveral ways to fix the error, it wasn't working. After several hours, I was able to eventually find my way around fixing the error.
