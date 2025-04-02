# Taxi Trip Price Prediction

## Project Overview

This project aims to predict taxi trip prices using machine learning techniques. It utilizes a dataset of taxi trips with various features such as time of day, day of week, traffic conditions, weather, and distance traveled. By leveraging these features, the project develops a model capable of estimating trip prices with reasonable accuracy.

## Technology Used

- **Programming Language:** Python
- **Libraries:** Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn
- **Algorithm:** K-Nearest Neighbors Regression
- **Platform:** Google Colab

## Data

The project uses a dataset called 'taxi_trip_pricing.csv' which contains information about taxi trips, including features like:

- Time of Day
- Day of Week
- Traffic Conditions
- Weather
- Distance Traveled
- Trip Price (Target variable)

## Logic

1. **Data Loading and Preprocessing:**
   - Load the dataset using Pandas.
   - Handle missing values by dropping rows with missing data.
   - Convert categorical features (Time_of_Day, Day_of_Week, Traffic_Conditions, Weather) into numerical representations using one-hot encoding.
   - Split the data into training and testing sets.
   - Scale numerical features using StandardScaler to ensure features have similar ranges.

2. **Model Building:**
   - Utilize the K-Nearest Neighbors Regression algorithm to build the predictive model.
   - Train the model using the training data.

3. **Model Evaluation:**
   - Evaluate the model's performance using metrics such as Mean Squared Error (MSE) and R-squared.
   - Compare predicted trip prices with actual trip prices to assess accuracy.

4. **Hyperparameter Tuning:**
   - Use GridSearchCV to find the optimal value for the 'n_neighbors' hyperparameter, which determines the number of neighbors considered for prediction.

5. **Visualization:**
   - Create visualizations to understand the relationship between predicted and actual values:
     - Scatter plot of actual vs. predicted values.
     - Residual plot to check for patterns in errors.
     - Histogram of residuals to analyze their distribution.
    
    ![image](https://github.com/user-attachments/assets/1e35f905-1f49-4430-944b-189cd9142995)

   ![image](https://github.com/user-attachments/assets/51906713-a267-4019-b5a4-8cb633bee6c1)

   ![image](https://github.com/user-attachments/assets/5f3c841d-7cf5-47b3-8996-b8fb909cca4d)




## Code Explanation

The code is organized into sections with comments to explain each step. Here's a summary:

- **Data Loading and Preprocessing:** Reads the CSV file, handles missing values, performs one-hot encoding, and scales the features.
- **Model Building:** Creates and trains a K-Nearest Neighbors Regression model.
- **Model Evaluation:** Calculates and prints evaluation metrics (MSE, R-squared).
- **Hyperparameter Tuning:** Uses GridSearchCV to find the best hyperparameters for the model.
- **Visualization:** Generates scatter plots, residual plots, and histograms to visualize the results.

## Conclusion

This project demonstrates the application of machine learning for taxi trip price prediction. By utilizing relevant features and a suitable algorithm, the model achieves reasonable accuracy in estimating trip prices. The visualizations provide insights into the model's performance and potential areas for improvement.

## Future Work

- Explore other regression algorithms to potentially improve accuracy.
- Incorporate additional features, such as location data, to enhance the model's predictive power.
- Deploy the model as a web application or API for real-time price prediction.
