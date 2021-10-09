# MIT_Crit_Data-GBCF (also known as MIT-LCP)
## A Non-Mechanistic Approach to Real-Time Forecasting of US COVID-19 Mortality Using Machine Learning and Novel Digital Data

### About the model
This model uses a gradient boosted regressor with hyperparameter optimization that uses prior COVID cases and deaths as well as demographic, socioeconomic, mobility, and healthcare related county-level covariates. This model forecasts COVID deaths at the county level and aggregates to the state and national level. This model does not directly account for state reopenings and closures but indirectly via changes in the mobility measures. Evaluation of model predictions is done using 
[COVID-19 Forecast Hub Evaluation](https://github.com/youyanggu/covid19-forecast-hub-evaluation)  modules.

### Data Sources
| Source      | Description | Scope |
| ----------- | ----------- | ----- |
|[JHU CSSE](https://github.com/CSSEGISandData/COVID-19)|Daily US COVID-19 Deaths and Cases|County Level|
|[County-level Socioeconomic Dataset](https://github.com/JieYingWu/COVID-19_US_County-level_Summaries)|300 variables that summarize population estimates, demographics, ethnicity, housing, education, employment and income, climate, transit scores, and healthcare system-related metrics|County Level|
|[PlaceIQ](https://github.com/COVIDExposureIndices/COVIDExposureIndices)|Exposure indices derived from PlaceIQ movement data|County Level|
|[US Dept of HHS](https://protect-public.hhs.gov/pages/hospital-utilization)|COVID-19 Hospital capacity and utilization from HHS|State Level|

### Pipeline
![](https://cdn.discordapp.com/attachments/889317786059427894/896502334480326707/pipeline.JPG)
