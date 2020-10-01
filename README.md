# Forecasting-US-Interest-rate-R
**Script method output**

This repository contains the data behind the "Forecasting the US interest rate from 1970 to 2020" using R, and the code that I used to clean, analyse and present the numbers.

**Cleaning_script.R:**

- This imports raw data from Economic Research Federal Reserve Bank of St. Louis (FRED) (historical time series monthly). 

**Variables with its source:**

All most the data are automatically downloaded from the offical website. These are collated as the links below:

1) Macro variables
 
 - Inflation (CPI): monthy https://fred.stlouisfed.org/series/FPCPITOTLZGUSA
 
 - Gross Domestic Product (GDP): using the real GDP growth rate, quarterly https://fred.stlouisfed.org/series/A191RL1Q225SBEA
 
 - Unemployment Rate (UN): monthly  https://fred.stlouisfed.org/series/UNRATE
 
 2) Interest rate variables:
 
 - 1-month Treasury Bill (1 mth):  https://fred.stlouisfed.org/series/TB4WK
 
 - 3-Month Treasury Bill (3 mth):  https://fred.stlouisfed.org/series/TB3MS
 
 - 1-year Treasury Bill (12 mth):  https://fred.stlouisfed.org/series/TB1YR
 
 - 3-Year Treasury Bond (36 mth): https://fred.stlouisfed.org/series/GS3
 
 - 5-Year Treasury Bond (60 mth):  https://fred.stlouisfed.org/series/GS5
 
**Data_exploration.R:**

- For interest-rate variables, the data incomplete might be removed.

- For the macro-economic avariable: the real GDP (quarterly) where the month has missing data, its missing value will equal the quarterly GDP value.

**Methods.R:**

- Using the main VAR approach to predict the interest rates in the furture, and combine with the AR model.

- Appling the Cross-validation time series data will increase the accurate prediction. 
