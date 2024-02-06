## Bitcoin-Historical-Data-Analysis

### Project Overview

The dataset contains 4,857,377 rows and 14 columns. The table gave information about transactions carried out between the year 2011 and 2021. The dataset has a timestamp column from which day, month and year were generated to determine the trend of transactions. 

### Data Sources 

Quantum Analytics NG 

### Tool Used:

Power BI 

### Data Cleaning

The data set contained a lot of NaN values which were replaced with 0. - The timestamp column was converted into a date and time column by adding a custom column and using the formula =hashtag#datetime(1970,1,1,0,0,0) + hashtag#duration(0,0,0,[Timestamp]) -I separated the resulting column into date and time, where further values of year, month, day, hours and seconds were generated.

###   DATA VISUALIZATION KPIs
 - Total Transactions = Countrows(bitstampUSD)
   
 - Total Successful Transactions = Calculate ([Total Transactions], 'bitstampUSD[Open]> 0)

-  Average Weighted Price = Average('bitstampUSD'[Weighted_Price]) 

-  Total Weighted Price = Sum(bitstampUSD[Weighted_Price])

 -   Total Volume (Currency) = Sum(bitstampUSD[Volume_Currency])
 
 -  Total Volume (BTC) = Sum(bitstampUSD[Volume_BTC])


### Insight/Charts 
- Volume (Currency) Distribution by Year 

- Weighted Price Distribution by Year

 -  Weighted Price Distribution by month 
 
-  Weighted Price Distribution by Day

 -  Yearly Average Weighted Price 
