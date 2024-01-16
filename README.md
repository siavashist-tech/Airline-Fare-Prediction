# Airline-Fare-Prediction
Data Science Project

# Project Statistics

## Dataset Overview:
- **Total Instances:** 10,000
- **Features:** 15
- **Target Variable:** Flight Fare

## Data Processing:
- **Missing Values:** Handled appropriately through imputation and dropping.
- **Feature Extraction:** Extracted day, month, and year from date-time columns.
- **Categorical Encoding:** Applied one-hot encoding for categorical variables.
- **Feature Scaling:** Ensured all features were on a comparable scale.

## Model Building:
- **Algorithm:** Random Forest Regressor
- **Hyperparameter Tuning:** Utilized GridSearchCV for optimal parameters.
- **Evaluation Metrics:**
  - Mean Absolute Error (MAE)
  - Mean Squared Error (MSE)
  - Root Mean Squared Error (RMSE)
  - R^2 Score
    
## Model Performance:
- **Original Model Score:** 66%
- **Tuned Model Score:** Aiming for above 70%
- **Best Hyperparameters:**
  - Number of Estimators: 200
  - Maximum Depth: 20
  - Minimum Samples Split: 2
  - Minimum Samples Leaf: 1

## Visualization:
- **Histogram of Residuals:** Visualized distribution of prediction errors.
- **Scatter Plot:** Compared actual vs. predicted flight fares.
  
## Model Persistence:
- **Model Save Format:** Pickle (.pkl)
- **Saved Model Size:** 2.5 MB

## Conclusion:
The project successfully tackled the challenge of predicting flight fares with a machine learning model. Further optimization is underway to achieve a target model score above 80%. The visualization tools provided valuable insights into prediction errors, guiding further model refinement. The saved model allows for easy integration into applications or services requiring flight fare predictions.

---

# Flight Fare Prediction
Flight ticket prices are often considered unpredictable, with fluctuations that can make planning travel challenging. In this project, we aim to challenge that notion by leveraging data science techniques to predict airline flight fares for various routes across Indian cities. The dataset used for this project was provided by the company, and it includes detailed information about flight prices for different airlines.

## Dataset Overview
The dataset for the Airline Flight Fare Prediction project is time-stamped, requiring extensive pre-processing to prepare it for model training. The primary goal is to develop a machine learning model capable of accurately predicting flight fares between different cities in India. Several features in the dataset underwent pre-processing and transformation, especially those related to date-time information.

## Project Highlights
- **Time-Stamped Dataset:** The dataset is time-stamped, providing a chronological aspect to the flight fare data. Handling date-time columns required careful pre-processing to extract meaningful features.

- **Feature Engineering:** To enhance the predictive power of the model, new parameters were derived from existing features. Feature engineering played a crucial role in creating a cleaner and more effective input for the machine learning algorithm.

- **Machine Learning Model:** A machine learning model was developed to predict airline fares based on the processed dataset. The choice of the model, along with hyperparameter tuning, was critical in achieving accurate predictions.

## Steps in Data Processing
1. **Data Cleaning:** Handling missing values and ensuring data integrity was the first step. Null values were addressed appropriately, and data entries were validated.

2. **Feature Extraction:** Date-time columns were decomposed to extract day, month, and year information separately. This facilitated better understanding and utilization of temporal aspects in the model.

3. **Categorical Encoding:** Categorical variables like airlines, source, and destination were encoded to enable their incorporation into the machine learning model.

4. **Feature Scaling:** Depending on the chosen machine learning algorithm, features might require scaling for optimal performance. This step ensured all features were on a comparable scale.

## Model Building and Evaluation
- **Random Forest Regressor:** A Random Forest Regressor was chosen as the primary model for predicting flight fares. The model underwent hyperparameter tuning to enhance its predictive capabilities.

- **GridSearchCV:** A grid search was performed to find the optimal hyperparameters for the Random Forest Regressor, improving the overall performance of the model.

- **Model Evaluation:** Evaluation metrics such as Mean Absolute Error (MAE), Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and R^2 score were used to assess the model's accuracy and effectiveness.

## Visualization of Predictions
- **Histogram of Residuals:** A histogram was plotted to visualize the distribution of residuals, providing insights into the model's prediction errors.

- **Scatter Plot for Actual vs. Predicted Values:** A scatter plot allowed a direct comparison between the actual flight fares and the predicted fares, showcasing the model's predictive accuracy.

## Model Persistence
- Pickle: The final tuned model was saved using the Pickle library, allowing for easy storage and reuse.
  
## Conclusion
This Flight Fare Prediction project demonstrates the power of data science in tackling the seemingly unpredictable nature of airline ticket prices. The implemented machine learning model, backed by thorough data processing and feature engineering, offers a reliable tool for predicting flight fares between various Indian cities. The project contributes to the broader field of travel analytics and has the potential to enhance the user experience in planning air travel.
