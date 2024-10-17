# Titanic Survival Prediction

This repository contains a Python script for predicting the survival of passengers on the Titanic, using machine learning models like Logistic Regression and Random Forest.

## Dataset

The dataset used in this project is the Titanic dataset, which is publicly available on Kaggle and other sources. It contains information about passengers on the Titanic, such as their age, sex, class, and fare. The goal is to predict whether a passenger survived the disaster based on these features.


## Code Overview

The code performs the following steps:

1. **Load and Explore Data:** Loads the Titanic dataset from a URL and displays basic information like the first few rows, data types, and missing values.
2. **Data Cleaning and Preprocessing:**
   - Fills missing values in the 'Age' column with the mean age.
   - Removes the 'Cabin' column due to a large number of missing values.
   - Fills missing values in the 'Embarked' column with the most frequent value.
   - Converts 'Sex' to numerical values (0 for male, 1 for female).
   - Applies one-hot encoding to the 'Embarked' column to convert categorical values to numerical features.
3. **Feature Selection and Model Preparation:**
   - Selects relevant features (columns) for the prediction model.
   - Splits the data into training and testing sets.
4. **Model Training and Evaluation:**
   - Trains a Logistic Regression model and a Random Forest model.
   - Evaluates both models using accuracy and confusion matrices.
   - Performs K-Fold Cross-Validation for each model to assess their robustness.
5. **Results and Discussion:**
   - Presents accuracy scores for both models, with and without Cross-Validation.
   - Discusses the relative performance of the two models.

## Results

- **Logistic Regression Accuracy:** Approximately 0.80
- **Logistic Regression (Cross-Validation) Accuracy:** Approximately 0.80
- **Random Forest Accuracy:** Approximately 0.82
- **Random Forest (Cross-Validation) Accuracy:** Approximately 0.82

## Conclusion

The Random Forest model demonstrates slightly better performance than Logistic Regression, achieving a higher accuracy both in regular testing and Cross-Validation.


## How to Run

1. Make sure you have Python and the necessary libraries installed (Pandas, Matplotlib, Seaborn, Scikit-learn).
2. Download the code from this repository.
3. Run the Python script using a suitable environment.
4. The results will be printed to the console, including the model's accuracy and confusion matrices.

## Future Work

- Experiment with different machine learning models and feature engineering techniques.
- Optimize the hyperparameters of the models.
- Develop a more sophisticated user interface for model prediction. 

Feel free to explore the code and adapt it to your needs!
