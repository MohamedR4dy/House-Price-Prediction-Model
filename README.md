# House Price Prediction Project

Welcome to the House Price Prediction project! In this project, we'll be working with a dataset containing house sale prices for King County, including Seattle. Our goal is to develop a machine learning model that can accurately predict house prices based on various features. This README will guide you through the project's structure, data analysis, model creation, evaluation, and more.
This project focuses on predicting house sale prices in King County, which includes Seattle, based on various features. The dataset used for this analysis contains information on homes sold between May 2014 and May 2015. The dataset has 21 columns (features) and 21613 rows.
## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Data Analysis and Preprocessing](#data-analysis-and-preprocessing)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Model Creation](#model-creation)
- [Model Evaluation](#model-evaluation)
- [Predicting House Prices](#predicting-house-prices)
- [Conclusion](#conclusion)

## Introduction

This project focuses on predicting house sale prices in King County, Seattle. By analyzing various features of houses, such as the number of bedrooms, bathrooms, square footage, condition, and more, we aim to build a machine learning model that can accurately predict the price of a house. This prediction has practical applications for both homebuyers and sellers, as well as real estate professionals.

## Dataset

The dataset contains information about house sales between May 2014 and May 2015 in King County. It includes 21 columns (features) and 21,613 rows. Here are some key columns in the dataset:

1. **id**: Unique ID for each home sold
2. **date**: Date of the home sale
3. **price**: Price of each home sold
4. **bedrooms**: Number of bedrooms
5. **bathrooms**: Number of bathrooms (with .5 accounting for a room with a toilet but no shower)
6. **sqft_living**: Square footage of the apartment's interior living space
7. **sqft_lot**: Square footage of the land space
8. **floors**: Number of floors
9. **waterfront**: A dummy variable indicating whether the apartment overlooks the waterfront (0 or 1)
10. **view**: An index from 0 to 4 indicating how good the view of the property was
11. **condition**: An index from 1 to 5 indicating the condition of the apartment
12. **grade**: An index from 1 to 13 indicating the quality level of construction and design
13. **sqft_above**: Square footage of the interior housing space that is above ground level
14. **sqft_basement**: Square footage of the interior housing space that is below ground level
15. **yr_built**: The year the house was initially built
16. **yr_renovated**: The year of the house's last renovation
17. **zipcode**: The zipcode area the house is in
18. **lat**: Latitude
19. **long**: Longitude
20. **sqft_living15**: Square footage of interior housing living space for the nearest 15 neighbors
21. **sqft_lot15**: Square footage of the land lots of the nearest 15 neighbors


## Data Analysis and Preprocessing

Before building our predictive model, we perform data analysis and preprocessing to understand the dataset and prepare it for training. This includes:

- Checking the dataset dimensions
- Exploring feature columns and their types
- Handling missing values, if any
- Feature engineering, e.g., creating year and month columns from the date
- Scaling and splitting the data into training and testing sets

## Exploratory Data Analysis

Exploratory Data Analysis (EDA) helps us understand the relationships between different features and the target variable. We use visualization libraries such as Seaborn and Plotly to create visualizations, including:

- Distribution plots of numerical features
- Box plots to analyze features like bedrooms, floors, and waterfront
- Heatmaps to visualize correlations between features
- Interactive maps to visualize housing conditions and prices geographically
- Price trends over different years and months

## Model Creation

We build a neural network regression model using TensorFlow and Keras to predict house prices based on the provided features. The model architecture includes input, hidden, and output layers. We use an Adam optimizer and mean squared error loss function for training.

## Model Evaluation

We evaluate the trained model using various metrics, including:

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- Variance Regression Score

These metrics help us understand how well the model's predictions align with the actual test set values.

## Predicting House Prices

We use the trained model to predict the price of a new house based on its features. This demonstrates the model's ability to generalize to new, unseen data.

## Conclusion

In this project, we explored house price prediction using a neural network regression model. While the model exhibited a certain level of accuracy, predicting house prices is a complex task due to the multitude of factors involved. This project provides valuable insights into the potential of machine learning for real estate predictions, acknowledging the ongoing need for refining models and exploring additional features.
