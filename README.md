# MIT_Crit_Data-GBCF (also known as MIT-LCP): A Non-Mechanistic Approach Using Machine Learning and Novel Digital Data


This model uses a gradient boosted regressor with hyperparameter optimization that uses prior COVID cases and deaths as well as demographic, socioeconomic, mobility, and healthcare related county-level covariates. This model forecasts COVID deaths at the county level and aggregates to the state and national level. This model does not directly account for state reopenings and closures but indirectly via changes in the mobility measures. Evaluation of model predictions is done using 
[COVID-19 Forecast Hub Evaluation](https://github.com/youyanggu/covid19-forecast-hub-evaluation)  modules.
