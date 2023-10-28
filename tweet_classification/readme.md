# Tweet Classification with TensorFlow Decision Forests

## Overview
This project employs TensorFlow Decision Forests (TF-DF) to categorize tweets. The models utilize a Universal Sentence Encoder for text embedding, and two Gradient Boosted Trees models (model_1 and model_2) for classification.

## Dataset
The training data is sourced from a CSV file available [here](https://raw.githubusercontent.com/IMvision12/Tweets-Classification-NLP/main/train.csv). Columns 'id', 'keyword', and 'location' are dropped, leaving only 'text' and 'target'. The dataset is shuffled and split into training and validation sets.

## Model Architecture
- **Input Preprocessing:** The Universal Sentence Encoder converts tweet text into numerical representations.
- **Model 1:** TF-DF Gradient Boosted Trees Model with a preprocessing layer.
- **Model 2:** TF-DF Gradient Boosted Trees Model without a preprocessing layer.

## Training
Both models are compiled with metrics such as Accuracy, Recall, Precision, and AUC. They are trained for one epoch using the training dataset.

## Evaluation
Model performance is visualized using training logs, and evaluation metrics are computed for both model_1 and model_2 on the validation set.

## Results
The training logs and evaluation metrics are plotted and displayed for analysis. Additionally, a subset of the validation set is used to showcase individual predictions made by model_1.

## How to Use
1. Install necessary libraries: `pandas`, `numpy`, `tensorflow`, `tensorflow_hub`, `tensorflow_decision_forests`, and `matplotlib`.
2. Load the dataset from the provided CSV link.
3. Preprocess the data and split it into training and validation sets.
4. Create TensorFlow datasets for training and testing.
5. Build the model architecture with the Universal Sentence Encoder and TF-DF Gradient Boosted Trees.
6. Train the models using the training dataset.
7. Evaluate model performance on the validation set.
8. Visualize training logs and evaluation metrics.
9. Make predictions on a subset of the validation set using model_1.

Feel free to customize the code and experiment with different hyperparameters for improved performance!
