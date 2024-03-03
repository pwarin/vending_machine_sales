# Project Description
This is a data visualisation project of vending machine sales from 2000+ vending machines in Central New Jersey, year 2022.
Data source: https://www.kaggle.com/datasets/awesomeasingh/vending-machine-sales

Aim of the project was to create a sales performance dashboard of vending machine sales using Power BI to easily visualise key performance metrics such as monthly revenue, categorical popularity and product ranking.
Key skils used:
- **Microsoft Excel**: Initially visualise and interpret the dataset
- **Python**: Cleanse and transform the dataset appropriately for Power BI dashboard, primarily using the Pandas library
- **Power BI**: Visualise a sales performance dashboard of the vending machines in a succint and interactive manner

# Notes for Repository Files

## vending_machine_sales.csv
Original dataset imported from kaggle. 
This file has the following attributes

Status : Represents if the machine data is successfully processed
Device ID : Unique electronic identifier ( also called as ePort) for the vending machine. A machine is allocated a unique ePrt * device
Location : Indicates location of the vending machine
Machine : User-friendly machine name
Product : Product vended from the machine
Category : Carbonated / Food / Non-carbonated / Water
Transaction : Unique identifier for every transaction
TransDate : The Date & time of transaction
Type : Type of transaction ( Cash / Credit )
RCoil : Coil # used to vend the product
RPrice : Price of the Product
RQty : Quantity sold. This is usually one but machines can be configured to sell more items in a single transaction
MCoil : Mapped coil # used to vend the product ( from toucan )
MPrice : Mapped price of the Product
MQty : Mapped quantity sold. This is usually one but machines can be configured to sell more items in a single transaction
LineTotal : Total sale per transaction
TransTotal : Represents total of all transactions that will show up on the Credit Card. A user could vend a drink for $3 and a snack for $1.5 making a total of $4.50
Prcd Date : Date when the transaction was processed by SeedLive ( an entity that is used to aggregate all transactions electronically )

## Vending_Machine_Sales_Data_Cleansing.ipynb
This jupyter notebook contains the code used to cleanse and tranform the vending_machine_sales.csv dataset and outputting the transformed_vending_machine_sales.csv dataset.
Cleansing steps executed:
- Duplicates identifed and amended
- Uniformised date format
- Irrelevant attributes identifed and dropped for simplification
- Renamed attributes for simplification and clarity

## transformed_vending_machine_sales.csv
Final cleansed and transformed dataset used for data visualisation in Vending_Machine_Sales_Visualisation.pbix

## Vending_Machine_Sales_Visualisation.pbix
Power BI dashboard visualising the key sales performance metrics inclyding total revenue, items sold, revenue by month, product ranking and more.
To navigate the filter options, please follow the steps below:
- Open the 'Filters' plane on the right hand side
- Select the visual / chart the filter to be utilised upon
- Select the attribute to filter, eg. 'Month'
- Filter by selecting desired attributes, excluding selected attributes, or use the dropdown search bar

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
If you have read this far, I really appreciate your time and effort. 
God bless you and have a wonderful day.
