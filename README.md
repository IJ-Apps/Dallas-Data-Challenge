# Dallas Data Challenge
This repository contains two Machine Learning models that forecast the daily # of available and occupied hospital beds in the Dallas-Fort Worth region based on previous data.

**That is, when given future dates as input, the model will forecast the # of available hospital beds on each of those future dates and in addition, provide a range of possible values.**


## About the Code
The code is easily modifiable and [**very detailed**](https://github.com/IJ-Apps/Dallas-Data-Challenge/blob/master/DFW%20Available%20Hospital%20Bed%20Forecasting.ipynb) so that predictions can be made for different cities/regions given their data.

- [**DFW Available Hospital Bed Forecasting.ipynb**](https://github.com/IJ-Apps/Dallas-Data-Challenge/blob/master/DFW%20Available%20Hospital%20Bed%20Forecasting.ipynb) is a very detailed Jupyter Notebook for creating a model that forecasts the # of available hospital beds on future dates
- [**DFW Occupied Hospital Bed Forecasting.ipynb.ipynb**](https://github.com/IJ-Apps/Dallas-Data-Challenge/blob/master/DFW%20Occupied%20Hospital%20Bed%20Forecasting.ipynb) is a Jupyter Notebook for creating a model that forecasts the # of occupied hospital beds.

### Features of the Notebooks
- **Evaluating Model Performance on Known Data:** 
  - In each Jupyter Notebook I train the model on data only before September - *(data is available for September dates)*. 
  - After the model is trained, I make it "forecast" the \# of available/occupied hospital beds in the first 3 weeks of September.
  - I compare these forecasts with the actual \# of hospital beds and calculate the **percent error, mean absolute error, and \# of forecast *intervals* that captured the correct \# of beds)**
- **Forecasting for Future Dates:** 
  - In this part of the notebook, I train the model on all past hospital bed data *(including September)*, then generate a list of 31 days from September 23rd to October 23rd and feed it into the model.
  - **The model forecasts the # of available/occupied hospital beds in the DFW region for future dates *(late September - October)*.**

### Features of the Model
- Providing a **forecast** of the \# of hospital beds available/occupied for a specified date in the future.
- Providing an **interval** of possible \# of hospital beds for a specified date in the future.
-----

## About the Data
The data comes from the Texas DSHS website: https://dshs.texas.gov/coronavirus/additionaldata.aspx

The CSVs in this repository are:
- [**available_beds.csv:**](https://github.com/IJ-Apps/Dallas-Data-Challenge/blob/master/available_beds.csv) \# of available hospital beds in regions in Texas.
- [**occupied_beds.csv:**](https://github.com/IJ-Apps/Dallas-Data-Challenge/blob/master/occupied_beds.csv) \# of occupied hospital beds in regions in Texas


