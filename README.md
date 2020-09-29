# Forecasting-US-Interest-rate-R
***Script method output***

This repository contains the data behind the "Forecasting the US interest rate from 1970 to 2020" using R, and the code that I used to clean, analyse and present the numbers.

Cleaning_script.R: 

-This imports raw data from various sources, but mostly in FRED ( historical time seriesmonthly). 

Data_source.R:

-For interest-rate variables, the data incomplete might be removed.

-For the macro-economic avariable: the GDP (quarterly) where the month has missing data, its missing value will equal the quarterly GDP value.

Notes: The dataset are obtained form number of statistic bureases, goverment departments. The source documents in the link:.... (folder/link). All most the data are automatically downloaded from the offical websites. The full of list of source and links are collated in a filed called .....(links)

Method:

- Using the main VAR to predict the interest rates, and an additional model such as AR, that will have a good comparison. 

- Combine with the Cross-validation time series data will increase the accurate prediction. 


