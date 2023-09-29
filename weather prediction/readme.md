# Climate Data Analysis with LSTM

This project involves the analysis of climate data using Long Short-Term Memory (LSTM) networks. The code provided includes data download, visualization, preprocessing, model training, and prediction.

## Data

The climate data used in this project is sourced from the [Jena Climate dataset](https://storage.googleapis.com/tensorflow/tf-keras-datasets/jena_climate_2009_2016.csv.zip). The data includes various features such as pressure, temperature, humidity, and wind speed recorded over several years.

## Code Structure

The code is organized into several sections:

1. **Data Download and Preprocessing:**
   - Downloads the Jena Climate dataset and performs basic preprocessing.

2. **Raw Data Visualization:**
   - Visualizes raw time series data including features like pressure, temperature, and wind speed.

3. **Heatmap Visualization:**
   - Generates a heatmap showing the correlation between different features.

4. **Data Preprocessing:**
   - Splits the data into training and validation sets, normalizes the features, and prepares time series datasets.

5. **Model Definition and Training:**
   - Defines an LSTM model, compiles it, and trains it using the prepared datasets.

6. **Visualizing Training History:**
   - Plots the training and validation loss over epochs to assess model performance.

7. **Prediction and Plotting:**
   - Uses the trained model to make predictions on the validation dataset and visualizes the results.

## How to Use

1. Clone the repository:

   ```bash
   git clone https://github.com/shivanshmaheshwari/Machine-Learning-projects/tree/main/weather%20prediction
   cd climate-data-analysis
    ```
2. Run the Jupyter Notebook or Python script:

    ```bash
    jupyter notebook  # or python script.py
    ```

3.Explore the visualizations and analysis results.

## **Dependencies:**
    - tensorflow
    - matplotlib
    - pandas






