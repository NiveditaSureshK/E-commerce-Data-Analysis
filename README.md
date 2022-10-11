# E-commerce-Data-Analysis for Sales Strategy

In their annual sales review meeting, Kmart, one of the largest online retailers in the US, must decide on their sales strategy for 2020 based on insights from the 2019 sales data.

This project focuses on generating key insights regarding Kmart's sales for each month of 2019. The data will be used to assist Kmart's sales team in fine-tuning sales strategies as the year progresses.

## Business Problem Statements
Observations on the following are made:
1. What was the best month for sales?
2. Which city had the highest number of sales?
3. Best time to display advertising to maximize sales?
4. Best-selling product & Why?
5. What products are most often sold together?

## Dataset

- **Data belongs to Kmart:** A leading online retailer in the US
- **Time Period :**  January 2019  -  December 2019
- **Unique Products:**  19
- **Total Orders :**  178,437
- **Cities :**  9
- **KPI’s :** Total Sales, Total Products Sold

## Data Analysis Using Python

1. Loaded data for each month and created a data frame using Pandas.
2. For 2019 sales, an aggregated dataset was created by concatenating multiple datasets together.
3. Data handling for null values and junk data.
4. Preprocessed data to make a filtered dataset.
5. Business problem analysis and their solutions. (visualizations using matplotlib and seaborn library)

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
![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)   ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)   ![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)   ![Matplotlib](https://img.shields.io/badge/Matplotlib-%23#ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=white)   ![Plotly](https://img.shields.io/badge/Plotly-%233F4F75.svg?style=for-the-badge&logo=plotly&logoColor=white)

- **Jupyter Notebook** is used as IDE.
- Among the **Python libraries**, **Pandas** is used for handling and preprocessing data.
- **Plotly, Seaborn**, and **Matplotlib** are used for visualizing plots.

For more details, please go through the Jupyter Notebook attached above.

## Conclusion
- The analysis above clearly illustrates that ***month 12 (December)*** boasts the maximum sales in 2019 with roughly ***$9,226,886***.
- According to the graph, ***San Francisco*** has the largest number of sales.
- The optimum time to display advertising to increase the probability of buyers purchasing the product/s is ***shortly before 12 pm and/or right before 7 pm***.
- The top selling product is ***'AAA Batteries (4-pack)'***. The top selling products seem to have a correlation with the price of the product. The ***cheaper the product, higher the quantity ordered and vice versa***.


