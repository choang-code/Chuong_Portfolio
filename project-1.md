<iframe title="Chuong_SalesDashboard_Portfolio - Page 1" width="1024" height="1060" src="https://app.powerbi.com/view?r=eyJrIjoiNTM2YzdiMDktODFjMC00MmFlLTk3OTAtYTM0YjgxZjBmMTE2IiwidCI6IjhjYTllYWNhLTZjNzctNGM5MC1hZTM1LTQ4NjhlMzFiNzRlZSIsImMiOjZ9" frameborder="0" allowFullScreen="true"></iframe>


[Open interactive dashboard](https://app.powerbi.com/view?r=eyJrIjoiNTM2YzdiMDktODFjMC00MmFlLTk3OTAtYTM0YjgxZjBmMTE2IiwidCI6IjhjYTllYWNhLTZjNzctNGM5MC1hZTM1LTQ4NjhlMzFiNzRlZSIsImMiOjZ9)

# Overview

Understanding the sales data from any business can offer insights that will be used to drive key decisions. Using sample sales data obtained from the data science community platform Kaggle, I will clean, analyze, ad visualize a set of monthly spreadsheets.

# End Goal

In this scenario, my supervisor has asked for two deliverables: 

- An Excel spreadsheet with PivotTables with the following information: 

  - Total Sales by Month
  
  - Category Sales by Month
  
  - Both of the previous tables but expressed as a percent of monthly sales/orders (e.g. “40% of January’s sales revenue was derived from Category A”)

- A dashboard created with Power BI with the following information visualized and made interactive:
  
  - Monthly Sales Trend
  
  - Map Showing Sales by State
  
  - Both of the previous visuals should be able to be filtered by the following:  
    
    - Category
    
    - Product
    
    - Date

# Datasets and Files

[Sales2019.zip](https://github.com/choang-code/sales-analysis/raw/main/Sales2019.zip)

* 12 CSV files containing sales and product information throughout 2019

[Chuong_SalesAnalysis_Portfolio.xlsx](https://github.com/choang-code/sales-analysis/raw/main/Chuong_SalesAnalysis_Portfolio.xlsx)

* Completed Excel report with Pivot Tables of the previous dataset

[Chuong_SalesDashboard_Portfolio.pbix](https://github.com/choang-code/sales-analysis/raw/main/Chuong_SalesDashboard_Portfolio.pbix)

* Completed PowerBI report file (the same as the embed preview above)

* Requires both the Sales2019 files and the previous spreadsheet since I had Power BI import from Excel

# Explanation of Source Data

[Sales2019.zip](https://github.com/choang-code/sales-analysis/raw/main/Sales2019.zip)

Source: https://www.kaggle.com/knightbearr/sales-product-data/code 

This sample sales dataset comprises of 12 CSV files (one file for each month of the year). The column headers are as follows:

| Attribute        | Definition & Notes                                                             |
| ---------------- | ------------------------------------------------------------------------------ |
| Order ID         | ID’s are not distinct values because each row is accounts for only one product |
| Product          | The full name of the product purchased                                         |
| Quantity Ordered | The number of items purchased                                                  |
| Price Each       | The price of one product                                                       |
| Order Date       | The full date including time when the order was placed                         |
| Purchase Address | Street, City, State and Zip Code all combined into one column                  |

After combining the CSV files and cleaning them, we will discover that the full dataset contains 185,652 rows or 178,406 distinct orders throughout 2019

# Process

## Excel Power Query

When I am presented with multiple files to combine and analyze, Excel’s Power Query (PQ) tool is the key to processing datasets of this size without having the computer slowing down.  

After launching Power Query, I will redirect PQ to the folder where the 12 CSV files are stored to begin transforming or cleaning the data. 

[](images/F1.png)
