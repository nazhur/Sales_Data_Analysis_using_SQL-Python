# Retail Sales Orders Data Analysis Project using SQL + Python

## Overview

This project focuses on analyzing retail sales orders data using SQL and Python. The dataset was downloaded using the Kaggle API into a Jupyter Notebook environment. Data cleaning and transformation were performed using Pandas to prepare the data for analysis. The cleaned data was then loaded into a MySQL database using SQLAlchemy and mysql-connector-python libraries.

Kaggle Dataset link: https://www.kaggle.com/datasets/ankitbansal06/retail-orders

## Project Architecture

![project_architecture](https://github.com/nazhur/Sales_Data_Analysis_using_SQL-Python/assets/125865054/f9e01f62-1797-45dd-b28d-5097b70457c6)

## Instructions

Before loading the data into MySQL Workbench, it's necessary to create a new database in MySQL Workbench with the desired name, which will be used in the code. Additionally, while loading the data into the MySQL database, it's important to note the issue regarding incorrect data types. To address this, a table with column names and proper data types should be created prior to using the code snippet:

df.to_sql('df_orders', con=conn, index=False, if_exists='append')

Make sure to use 'append' instead of 'replace'

This code ensures that the correct data is loaded into the MySQL database.

## Analysis Questions

The following questions were addressed using MySQL in this analysis:

1. **Top 10 Highest Revenue Generating Products**
   - Identifying the top 10 products with the highest revenue.
  
  ![sales_project_top10](https://github.com/nazhur/Sales_Data_Analysis_using_SQL-Python/assets/125865054/cff10dad-74da-4c75-b0ae-47457eca3fb2)

2. **Top 5 Highest Selling Products in Each Region**
   - Determining the top 5 highest selling products in each region.
  
  ![Sales_Top5_high_inRegion](https://github.com/nazhur/Sales_Data_Analysis_using_SQL-Python/assets/125865054/8657f617-05ae-4fd5-adb5-6326fad9e6bf)


3. **Month Over Month Growth Comparison (2022 vs. 2023 Sales)**
   - Comparing the sales growth month over month between 2022 and 2023.

  ![sales_MOM](https://github.com/nazhur/Sales_Data_Analysis_using_SQL-Python/assets/125865054/17ab414e-2808-4809-a8a1-b2338b81a49d)


4. **Highest Sales Month for Each Category**
   - Identifying the month with the highest sales for each category.
  
  ![sales_month _high](https://github.com/nazhur/Sales_Data_Analysis_using_SQL-Python/assets/125865054/4bd06139-8fb0-4fd4-b6b0-cf1dfd03f330)


5. **Subcategory with Highest Growth by Profit in 2023 compared to 2022**
   - Analyzing the subcategory with the highest growth in profit from 2022 to 2023.
  
  ![sales_subcategory](https://github.com/nazhur/Sales_Data_Analysis_using_SQL-Python/assets/125865054/9a81be96-23bf-4371-865f-497bd7f168a1)

  ![sales_subcategory_full](https://github.com/nazhur/Sales_Data_Analysis_using_SQL-Python/assets/125865054/f5f78428-64d6-48c3-8df8-ca4d8ce2900c)


## Project Structure

- `Data Pulling and Cleaning using Pandas.ipynb`: Jupyter Notebook containing the data fetching and data transformation code.
- `Data Analysis using SQL`: This file containing the questions and answer part, where SQL has been used to answer those questions.
- `README.md`: This README file providing an overview of the project.

## Conclusion

In this project I have demonstrates the use of SQL and Python for retail sales orders data analysis. By leveraging these tools and techniques, valuable insights were obtained, enabling informed decision-making for business optimization and strategy development.






