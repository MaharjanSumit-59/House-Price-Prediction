# House Price Prediction (Machine Learning Project)

## Project Overview

This project builds a **Machine Learning model to predict house prices** based on different house features such as bedrooms, bathrooms, living area, and condition.
The goal is to understand the **complete machine learning workflow**, including data preprocessing, visualization, model training, and evaluation.

## Dataset

The dataset contains **4600 house records** with **18 features** describing property characteristics.

### Key Columns

* **price** – Target variable (house price)
* **bedrooms** – Number of bedrooms
* **bathrooms** – Number of bathrooms
* **sqft_living** – Living area size
* **sqft_lot** – Total lot size
* **floors** – Number of floors
* **waterfront** – Whether the house has a waterfront view
* **view** – Quality of the view
* **condition** – Overall condition of the house
* **sqft_above** – Above ground living area
* **sqft_basement** – Basement area
* **yr_built** – Year the house was built
* **yr_renovated** – Year of renovation

Some columns such as **date, street, city, statezip, and country** were removed because they are not necessary for a basic prediction model.

## Project Workflow

### 1. Data Loading

The dataset is loaded using **Pandas** and inspected using `.info()`, `.describe()`, and `.head()`.

### 2. Data Cleaning

* Checked for missing values
* Removed unnecessary categorical columns

### 3. Data Visualization

Basic visualizations were created to understand relationships in the data:

* Histogram of house prices
* Scatter plot of **sqft_living vs price**
* Boxplot of **bedrooms vs price**
* Correlation heatmap for numeric features

### 4. Feature Selection

The following features were used for training the model:

* bedrooms
* bathrooms
* sqft_living
* sqft_lot
* floors
* waterfront
* view
* condition
* sqft_above
* sqft_basement
* yr_built
* yr_renovated

Target variable:

* **price**

### 5. Train-Test Split

The dataset was split into:

* **80% training data**
* **20% testing data**

### 6. Model Training

A **Linear Regression model** from Scikit-Learn was used to train the prediction model.

### 7. Model Evaluation

The model was evaluated using the following metrics:

* **MAE (Mean Absolute Error)**
* **MSE (Mean Squared Error)**
* **R² Score**

Example results:

* MAE: ~210,908
* MSE: ~9.86e11
* R² Score: ~0.03

The low R² score indicates that the linear regression model does not capture the complex relationships in the dataset very well.


## Conclusion

This project demonstrates the basic steps involved in building a **machine learning regression model** for predicting house prices.
Although the Linear Regression model performed poorly, the project provides a foundation for experimenting with more advanced algorithms such as **Decision Trees and Random Forests**.

