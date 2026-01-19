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
```
## Results
The model was trained on the CIFAR-10 dataset (32x32 images upsampled to 224x224).
Epochs,Accuracy
10,60.55%
20,78.94%

### Why the accuracy increased
The improvement from 60% to 78% occurred because the model had twice as many iterations to perform backpropagation. Deep learning models require thousands of update steps for the weights to converge from random initialization to precise feature detectors. The additional epochs allowed the optimizer to minimize the loss function further and learn finer details distinguishing the classes.
