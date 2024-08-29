# Forecasting the Electric Power Consumption of a Household

## Objective

The objective of this capstone project is to build and evaluate models that can accurately forecast the next 24 hours of global active power consumption in a household. This project explores various deep learning models to determine the most effective approach for time series forecasting.

## Dataset

The dataset contains household electric power consumption data, including features like global active power, global reactive power, voltage, global intensity, and energy sub-metering. The data is recorded at one-minute intervals.

## Steps to Achieve the Objective

1. **Data Preprocessing:**
   - Handled missing values and converted data types.
   - Combined the Date and Time columns into a DateTime object.
   - Resampled the data by hour.

2. **Feature Engineering:**
   - Identified seasonality patterns.
   - Encoded time using sine and cosine transformations.
   - Scaled the data for model training.

3. **Data Splitting:**
   - Split the dataset into 70% training, 20% validation, and 10% testing sets.

4. **Modeling:**
   - Implemented and trained multiple models:
     - Baseline Linear Regression
     - LSTM, GRU, BiLSTM
     - CNN and hybrid models (CNN+LSTM, CNN+GRU)
     - Deep Neural Networks (DNN)

5. **Model Evaluation:**
   - Evaluated models using the R² score on the test data.
   - **Best Model:** GRU with an R² score of 0.6067.

## Results

The GRU model emerged as the best-performing model, achieving an R² score of 0.6067 on the test dataset, indicating a strong fit for forecasting household power consumption.

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/Pritam0112/Forecasting-the-electric-power-consumption-of-a-household.git
   ```
2. Install the required dependencies:

3. Run the Jupyter notebook or Python scripts to reproduce the results.

## Conclusion

This project demonstrates the power of deep learning models, particularly GRU, in effectively forecasting time series data like household power consumption. The approach can be further extended to other similar forecasting problems.
