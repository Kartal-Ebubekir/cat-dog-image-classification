# Cat vs Dog Image Classification

A binary image classification project developed using PyTorch and Convolutional Neural Networks (CNN).

## Project Overview

The goal of this project is to classify images into two categories: Cat and Dog.

The Oxford-IIIT Pet dataset was used, containing 37 different pet breeds mapped into two classes.

## Dataset

- Training images: 3,128
- Validation images: 552
- Test images: 3,669
- Input image size: 128 × 128 RGB

## Model Architecture

A custom CNN architecture consisting of:

- Three convolutional blocks (32, 64, 128 filters)
- Batch Normalization
- ReLU activation
- Max Pooling
- Adaptive Average Pooling (4 × 4)
- Fully Connected layer (256 units)
- Dropout (0.5)
- Two output classes

## Training Configuration

- Framework: PyTorch
- Optimizer: Adam
- Learning rate: 0.001
- Batch size: 32
- Epochs: 15
- Loss function: Weighted CrossEntropyLoss
- Hardware: NVIDIA Tesla T4 GPU

## Results

- Best validation accuracy: 78.62%
- Test accuracy: **80.49%**
- Dog F1-score: 85.34%
- Cat F1-score: approximately 71%

## Additional Features

- Model evaluation using confusion matrix, precision, recall and F1-score.
- Inference time measurement.
- Real-world image testing.
- Interactive prediction interface built with Gradio.

## Technologies

Python, PyTorch, Torchvision, NumPy, Matplotlib, Scikit-learn, Gradio, Google Colab.

## Limitations

The model performs better on the Dog class than the Cat class. Class imbalance and limited dataset diversity may affect classification performance.

This project was developed for learning and practical exploration of deep learning and computer vision.
