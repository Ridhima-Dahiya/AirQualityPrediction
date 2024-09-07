# AirQualityPrediction
This was my Master's dissertation work, where the study of air quality in Rohtak city of Haryana using various machine learning (ML) approaches was performed.


**Introduction**
Due to the impacts of air_quality on human’s everyday life, precise prediction of air_quality has become an urgent and essential problem. The study demonstrates the various ML models that are capable of performing better predictions, the parameters which are helpful in making better predictions and the various ways to handle the noise in the air_quality data. 

**DATASET ACQUISITION**
Here, the data used for this work included the pollutant as well as meteorological parameters that were collected for the city of Rohtak, town in Haryana state of India. The time period of the collected data was from“01-01-2014” to “30-04-2020”. The overall data containing all the “criteria” pollutants and the meteorological data consisted of 32,368 samples containing missing values for the pollutant concentrations

**POLLUTANT PARAMETERS**
The dataset for “pollutant” parameters recorded for Rohtak were collected from the air quality monitoring station in Rohtak “H.S.P.C.B” which gave us the recorded concentrations for the parameters PM2.5, CO, NO, NO2, NOX, O3 and, SO2 respectively. The dataset was available since January 1, 2014 to April 30, 2020.Being precise, the dataset was missing for every parameter between dates “1-06-2014 to 31-08-2014”, ”29-03-2018 to 12-04-2018” and “01-11-2018 to 30-11-2018” and also on dates “09-10-2017”, “10-10-2017”, “23-07-2018” and “31-10-2018”. And the recorded concentrations for specific pollutant parameters were also found missing on several dates.

![image](https://github.com/user-attachments/assets/8aed9b29-3bcf-49c0-baab-cb56d9471544)


**METEOROLOGICAL PARAMETERS**
Requisite meteorological parameters include the information related to the wind 
speed, wind direction, temperature, moisture levels etc. The meteorological data was collected through the SoDa “Solar Radiation and Meteorological Data Services” website as it provides access to the meteorological data from MERRA 2 “Modern-Era Retrospective analysis for Research and Applications” web-service delivering time series of meteorological parameters worldwide. The meteorological data for Rohtak since January 2014 to April, 2020 was downloaded in CSV “Comma Separated Values” by filling the details of latitude and longitude of Rohtak which are “28.8699°” and “76.46937°” respectively.

![image](https://github.com/user-attachments/assets/9c1169f2-41e0-4f11-b0ce-b82c48402868)
![image](https://github.com/user-attachments/assets/02cd3c58-5324-4ee7-b3dc-a628287ad94a)

# Parameters considered collectively: ![image](https://github.com/user-attachments/assets/baa3fa2a-19f4-454e-922f-19e7561c54d3)

**DATASETS CONSIDERED FOR BUILDING MODELS**
I have divided the overall data into mini datasets where done the predictions for  individual  air pollutant parameter i.e. “output variable” is done  on the  basis of  previous  air pollutant concentration of the pollutant parameter and the meteorological parameters i.e. “input variables”. Hence, I have a total of 6 datasets for which the models are built.  Sample dataset file for “AQI” pollutant parameter named as “PREVaqi” is shown in figure along with the screenshot containing list of other dataset csv files for which the models are built using code.
![image](https://github.com/user-attachments/assets/5fa4876a-3ceb-4342-84b1-ef6a97d0eaef)

**EXPERIMENTAL RESULTS**
I have built a  total of 11 ML models comprising of Linear Regression, BayesianRidge Regression, ARD Regression, DecisionTree Regression, Bagging Regressor, ExtraTrees Regressor, AdaBoost Regressor, Gradient Boosting Regressor, Multi-Layer Perceptron Regressor, Random Forest Regressor and Support Vector Regressor. Each of these models are used to predict air_pollutant parameter present in the 6 datasets used in the study.  

