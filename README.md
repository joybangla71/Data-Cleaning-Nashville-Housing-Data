# Data-Cleaning-Nashville-Housing-Data

Data Source: https://github.com/AlexTheAnalyst/PortfolioProjects/blob/main/Nashville%20Housing%20Data%20for%20Data%20Cleaning.xlsx

First, the data is downloaded from the source, loaded into SQL server, renamed appropriately and viewed using the SELECT * statement. Upon looking at the SaleDate column, it is clear that this column contains data in the datetime format which is unnecessary for analytic purposes and so we want to standardize this column so that it only contains dates. This is done in the Standardize Date Format section of the SQLQueries_NashvilleHousing_Dataset.sql file.

Next, upon examining the PropertyAddress and OwnerAddress columns we see that these columns include city and state names. We want to seperate the addressess from cities and states which makes the data much more useful. This is shown in Populate Property Address data and Breaking out Address into Individual Columns (Address, City, State) sections in the SQL file.

Another interesting column is the SoldAsVacant which shows that it has four different data: 'Yes', 'No', 'Y' and 'N'. To make this consistent, 'Y' should be replaced with 'Yes', 'N' should be replaced with 'No' or vice versa. This is done in the Change Y and N to Yes and No in "Sold as Vacant" field section of the sql script.

Finally, duplicate data and unsued data are removed in order to create a more robust and analysis ready dataset.
