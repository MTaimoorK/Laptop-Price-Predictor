# Laptop Price Predictor
## Author: Muhammad Taimoor khan

## Table of Contents
- [Problem Statement](#problem-statement)
- [Solution](#solution)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Dependencies](#dependencies)
- [Usage](#usage)
- [Streamlit App](#streamlit-app)
- [Model Training](#model-training)
- [Exported Files](#exported-files)
- [Contributing](#contributing)
- [License](#license)

## Problem Statement

The problem at hand is to build a laptop price predictor based on various features such as brand, type, specifications, and hardware components. In the current era, where technology is advancing rapidly, users are often overwhelmed by the multitude of laptop options available in the market. This predictor aims to assist potential laptop buyers in estimating the price of a laptop based on their preferred specifications and features.

## Solution

### 1. Importing Dependencies

The initial step involves importing necessary libraries such as NumPy, Pandas, and Matplotlib for data manipulation and visualization.

### 2. Data Preprocessing

- The dataset is loaded and initial exploration is performed.
- Unnamed columns are dropped, and missing values are checked. No missing values are found.
- The 'Ram' and 'Weight' columns are cleaned and converted to the appropriate data types.
- Laptop prices are converted to USD for better generalization.

### 3. Data Analysis

- Exploratory Data Analysis (EDA) is conducted using Seaborn and Matplotlib to gain insights into the dataset.
- Visualizations include distribution of laptop prices, top-selling brands, price distribution based on brand, laptop type analysis, and the impact of screen size and resolution on prices.
- Feature engineering is performed to identify touchscreen and IPS display laptops.
- Correlation analysis is conducted to understand the relationship between numerical features and laptop prices.

### 4. Model Training

- The dataset is split into training and testing sets.
- Various regression models are trained, including Linear Regression, Ridge Regression, Lasso Regression, K-Nearest Neighbors, Decision Tree, Support Vector Machines, Random Forest, Extra Trees, AdaBoost, Gradient Boost, XG Boost, and a Voting Regressor.
- The models are evaluated using R2 score and Mean Absolute Error.

### 5. Exporting The Model

- The trained model and the preprocessed dataset are exported using Pickle for future use.

### 6. Streamlit App

- The trained model and dataset are loaded in a Streamlit web application.
- Users can input their preferences for brand, type, RAM, weight, touchscreen, IPS, screen size, resolution, CPU, HDD, SSD, GPU, and OS.
- Upon clicking the "Predict Price" button, the app uses the trained model to estimate and display the predicted laptop price.

This solution provides a user-friendly interface for potential laptop buyers to estimate the price of a laptop based on their desired specifications, helping them make informed purchasing decisions. The predictive model takes into account various features and specifications to generate accurate price estimates.

## Project Structure

- `data/`: Folder containing the dataset (`laptop_data.csv`).
- `models/`: Folder to store the exported model and preprocessed data.
- `notebooks/`: Jupyter notebooks for data exploration and model development.
- `app/`: Streamlit web application code (`app.py`).
- `README.md`: Project documentation.

## Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/MTaimoorK/laptop-price-predictor.git
   cd laptop-price-predictor
