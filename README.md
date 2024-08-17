PROBLEM STATEMENT :

Task 1:- Prepare a complete data analysis report on the given data.

Task 2:- Fix a period for prediction of confirmed cases/deaths. Create a predictive model to forecast the Covid19 cases based on past cases for a specific country or region.

Task3:- Make suggestions to the government health department of the country/region for preparation based on your predictions

In this project we have the 3 datasets they are : 

3 Dataset for Analysis

1.time_series_covid19_confirmed_global Contains the count of confirmed patients on each day along with their country,states etc.

2.time_series_covid19_deaths_global Contains the count of death cases on each day along with their country,States etc.

3.time_series_covid19_recovered_global Contains the count of recovered patients on each day along with their country,states,etc. 
This is a daily updating version of COVID-19 Data Repository by the Center for Systems Science and Engineering (CSSE) at Johns Hopkins University (JHU). 
The data updates every day at 6am UTC, which updates just after the raw JHU data typically updates.

The JohnsHopkinsCovid19 project consist of 3 different dataset.They are * * * 'time_series_covid19_confirmed_global','time_series_covid19_deaths_global','time_series_covid19_recovered_global'.

Since the 3 datasets have 248 columns in which first 4 columns are Province/State,Country/Region,Lat,Long and rest are the dates so I converted the wide dataset into long by using the melt function.

After melting 3 datasets then i merge those datasets into one single dataset.

While doing the EDA it is seen that US,Brazil and India are those countries mostly affected by the Covid19 virus.

i have tried with 4 models for forcasting -ARIMA,SARIMAX,Exponential Smoothing and AR.

After evaluating multiple time series models, it was determined that the HOLT WINTER model demonstrated the best performance based on Mean Squared Error (MSE).
Thus I selected HOLT WINTER model for predicting confirm cases for the period of time "2020-09-21" to "2020-12-21".

SUGGESTION

Based on our analysis on US these are our suggestions,
Improve testing capabilities:-Make testing more accessible and capable in order to quickly detect and isolate affected people.

Improve Healthcare System :-Boost the healthcare system by making sure there are enough hospital beds, medical supplies, and equipment to handle any spikes in COVID-19 cases.

Affordable medical support :- As most of these medical facilities are expensive most of the people stay back from these which can be threaten for their life.

Proper Awareness programs on Rural Areas:- As the population in Rural areas are comparitively more proper awareness programs are necessary.

RISKS


Since there was 3 dataset it was difficult to merge them.

Finding the best time series model was also a challenging one.
