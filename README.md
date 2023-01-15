# E-commerce-data-analysis-sales-strategy
Based on the conclusions from the 2019 sales data, K-sales Mart's strategy for 2020.

One of the biggest US online retailers, Kmart, must decide on its sales plan for 2020 based on information from the previous year's sales in their annual sales review meeting.

This initiative aims to produce significant new information about Kmart's sales for each month of 2019. The information will be utilised to help Kmart's sales team adjust their sales tactics as the year goes on.

# Business Problem Statements
Observations on the following are made:

1.What was the best month for sales?

2.Which city had the highest number of sales?

3.Best time to display advertising to maximize sales?

4.Best-selling product & Why?

5.What products are most often sold together?

# Dataset

.Data belongs to Kmart: A leading online retailer in the US

.Time Period :  January 2019  -  December 2019

.Unique Products:  19

.Total Orders :  178,437

.Cities :  9

.KPI’s : Total Sales, Total Products Sold

# Data Analysis Using Python

1.Loaded data for each month and created a data frame using Pandas.

2.For 2019 sales, an aggregated dataset was created by concatenating multiple datasets together.

3.Data handling for null values and junk data.

4.Preprocessed data to make a filtered dataset.

5.Business problem analysis and their solutions.(visualizations using matplotlib and seaborn library)

### What was the best month for sales?
- Create a new dataset with all records grouped by month 
- Plot the graph using **matplotlib**

<p align="center"><img width="208" alt="image" src="https://user-images.githubusercontent.com/71536311/192696748-f475f862-0ff1-4e29-a02b-8e0677b69bf1.png"></p>
<p align="center"><img width="334" alt="image" src="https://user-images.githubusercontent.com/71536311/192509661-634c5a5b-17a7-4307-974c-bfe12592ee48.png"></p>

### Which city had the highest number of sales?
- Extract the ***“Purchase Address”*** column containing the city information into a separate dataframe.
- Group this dataframe by City and each group will have a sum of all the sales in that city.
- Visualize the graph using **matplotlib**

<p align="center"><img width="250" alt="image" src="https://user-images.githubusercontent.com/71536311/192511499-76c45c52-78bf-4ddd-99e8-82743b7a2a59.png"><img width="343" alt="image" src="https://user-images.githubusercontent.com/71536311/192511185-a8ee21d5-4b57-4a4b-adf2-c5ee322b86be.png"></p>

### Best time to display advertising to maximize sales?
- Extract the ***Hours*** from the ***Order Date***.
- Group the data by Hours and depict the graph using **matplotlib**.

<p align="center"><img width="328" alt="image" src="https://user-images.githubusercontent.com/71536311/192513281-b7957d34-3c44-4814-8e84-ff55da98b1c1.png"></p>

### Best-selling product & Why?
- Determine the sum of the ***"Quantity Ordered"*** by grouping by ***"Product"***.
- Visual representation of the ***Quantity Ordered*** for each ***Product***.

<p align="center"><img width="355" alt="image" src="https://user-images.githubusercontent.com/71536311/192695672-0e959352-4941-468b-b9a3-a97e19d6ebf0.png"></p>

- Let us also see a graphic representation of the ***Prices for each product*** grouped by ***Product***.

<p align="center"><img width="349" alt="image" src="https://user-images.githubusercontent.com/71536311/192696011-4090c566-aa3f-495a-895b-13a82cb0b244.png"></p>

### What products are most often sold together?
- Group the product by the ***Order ID*** to know which products were sold together.
- Find the duplicate values of the ***“Order ID”*** by using the **.duplicated() method**.
- Using **.transform() method**, create a new column called ***"Grouped"*** to combine values from multiple rows into one.
- Drop the duplicates created when products were merged for each order ID.
- Display the top 5 products most often sold together.

<p align="center"><img width="583" alt="image" src="https://user-images.githubusercontent.com/71536311/192694593-737bfc37-5eb9-46c1-ac69-65e08e4f946b.png"></p>

## Tools Used

- **Jupyter Notebook** is used as IDE.
- Among the **Python libraries**, **Pandas** is used for handling and preprocessing data.
- **Plotly, Seaborn**, and **Matplotlib** are used for visualizing plots.

For more details, please go through the Jupyter Notebook attached above.

## Conclusion
- The study above demonstrates unequivocally that ***December***, with around ***$9,226,886***in sales, has the highest sales in 2019.
- The graph indicates that ***San Francisco*** has the most sales.
- The best times to run advertisements are just **before 12 and/or just before 7 o'clock in the evening*** to improve the likelihood that customers will buy the product or products.
- The top selling product is ***'AAA Batteries (4-pack)'***. The top selling products seem to have a correlation with the price of the product. The ***cheaper the product, higher the quantity ordered and vice versa***.


