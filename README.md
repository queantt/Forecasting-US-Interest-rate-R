# Forecasting-US-Interest-rate-R
***Script method output***

This repository contains the data behind the "Forecasting the US interest rate from 1970 to 2020" using R, and the code that I used to clean, analyse and present the numbers.

Cleaning_script.R: 

- This imports raw data from various sources, but mostly in FRED (historical time series monthly). 

Data_source.R:

- For interest-rate variables, the data incomplete might be removed.

- For the macro-economic avariable: the GDP (quarterly) where the month has missing data, its missing value will equal the quarterly GDP value.

Notes: The dataset are obtained form number of statistic bureases, goverment departments. The source documents in the link:.... (folder/link). All most the data are automatically downloaded from the offical websites. The full of list of source and links are collated in a filed called at the links as below:

Macro variables:
 
 - Inflation (CPI): monthy https://fred.stlouisfed.org/series/FPCPITOTLZGUSA
 
 - Real Gross Domestic Product: using the real GDP growth rate, quarterly https://fred.stlouisfed.org/series/A191RL1Q225SBEA
 
 - Unemployment Rate (UN): monthly  https://fred.stlouisfed.org/series/UNRATE
 
 Interest rate variables:
 
 - 1- month Treasury Bill (1 mth): https://fred.stlouisfed.org/series/TB4WK
 
 - 3-Month Treasury Bill (3 mth): https://fred.stlouisfed.org/series/TB3MS
 
 - 12 Month Treasury Bill (12 mth): https://fred.stlouisfed.org/series/TB1YR
 
 - 3-Year Treasury Bond (36 mth): https://fred.stlouisfed.org/series/GS3
 
 - 5-Year Treasury Bond (60 mth): https://fred.stlouisfed.org/series/GS5

Method.R:

- Using the main VAR to predict the interest rates, and an additional model such as AR, that will have a good comparison. 

- Combine with the Cross-validation time series data will increase the accurate prediction. 
