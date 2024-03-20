# BTC Machine Learning Model

## Overview
This project implements an LSTM (Long Short-Term Memory) model to predict buy and sell signals for BTC (Bitcoin) based on minute-level data. The model is trained using historical data sourced from a CSV file, which is preprocessed, cleaned, and augmented with additional data obtained through API calls. The project also includes exploratory data analysis (EDA) to understand the underlying patterns in the data and feature engineering, including the incorporation of technical analysis (TA) indicators.

## Requirements
- Python 3.12.2
- Libraries listed in `requirements.txt`

## Installation
1. Clone this repository:
    ```bash
   git clone https://github.com/hugobombaca/btc-trading-bot.git

2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt

## Usage
1. Preprocess the data:
   - Ensure your BTC minute-level data is stored in a CSV file.
   - Run the data preprocessing script to clean the data and augment it with additional features:
     ```bash
     python Cleaning Data.ipynb --input_file data/btc_minute_data.csv --output_file data/Clean Data.pkl
     
2. Explore the data:
   - Use Jupyter Notebook or any preferred tool to explore the cleaned_btc_data.csv file and understand the data distribution, correlations, and trends.
   - Visualize the data using matplotlib, seaborn, or other plotting libraries.

3. Train the model:
   - Run the training script to train the LSTM model on the cleaned data:
   ```bash
   python ML Assembly.ipynb --input_file data/Clean Data.pkl --output_model models/btc_ml_model.keras

4. Make predictions:
   - Use the trained model to make predictions on new data.
