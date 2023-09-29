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
   git clone https://github.com/shivanshmaheshwari/Machine-Learning-projects
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
## **Results:**
![image](https://github.com/shivanshmaheshwari/Machine-Learning-projects/assets/78491674/5fe76697-0d75-42a8-a973-ee0775977b06)
The visual representation above provides a snapshot of the project's key outcomes. The plot showcases the model's performance in single-step predictions on the climate dataset. The blue curve represents the historical data, offering insights into the patterns and trends leading up to the present. The red 'X' markers denote the true future values, providing a benchmark for evaluating the model's accuracy. The green dots represent the model's predictions, illustrating its ability to capture and forecast climate variables. The alignment between the red markers and green dots reflects the model's effectiveness in predicting future values. Overall, this visualization serves as a qualitative assessment of the LSTM model's proficiency in forecasting climate data.





