# ResNet on FashionMNIST

This repository contains a PyTorch implementation of the ResNet architecture (specifically ResNet-50) built entirely from scratch. I used the FashionMNIST dataset to train and test the model.

## What's in this project?
Instead of just importing a pre-built model from `torchvision`, I wrote the ResNet classes (`BasicBlock` and the main `ResNet` module) manually. This project was a great way to understand exactly how skip connections and residual layers work under the hood.

The Jupyter notebook covers:
- **Data Prep:** Loading the FashionMNIST dataset, resizing the images to 224x224, and converting them from grayscale to 3 channels so they work with standard ResNet dimensions.
- **Model Architecture:** Building ResNet-50 from the ground up.
- **Training:** A custom training and validation loop using the Adam optimizer and CrossEntropyLoss.
- **Evaluation:** Plotting the training and validation accuracy/loss curves over time using Matplotlib.

## Results
I trained the model for 10 epochs. By the end of the run, it achieved the following results:
- **Training Accuracy:** ~94.8%
- **Validation Accuracy:** ~91.5%

## How to run it locally
If you want to play around with the code yourself:

1. Make sure you have Python and Jupyter installed.
2. Install the required libraries. You can do this by running:
   ```bash
   pip install torch torchvision numpy matplotlib
