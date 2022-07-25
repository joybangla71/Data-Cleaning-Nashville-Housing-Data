# Data-Cleaning-Nashville-Housing-Data

Data Source: https://github.com/AlexTheAnalyst/PortfolioProjects/blob/main/Nashville%20Housing%20Data%20for%20Data%20Cleaning.xlsx

First, the data is downloaded from the source, loaded into SQL server, renamed appropriately and viewed using the SELECT * statement. Upon looking at the SaleDate column, it is clear that this column contains data in the datetime format which is unnecessary for analytic purposes and so we want to standardize this column so that it only contains dates. This is done in the Standardize Date Format section of the 
