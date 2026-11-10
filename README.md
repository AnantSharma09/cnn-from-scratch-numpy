# CNN From Scratch using NumPy

A Convolutional Neural Network (CNN) implemented entirely from scratch using NumPy and trained on the CIFAR-10 image classification dataset.

The goal of this project is to understand the mathematical foundations and internal mechanics of convolutional neural networks by implementing the core components without relying on deep learning frameworks such as PyTorch or TensorFlow.

## Project Overview

This project implements a CNN capable of classifying images into 10 different categories from the CIFAR-10 dataset.

The implementation covers the complete training pipeline, including forward propagation, loss computation, backpropagation, and parameter updates using mini-batch Stochastic Gradient Descent (SGD).

## Architecture

The model consists of the following layers:

- Conv2D (3 → 8 filters)
- ReLU
- Max Pooling
- Conv2D (8 → 16 filters)
- ReLU
- Max Pooling
- Flatten
- Fully Connected Layer (10 outputs)
- Softmax Cross-Entropy Loss

## Implemented Components

- Convolution operation using NumPy
- Efficient convolution forward pass using im2col
- Convolution backward propagation
- ReLU activation and its gradient
- Max pooling and backward propagation
- Flatten layer
- Fully connected layer
- Softmax cross-entropy loss
- Mini-batch SGD training
- Training and validation accuracy evaluation

## Dataset

CIFAR-10 consists of 60,000 color images of size 32 × 32 pixels distributed across 10 classes.

| Split | Images |
|---|---:|
| Training | 45,000 |
| Validation | 5,000 |
| Test | 10,000 |

The images are normalized before training.

## Technologies

- Python
- NumPy
- Matplotlib
- CIFAR-10

## Training

The model is trained using mini-batch SGD.

Training configuration:

- Training samples: 45,000
- Validation samples: 5,000
- Batch size: 32
- Learning rate: 0.01
- Epochs: 10

## Results

Training and validation results will be added after the training run completes.

| Metric | Result |
|---|---:|
| Training Accuracy | TBD |
| Validation Accuracy | TBD |
| Test Accuracy | TBD |

## What I Learned

- How convolution operations extract spatial features from images
- How gradients propagate through convolutional and pooling layers
- How to implement backpropagation manually
- How im2col transforms convolution into matrix multiplication
- How neural network parameters are updated through gradient descent
- How to construct an end-to-end deep learning training pipeline

## Future Improvements

- Implement gradient checking using numerical gradients
- Add learning rate scheduling
- Experiment with deeper CNN architectures
- Improve model performance on CIFAR-10
- Compare the NumPy implementation against a PyTorch implementation

## Running the Project

Clone the repository:

```bash
git clone https://github.com/AnantSharma09/cnn-from-scratch-numpy.git
cd cnn-from-scratch-numpy
```

Install dependencies:

```bash
pip install numpy matplotlib
```

Run the notebook:

```bash
jupyter notebook
```

Open the CNN implementation notebook and execute the cells.

## Author

Anant Sharma

[GitHub](https://github.com/AnantSharma09)
