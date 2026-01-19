# AlexNet Implementation on CIFAR-10

## About
This project implements the AlexNet Convolutional Neural Network architecture from scratch using PyTorch. The goal is to study the architecture's specific layer dimensions, pooling operations, and training dynamics. The main logic is contained within `alex.ipynb`, which covers data loading, model definition, training loops, and evaluation.

## Directory Structure
```text
.
├── alex.ipynb      # Main notebook containing model architecture and training loop
├── data/           # Directory for CIFAR-10 dataset (downloaded automatically)
├── models/         # Saved model weights (.pth files)
│   └── format: model_dataset_device_epochs_timestamp_accuracy.pth
├── images/         # External images used for testing inference
└── .gitignore
