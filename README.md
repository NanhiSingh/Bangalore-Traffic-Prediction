

# Bangalore-Traffic-Prediction
Bangalore faces severe traffic congestion from rapid urban growth, causing delays and productivity loss. This project develops a prediction model using historical and contextual data to forecast congestion, provide real-time insights, guide commuters, aid authorities, and improve travel efficiency and sustainability.

## Acquire the data

Bangalore-Traffic-Dataset : https://www.kaggle.com/datasets/preethamgouda/banglore-city-traffic-dataset

## Libraries Used

- Pandas : Used for data manipulation and analysis, especially with structured data in DataFrames.
- numpy : Provides support for efficient numerical operations on large, multi-dimensional arrays and matrices.
- LabelEncoder : Encodes categorical labels into numerical format for machine learning models.
- Matplotlib : A plotting library for creating static, animated, and interactive visualizations in Python.
- Seaborn : An extension of Matplotlib for statistical data visualization with improved aesthetics.
- StandardScaler : Scales features to have a mean of 0 and a standard deviation of 1, aiding in model convergence.
- Sklearn : Provides algorithms for data mining and analysis
- Requests : A library for sending HTTP requests, used to interact with APIs and fetch data from web sources.
- Folium : Creates interactive maps by leveraging the Leaflet JavaScript library, ideal for geographic data visualization.
- Nominatim : A geocoding tool that converts addresses into geographic coordinates and vice versa.
- Polyline : Encodes and decodes geographic paths, often used in mapping and route visualization.

## Refine the data

The following operations have been performed on the dataset : 
- Checking missing values
- Removing the duplicates
- Deriving new feature
- Converting the categorical data

## Explore the data

We would like to visually explore the dataset to see if we can confirm some of the hypothesis and formulate new hypothesis based on the insights from different features.

1. Are weekends less congested compared to weekdays?
2. Which areas experience the highest traffic density?
3. How does traffic vary under different weather conditions?
4. How does traffic volume affect the congestion level?


## Model the solution

Before feeding teh data to any model for training, we will do the folling pre-processing: 

1. Feature and Target Selection
2. Feature Scaling
3. Train-Test Split

    ### Models used
    - Support Vector Regression (SVR)
    - Historical Average (HA) Model
    - Long Short-Term Memory (LSTM)

    ### Model Performance Evaluation
    Three regression metrics are used to evaluate the model's performance : 
    - Mean Absolute Error (MAE): Measures the average absolute differences between predicted and actual values.
    - Mean Squared Error (MSE): Captures the average of squared differences, penalizing larger errors more significantly.
    - R-squared (R²): Indicates how well the model explains the variability in the target variable (closer to 1 indicates a better fit).

## Aesthetics

For look and feel the user is provided with the inputs to select the start and the end points and show the congestion level on map.

![WhatsApp Image 2025-08-14 at 17 01 03](https://github.com/user-attachments/assets/b586870e-580c-4dfc-adb1-ec2d6478ca95)

![WhatsApp Image 2025-08-14 at 17 01 03 (1)](https://github.com/user-attachments/assets/bb46e5f6-d89f-422f-a4c5-62658f22a20a)
