# House-Sales-Analysis
## Introduction
This repository contains a Python script for analyzing house sales data in the USA. The script utilizes various machine learning techniques for data preprocessing, exploratory data analysis (EDA), model development, evaluation, and refinement. It employs popular libraries such as Pandas, Matplotlib, NumPy, Seaborn, and scikit-learn.

## Dependencies
* Python 3.x
* Pandas
* Matplotlib
* NumPy
* Seaborn
* scikit-learn

## Installation
* Clone this repository to your local machine or download the script directly.
* Ensure you have the required dependencies installed. You can install them using pip:
     pip install pandas matplotlib numpy seaborn scikit-learn

## Usage
* Open the script in your preferred Python environment.
* Run the script:
  python house_sales_analysis.py
* Follow the prompts and instructions provided in the script.

## Contents
### Module 01: Data Overview
* Displays data types of each column.
* Provides descriptive statistics of the dataset.

### Module 02: Data Wrangling
* Removes unnecessary columns.
* Handles missing values in the 'bedrooms' and 'bathrooms' columns.

### Module 03: Exploratory Data Analysis (EDA)
* Counts houses with unique floor values.
* Determines the impact of waterfront view on prices using boxplots.
* Investigates correlation between features and price using regression plots and correlation coefficients.

### Module 04: Model Development
* Develops a linear regression model to predict house prices.
* Implements polynomial regression for improved model performance.

### Module 05: Model Evaluation and Refinement
* Splits the data into training and testing sets.
* Utilizes Ridge regression for regularization.
* Performs polynomial transformation for higher-order polynomial regression.
* Evaluates model performance using R^2 score.

## Contributions
Contributions are welcome! If you have any suggestions, improvements, or feature requests, feel free to open an issue or submit a pull request.
