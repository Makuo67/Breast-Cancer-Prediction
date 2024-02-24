# Breast Cancer Classification Model

## Overview

This project focuses on building a classification model to predict breast cancer using the Wisconsin Breast Cancer dataset. The dataset contains features computed from a digitized image of a fine needle aspirate (FNA) of a breast mass.

## Model Training

### Model 1: No Optimization

I initially trained a model without any optimization techniques, and the results were as follows:

- Training Accuracy: 89.45%
- Test Accuracy: 92.11%

### Model 2: Adam Optimization

For the second model, I employed the Adam optimization technique. Adam is an adaptive learning rate optimization algorithm that combines ideas from both Momentum and RMSProp. The model was trained with the following results:

- Training Accuracy: 100.00%
- Test Accuracy: 96.49%

#### Adam Optimization Parameters

- Learning Rate: 0.00005 
- *Reason*: To ensure small and stable weight updates
- Batch Size: 32 (default value)

### Model 3: Stochastic Gradient Descent (SGD)

The third model utilized Stochastic Gradient Descent as the optimization algorithm. SGD is a classic optimization algorithm that updates the weights using the gradients of the loss function with respect to the weights. However, the results were suboptimal:

- Training Accuracy: 62.86%
- Test Accuracy: 62.28%

#### SGD Optimization Parameters

- Learning Rate: 0.9
- *Reason*: To traverse through shallow local minima and accelerate convergence.
- Batch Size: 32

### Model 4: Root Mean Square (RMS)

For the fourth model, I applied the Root Mean Square (RMS) optimization technique. RMSProp adapts the learning rates of each parameter by dividing the learning rate by the moving average of the squared gradients. The model achieved the following results:

- Training Accuracy: 100.00%
- Test Accuracy: 96.49%

#### RMS Optimization Parameters

- Learning Rate: 0.001 (default value)
- Batch Size: 32 (default value)

## Conclusion

The results demonstrate the effectiveness of optimization techniques in improving model performance. The Adam and RMS optimization methods outperformed the model trained without optimization by 4.38%, achieving higher accuracy on both the training and test sets.


