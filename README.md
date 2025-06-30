# Fashion-MNIST Dimension Reduction Using Autoencoder

A deep learning project implementing autoencoder neural networks for dimension reduction on the Fashion-MNIST dataset.

## Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Features](#features)
- [Model Architecture](#model-architecture)
- [Results](#results)

## Overview

This project demonstrates dimension reduction techniques using autoencoder neural networks on the Fashion-MNIST dataset. The implementation reduces high-dimensional image data from 784 dimensions (28×28 pixels) to 128 dimensions while preserving essential visual information.

**Key Objectives:**
- Implement baseline autoencoder architecture
- Optimize model performance through architectural improvements
- Evaluate reconstruction quality using Structural Similarity Index (SSIM)
- Perform hyperparameter tuning for enhanced results

## Dataset

**Fashion-MNIST** contains 70,000 grayscale images of fashion items:
- **Image Size**: 28×28 pixels (784 features)
- **Classes**: 10 categories (T-shirt, Trouser, Pullover, Dress, Coat, Sandal, Shirt, Sneaker, Bag, Ankle boot) and only 2 categories that is used in this project (Pullover, and Dress)
- **Split**: 80% training, 10% validation, 10% testing

## Features

- **Data Preprocessing**: Loading, scaling, reshape, and visualization
- **Baseline Model**: Simple encoder-decoder architecture
- **Optimized Model**: Enhanced architecture
- **Performance Evaluation**: SSIM 
- **Hyperparameter Tuning**: Systematic optimization
- **Visualization**: Original vs reconstructed images

## Model Architecture

### Baseline Autoencoder
```
Encoder: 784 → 512 → 256 → 128
Decoder: 128 → 256 → 512 → 784
```

### Optimized Autoencoder
- **Enhanced Features**: Dropout, Batch Normalization
- **Advanced Activations**: LeakyReLU
- **Regularization**: L2 weight decay
- **Adaptive Learning**: Learning rate scheduling

## Results

| Metric | Baseline Model | Optimized Model |
|--------|----------------|-----------------|
| SSIM Score | [To be filled] | [To be filled] |
| MSE Loss | [To be filled] | [To be filled] |

## Technologies Used

- **TensorFlow/Keras** - Deep learning framework
- **NumPy** - Numerical computing
- **Matplotlib** - Visualization
- **Scikit-image** - SSIM calculation
- **Pandas** - Data manipulation
