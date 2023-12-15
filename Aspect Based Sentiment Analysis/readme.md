# Sentiment Analysis Model README

## Overview

This repository contains code for a sentiment analysis model implemented using a neural network with a Bidirectional LSTM architecture. The model is designed to analyze sentiments in text based on given aspects.

## Files

- **train.csv:** This CSV file contains the training data with columns 'text', 'aspect', and 'label'.
- **test.csv:** This CSV file contains the test data with columns 'text' and 'aspect'.
- **sentiment_analysis_model.ipynb:** This Jupyter notebook contains the code for training, evaluating, and using the sentiment analysis model.

## Code Explanation

1. **Data Loading and Preprocessing:**
   - Training data is loaded from `train.csv`.
   - Text and aspect columns are tokenized and padded using Keras' Tokenizer and pad_sequences.

2. **Model Architecture:**
   - The model has two branches for text and aspect inputs, each consisting of an Embedding layer and a Bidirectional LSTM layer.
   - Outputs from both branches are concatenated and passed through fully connected layers with dropout for regularization.

3. **Training the Model:**
   - The model is trained on the training data with early stopping and learning rate reduction callbacks.

4. **Saving Label Encoder:**
   - The LabelEncoder is saved to a file using pickle for later use.

5. **Testing the Model:**
   - Test data is loaded and preprocessed similarly to the training data.
   - The model predicts sentiment labels for the test data.

6. **Label Decoding:**
   - Predicted labels are inverse-transformed using the saved LabelEncoder to obtain the original sentiment labels.

7. **Example Predictions:**
   - The code provides an example by printing the first few predictions from the test data.

8. **Custom Predictions:**
   - Two examples of custom predictions are included using user-defined sentences and aspects.

## Usage

1. Open the Jupyter notebook `sentiment_analysis_model.ipynb` in a compatible environment.
2. Run each cell sequentially to train the model, evaluate its performance, and make predictions on new data.
3. The model architecture is visualized and saved as `model_architecture.png`.
4. The LabelEncoder used for sentiment labels is saved as `label_encoder.pkl`.
5. Custom predictions can be made by modifying the `custom_sentence` and `custom_aspect` variables in the notebook.

## Requirements

- Python 3.x
- Jupyter Notebook
- TensorFlow
- Scikit-learn
- Pandas
- Numpy



## License

This project is licensed under the [MIT License](LICENSE).
