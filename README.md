# House Sales in USA

This repository contains a comprehensive analysis of house sales data in the USA using Python. The analysis is performed through several steps, including data wrangling, exploratory data analysis, and model development using linear and ridge regression. The dataset used is `kc_house_data.csv`.

## Table of Contents

- [Installation](#installation)
- [Data Overview](#data-overview)
- [Modules](#modules)
  - [Module 1: Data Exploration](#module-1-data-exploration)
  - [Module 2: Data Wrangling](#module-2-data-wrangling)
  - [Module 3: Exploratory Data Analysis](#module-3-exploratory-data-analysis)
  - [Module 4: Model Development](#module-4-model-development)
  - [Module 5: Model Evaluation and Refinement](#module-5-model-evaluation-and-refinement)
- [Analysis](#analysis)
- [Conclusion](#conclusion)

## Installation

To run the code, you will need to install the required Python packages. Use the following command to install scikit-learn:

    pip install scikit-learn --upgrade --user
## Data Overview
The dataset `kc_house_data.csv` contains information about house sales in the USA. Key columns include:

- `price`: The sale price of the house.
- `bedrooms`: Number of bedrooms.
- `bathrooms`: Number of bathrooms.
- `sqft_living`: Square footage of the house.
- `sqft_lot`: Square footage of the lot.
- `floors`: Number of floors in the house.
- `waterfront`: Whether the house has a waterfront view.

## Modules

### Module 1: Data Exploration
In this module, we load and explore the dataset:

- Displayed the data types of each column.
- Generated descriptive statistics for all columns.

### Module 2: Data Wrangling
In this module, we performed data cleaning and wrangling:

- Dropped the `id` column (not successful due to an error).
- Checked and replaced missing values in the `bedrooms` and `bathrooms` columns with their respective means.

### Module 3: Exploratory Data Analysis
In this module, we performed exploratory data analysis (EDA) to uncover patterns:

- Counted the number of houses with unique floor values.
- Used a boxplot to analyze price outliers for houses with and without waterfront views.
- Used a scatter plot and regression line to analyze the correlation between `sqft_above` and `price`.
- Calculated correlation between all features and `price`.

### Module 4: Model Development
In this module, we developed predictive models:

- Performed linear regression using `longitude` as the predictor and `price` as the response variable.
- Used multiple linear regression with several features to predict `price`.
- Applied a pipeline with standard scaling, polynomial features, and linear regression.

### Module 5: Model Evaluation and Refinement
In this module, we evaluated and refined our models:

- Split the data into training and testing sets.
- Performed Ridge regression with regularization.
- Applied a second-order polynomial transformation and evaluated the model.

## Analysis

### Data Types
The dataset contains both numerical and categorical data. Initial exploration revealed that columns like `price`, `bedrooms`, and `bathrooms` are key variables of interest.

### Handling Missing Data
The dataset contained missing values in the `bedrooms` and `bathrooms` columns, which were replaced with the mean values to maintain data integrity.

### Exploratory Data Analysis
- **Floors**: Most houses in the dataset have 1 or 2 floors.
- **Waterfront**: Houses with waterfront views tend to have higher prices and more outliers.
- **Correlation**: Features like `sqft_living`, `grade`, and `sqft_above` showed a strong positive correlation with `price`.

### Model Development
- The simple linear regression using `longitude` as a predictor had a very low R² score, indicating that `longitude` alone is not a good predictor of `price`.
- Multiple linear regression with additional features provided a better fit, with significant coefficients for most variables.
- Polynomial regression and Ridge regression were used to capture more complex relationships and improve model performance.

### Model Evaluation
The Ridge regression model, particularly after applying a polynomial transformation, provided a better fit, as indicated by an improved R² score on the test data.

## Conclusion
The analysis demonstrates that multiple factors influence house prices, with `sqft_living`, `grade`, and `waterfront` being some of the most significant predictors. The models developed can be refined further by exploring more advanced machine learning techniques.

