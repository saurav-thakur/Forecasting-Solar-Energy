# Forecasting solar energy based on historical weather data

Given the current high cost of energy, the company plans to introduce a new service that will enable nearby residents who live near a renewable energy source to receive free electricity when there is an excess of energy in the area. The company plans to start a pilot study in which a portion of the client base will test this technology in May 2024. The company must first create a system that can precisely predict, at least 24 hours in advance, whether there will be a surplus of energy (from solar or wind power) in order to alert nearby customers and provide them the chance to opt-in for the slot.



# Required Libraries

 - Numpy
 - Pandas
 - Matplotlib
 - Seaborn
 - fancyimpute
 - tensorflow

# How to run the project

Follow the steps provided in the notebook to run the project. The project needs to be run sequentially. (For Notebook -> 02_final_model_building.ipynb)

**Note: There's a section in the code to Impute Null Values. Here I have used fancyimpute KNN algorithm. This algorithm might take up large amount of time and also use large space from RAM. So, you can choose not to run the project as I have included the preprocessed data.**

## Contents of this Notebook

 1. Introduction
 2. Importing Libraries
 3. Loading the dataset
 4. Preprocessing Data
    - Feature Selection
    - Imputing Missing Values
    - Saving Preprocessed Files
    - Importing the Preprocessed Files

 5. Feature Engineering
    - Creating Lag Features
    - Imputing Nulls Created by lags

 6. Choosing Threshold for Solarenergy
    - Converting Solar Energy from MJ/m2 to KW

 7. Model Building
    - Data Standardization
    - Preparing Data For Training](#preparing-data-for-for-training)
    - Metrics
    - Naive Model
    - LSTM
    - Prediction on Test
    - Convering Prediction to Dataframe
    - False Positives for initial threshold
    - Threshold Updation
    - False Positives for safe buffer threshold
    - Forecasting 24 hours in Advance
    - Making DataFrame to Visualize 24 hour Advance Forecast
    - Plots
      - Plots for Naive Model
      - Plots for LSTM Model

   