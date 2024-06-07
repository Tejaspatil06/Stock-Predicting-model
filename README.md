# Stock Market Predictor

## Overview

This project is a Stock Market Predictor web application built using Streamlit. The app allows users to upload stock market data, specify a date range, and visualize predictions for the stock's closing prices. The model used for predictions is a pre-trained Keras model.

## Features

- Upload CSV files containing stock market data.
- Specify date ranges for predictions.
- Visualize training, validation, and testing predictions.
- Generate and visualize recursive predictions.

## Requirements

- Python 3.x
- Streamlit
- Pandas
- Numpy
- Matplotlib
- Keras

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/Tejaspatil06/Stock_Predicting-model.git
    ```
2. Navigate to the project directory:
    ```bash
    cd Stock-Predicting-model
    ```
3. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. Start the Streamlit app:
    ```bash
    streamlit run app.py
    ```
2. Obtain your CSV file containing stock market data from [Yahoo Finance](https://finance.yahoo.com). The file should have columns for `Date` and `Close` prices.
3. Upload the CSV file.
4. Use the sidebar to select the start and end dates for the prediction window.
5. Visualize the predictions for training, validation, and testing datasets.

## File Structure

- `app.py`: Main Streamlit application file.
- `Stock_Predictions_Model.keras`: Pre-trained Keras model for stock predictions.
- `requirements.txt`: List of required Python packages.

## Custom CSS

The application uses custom CSS to enhance the UI. The CSS is defined in the `custom_css` variable within `app.py` and is applied using Streamlit's `st.markdown` method.


## Model Training and Predictions

The application uses a pre-trained Keras model (`Stock_Predictions_Model.keras`) for making predictions. The model is loaded and used to predict stock closing prices for the specified date ranges. The predictions are split into training, validation, and testing datasets and are visualized using Matplotlib.

## Visualization

The application visualizes the following:
- Training Predictions
- Validation Predictions
- Testing Predictions
- Combined Plot of all predictions
- Recursive Predictions

## Customization

You can modify the application by:
- Changing the date range window size in the `df_to_windowed_df` function.
- Using a different pre-trained model by replacing the `Stock_Predictions_Model.keras` file.
- Adjusting the CSS for a different look and feel.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request for any improvements or bug fixes.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---
