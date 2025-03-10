# Housing Price Prediction Model

This repository contains a machine learning model built to predict housing prices based on various property features such as size, rent, location, and amenities. The model is developed using Python, specifically using libraries such as `pandas`, `numpy`, `sklearn`, and `xgboost`.

## Project Overview

The goal of this project is to predict the price of a housing listing based on various features, such as the size of the property, monthly rent, amenities, and location. The project walks through data preprocessing, feature engineering, model building, and evaluation steps. 

### Key Steps:
1. Data Preprocessing
   - Handling missing data
   - Converting categorical and numerical variables
   - Feature engineering (e.g., extracting amenities and calculating price per square meter)
   - Outlier removal
   - Log transformation of the target variable
   
2. Model Building
   - Splitting data into training and testing sets
   - Building an XGBoost regression model

3. Model Evaluation
   - Evaluating the model using the Mean Absolute Error (MAE) metric

4. Saving the Model
   - Saving the trained model and preprocessing pipeline for future use

## Project Structure

HousingPricePrediction/ 
│ 
├── data/ 
│ └── otodom_data.csv # Dataset used for housing price prediction 
├── notebooks/ 
│ └── housing_price_prediction_notebook.ipynb # Jupyter notebook with data preprocessing, model building, and evaluation 
├── models/ 
│ ├── housing_price_predictor_model.pkl # Saved machine learning model 
│ └── preprocessor.pkl # Saved preprocessing pipeline 
├── README.md # Project documentation 
└── requirements.txt # Python dependencies


## Installation

### 1. Clone the repository

First, clone the repository to your local machine:

```bash
git clone
cd HousingPricePrediction
```

### 2. Set up the environment
Create a virtual environment and activate it:
```bash
python3 -m venv env
source env/bin/activate  
```
### 3. Install required dependencies
Install the necessary libraries with pip:
```bash
pip install -r requirements.txt
```
### 4. Download the dataset
Download the dataset (otodom_data.csv) from the relevant source and place it in the data/ directory, or adjust the path in the notebook accordingly.


### Usage
1. Run the Jupyter Notebook
You can run the Jupyter notebook that contains the entire process of building and evaluating the model.

Start Jupyter notebook by running the following command in the terminal:
```bash
jupyter notebook
```
Then, open the housing_price_prediction_notebook.ipynb notebook in the browser and follow the steps to see the model in action.

2. Predict Housing Prices
Once you have trained the model, you can use the saved model to make predictions. You can load the model and preprocessor using joblib and then predict prices for new data.