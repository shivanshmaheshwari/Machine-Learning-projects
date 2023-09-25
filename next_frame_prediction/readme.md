# Next Frame Prediction with Machine Learning

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

## Overview

This project implements a Next Frame Prediction model using machine learning techniques. The goal of this project is to predict the next frame in a sequence of images or video frames, which can have applications in various domains, including video compression, surveillance, and action recognition.

### Prerequisites

Before you begin, ensure you have met the following requirements:

- Python 3.x (with pip)
- [Virtual environment](https://docs.python.org/3/library/venv.html) (recommended)

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/next-frame-prediction.git
   cd next-frame-prediction

## Dataset

We used the Moving MNIST dataset for training and testing our Next Frame Prediction model. This dataset consists of sequences of handwritten digits that move within a frame, making it suitable for tasks involving video prediction.

To acquire the dataset, you can use the following code snippet:

```python
fpath = keras.utils.get_file(
    "moving_mnist.npy",
    "http://www.cs.toronto.edu/~nitish/unsupervised_video/mnist_test_seq.npy",
)
dataset = np.load(fpath)
```

### Results

![Next Frame Prediction Result](https://github.com/shivanshmaheshwari/Machine-Learning-projects/assets/78491674/e4522459-0aa6-4a4f-bb73-f5e138f458a7.png)

The image above represents the output of our Next Frame Prediction model. In this project, we trained the model to predict the next frame in a sequence of images or video frames. The result demonstrates the model's ability to generate a plausible next frame based on the input data.

This output showcases the potential applications of our model, which include video compression, action recognition, and various computer vision tasks. The quality of the predicted frames can be further improved through fine-tuning and experimentation with hyperparameters.


  

