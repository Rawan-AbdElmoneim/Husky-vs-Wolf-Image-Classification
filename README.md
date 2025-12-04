# Husky-vs-Wolf-Image-Classification

## Project Overview
This project implements a convolutional neural network (CNN) for binary classification of images containing huskies and wolves. The model distinguishes between these two visually similar dog breeds using a dataset of background-removed images, allowing the network to focus on distinguishing features.

## Key Features
- **Binary Classification:** Distinguishes between huskies and wolves.  
- **Background-Removed Images:** Training images have transparent backgrounds for better feature learning.  
- **K-Fold Cross Validation:** 5-fold cross-validation for robust model evaluation.  
- **Data Augmentation:** Multiple augmentation techniques to improve model generalization.  
- **Regularization:** L2 regularization and dropout layers to prevent overfitting.  

## Model Architecture
The CNN architecture includes:  
- **Input Layer:** 128x128 RGB images  
- **Convolutional Layers:** Two Conv2D layers (32 and 64 filters) with BatchNormalization  
- **Pooling Layers:** MaxPooling2D for dimensionality reduction  
- **Regularization:** Dropout (0.5) and L2 regularization  
- **Output Layer:** Single neuron with sigmoid activation for binary classification  



## Model Configuration
### Hyperparameters

| Parameter         | Value                    |
| ----------------- | ------------------------ |
| Image Size        | 128x128                  |
| Batch Size        | 32                       |
| Learning Rate     | 1e-4                     |
| Epochs            | 10 (with early stopping) |
| Dropout Rate      | 0.5                      |
| L2 Regularization | 0.01                     |
| Optimizer         | Adam                     |
| Loss Function     | Binary Crossentropy      |


## Data Augmentation

Rotation Range: ±20°

Width/Height Shift: ±20%

Shear Range: 20%

Zoom Range: 20%

Horizontal Flip: Enabled

Fill Mode: Nearest
