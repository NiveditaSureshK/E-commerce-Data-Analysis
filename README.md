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
- **Total Orders :**  178437
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
- Visualize the graph using **matplotlib**

<p align="center"><img width="334" alt="image" src="https://user-images.githubusercontent.com/71536311/192509661-634c5a5b-17a7-4307-974c-bfe12592ee48.png"></p>

### Which city had the highest number of sales?
- Extract the ***“Purchase Address”*** column containing the city information into a separate dataframe.
- Group this dataframe by City and each group will have a sum of all the sales in that city.
- Visualize the graph using **matplotlib**

<p align="center"><img width="250" alt="image" src="https://user-images.githubusercontent.com/71536311/192511499-76c45c52-78bf-4ddd-99e8-82743b7a2a59.png"><img width="343" alt="image" src="https://user-images.githubusercontent.com/71536311/192511185-a8ee21d5-4b57-4a4b-adf2-c5ee322b86be.png"></p>

### Best time to display advertising to maximize sales?
- Extract the Hours from the ***Order Date***.
- Group the data by Hours and visualize the graph using **matplotlib**.

<p align="center"><img width="328" alt="image" src="https://user-images.githubusercontent.com/71536311/192513281-b7957d34-3c44-4814-8e84-ff55da98b1c1.png"></p>

### Best-selling product & Why?
- 

### What products are most often sold together?
- Group the product by the ***Order ID*** to know which products were sold together.
- Find the duplicate values of the ***“Order ID”*** by using the **.duplicated()** method.
- Using **.transform()** method, create a new column called ***"Grouped"*** to combine values from multiple rows into one.
- 

## Tools Used
![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)   ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)   ![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)   ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)   ![Matplotlib](https://img.shields.io/badge/Matplotlib-%23#ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=white)   ![Plotly](https://img.shields.io/badge/Plotly-%233F4F75.svg?style=for-the-badge&logo=plotly&logoColor=white)

- Jupyter Notebook is used as IDE.
- Among the Python libraries, Pandas and NumPy are used for handling data, preprocessing, and mathematical functions, respectively.
- Plotly, Seaborn, and Matplotlib are used for visualizing plots.

For more details, please go through the Jupyter Notebook attached above.

## Conclusion



