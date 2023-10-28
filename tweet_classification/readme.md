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
- **Model 1 Evaluation:**
  - Loss: 0.0000
  - Accuracy: 0.8055
  - Recall: 0.7126
  - Precision: 0.8378
  - AUC: 0.8668

- **Model 2 Evaluation:**
  - Loss: 0.0000
  - Accuracy: 0.5440
  - Recall: 0.0029
  - Precision: 1.0000
  - AUC: 0.5026
 
The training logs and evaluation metrics are plotted and displayed for analysis. Additionally, a subset of the validation set is used to showcase individual predictions made by model_1.The plotted graphs illustrate the dynamic relationship between the number of trees in the ensemble and the accuracy achieved by both Model 1 and Model 2 during training. On the y-axis, the accuracy metric is depicted, serving as a measure of the models' performance, while the x-axis showcases the progression of the number of trees used in the Gradient Boosted Trees models. The curves provide insights into how the models' accuracy evolves as the ensemble size grows, offering a visual representation of their learning process. These plots are crucial for understanding the trade-off between model complexity (as determined by the number of trees) and performance, helping to identify the point of optimal accuracy and potential indications of overfitting or underfitting in the training process.

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
