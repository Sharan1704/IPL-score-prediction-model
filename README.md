# IPL-score-prediction-model
This repository contains a cricket score prediction project using a neural network model. The project leverages a dataset of historical IPL match data to train the model and predict the final score of a cricket match based on various in-game features.

Here's a breakdown of the project:

Data Collection and Cleaning:

The project uses an IPL dataset (ipl_data.csv) containing information about matches, players, and performance statistics.
Data cleaning involves handling missing values and converting data types (e.g., date to datetime).
Feature Engineering:

The project extracts relevant features from the dataset to improve model accuracy. These include:
Date-related features (year, month, day, day of the week).
Rolling averages of runs and wickets.
Interaction features (e.g., batting team vs. bowling team).
Cumulative statistics (e.g., cumulative runs and wickets).
Player and venue statistics (e.g., average runs scored by a batsman at a specific venue).
Data Preprocessing:

Categorical features are encoded using one-hot encoding to convert them into numerical representations.
Numerical features are standardized using StandardScaler to ensure they have a similar range of values.
Model Building:

A neural network model is constructed using the Keras library.
The model consists of an input layer, multiple hidden layers with ReLU activation, and an output layer with a linear activation function for regression.
Model Training and Evaluation:

The model is trained using the preprocessed data.
Huber loss is used as the loss function during training.
The model's performance is evaluated using metrics such as Mean Absolute Error (MAE), Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and R-squared.
Prediction and Visualization:

The trained model can be used to predict scores for new matches based on input features.
The project includes visualizations to analyze model performance and prediction errors (residual plots, predicted vs. actual plots, box plots).
Interactive Prediction:

An interactive prediction interface is implemented using ipywidgets, allowing users to input match features and get predicted scores.
This project demonstrates the application of machine learning techniques to predict cricket scores. It covers various aspects of a data science project, including data preprocessing, feature engineering, model building, evaluation, and visualization.
