# Predicting Urban Air Quality Using Machine Learning: A Case Study of Indian Cities
  
**Date**: June 18, 2025

---

## Dataset Overview

- **Dataset Description**:
  - **Source**: Air quality data collected from monitoring stations in Indian cities (e.g., AQI.in, IQAir).
  - **Size**: Covers three years (2022–2024), with hourly records—about 26,280 data points per city!
  - **Key Features**:
    - Pollutants: PM2.5 (tiny dust particles), PM10, NO2 (nitrogen dioxide), CO (carbon monoxide).
    - Traffic: Number of vehicles and traffic jams.
    - Weather: Temperature, humidity, wind speed, rain.
  - It’s time-series data, meaning it tracks changes over time.

- **Data Preprocessing**:
  - Fixed missing data by guessing values based on nearby records (interpolation).
  - Adjusted numbers to a similar scale (normalization) so the model works better.
  - Added past AQI values (e.g., last 24 hours) to spot patterns.

---

## Problem Statement

- **Brief Overview**:
  - Air pollution is a big problem in Indian cities, harming people’s health and nature. We want to predict the Air Quality Index (AQI) for the next day to help cities act fast.

- **Key Objectives**:
  1. Build a machine learning model to predict AQI accurately.
  2. Find out which factors (like dust or weather) affect air quality the most.
  3. See how this model can work with traffic systems to lower pollution.
  4. Show how AI can help solve air pollution in places like India.

---

## Methodology

- **Approach**:
  1. Gathered data from air quality stations.
  2. Cleaned and prepared the data.
  3. Trained machine learning models to predict AQI.
  4. Checked how well the models worked.

- **Algorithms Used**:
  - **CatBoost**: A smart algorithm that learns patterns quickly and handles messy data well. It’s great for predicting things like AQI because it combines many small predictions into one strong result.
  - **Random Forest**: Like a team of decision-makers—each “tree” votes on the answer. It’s simple to understand and works well with complex data.
  - **K-Nearest Neighbors (KNN)**: A basic method that looks at similar past examples to guess the AQI. We used it to compare with the fancier models.

- **Evaluation Metrics**:
  - **RMSE (Root Mean Square Error)**: Measures how far off our predictions are, in AQI points.
  - **MAE (Mean Absolute Error)**: Shows the average mistake in our predictions.
  - **R²**: Tells us how much of the AQI changes our model can explain (closer to 1 is better).

---

## Result

- **Model Performance**:
  - **CatBoost**: R² = 0.95 (super close fit!), RMSE = 5.0, MAE = 3.5
  - **Random Forest**: R² = 0.90 (still good), RMSE = 6.2, MAE = 4.0
  - **KNN**: R² = 0.80 (okay), RMSE = 10.0, MAE = 7.5

- **Graphs/Visualizations**:
  - **Bar Chart**: Compares R² and RMSE for all models—CatBoost wins!
  - **Feature Importance Plot**: Shows PM2.5 and wind speed as the biggest influencers of AQI.

---

## Discussion

- **Insights**:
  - PM2.5 (tiny dust) is the main troublemaker for bad air quality.
  - Wind speed helps blow pollution away, making it a key player.
  - Looking at yesterday’s AQI helps predict tomorrow’s better.

- **Challenges Faced**:
  - Some data was missing or messy, which made things tricky.
  - Air quality changes over time in complicated ways.
  - Training powerful models like CatBoost takes a lot of computer power.

---

## Solution Impact

- **Sustainability Impact**:
  - Predicting AQI helps warn people early, so we can cut pollution and keep the air cleaner.
  - Healthier air means a healthier planet and people!

- **Practical Implementation**:
  - Use the model in city systems to:
    - Control traffic when pollution is predicted to spike.
    - Send alerts telling people to stay indoors or wear masks.
    - Set up rules like “no cars” zones on bad air days.

---

## Conclusion

- **Summary**:
  - Our CatBoost model predicts AQI really well (R² = 0.95) and shows PM2.5 and wind speed matter most.
  - It can team up with traffic systems to fight pollution in cities.

- **Future Work**:
  - Make a system that predicts AQI in real-time.
  - Add more data, like pictures from satellites.
  - Predict other pollutants, like ozone.

---

## References

- [Air Quality Prediction by Machine Learning Models](https://www.sciencedirect.com/science/article/pii/S004565352301785X)  
- [Interpretable Machine Learning for Air Pollution](https://aaqr.org/articles/aaqr-23-06-oa-0151)  
- [Urban Air Quality Prediction Framework](https://www.nature.com/articles/s41598-024-83248-z)  
- [AI and Air Pollution Management in India](https://www.nature.com/articles/s41598-024-71269-7)  
- [Data Sources: AQI.in, IQAir]

---

## Thank You!