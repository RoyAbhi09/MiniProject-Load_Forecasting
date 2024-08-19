
# Power System Load Forecasting Automation using Artificial Neural Network

This project is conducted under the guidance of **Professor Mousumi Basu** from Department of Power Engineering, focuses on automating power system load forecasting using advanced machine learning techniques. The primary goal is to develop a robust forecasting model to predict future power loads accurately, which is crucial for efficient energy management and planning.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Data Preprocessing](#data-preprocessing)
- [Model Architecture](#model-architecture)
- [Training and Optimization](#training-and-optimization)
- [Performance Evaluation](#performance-evaluation)
- [Conclusion](#conclusion)
- [References](#references)

## Introduction

Load forecasting is a critical component of power system planning and operation. Accurate forecasts enable utilities to make informed decisions regarding generation, transmission, and distribution. This project leverages Artificial Neural Networks (ANN) to create a reliable load forecasting model.

## Dataset

The dataset used in this project contains historical power load data. It includes various features that influence power consumption, such as:

- Date and time
- Weather conditions (temperature, humidity, etc.)
- Historical load data

## Data Preprocessing

### Outlier Removal

Outliers in the dataset were identified and removed using two techniques:

**Z-score Method**: Statistical method to remove data points that are more than three standard deviations away from the mean.

### Data Scaling

Data was standardized to have a mean of 0 and a standard deviation of 1. This was achieved using the following formula:

\[ Z = \frac{(X - \mu)}{\sigma} \]

Where:
- \(X\) is the original data point
- \(\mu\) is the mean of the data
- \(\sigma\) is the standard deviation

## Model Architecture

The ANN model developed for this project consists of four layers, each containing 100 neurons. The architecture details are as follows:

- **Activation Function**: Rectified Linear Unit (RELU)
- **Optimizer**: Adam optimizer for adaptive learning rate

### Model Summary
 The model consists of four dense layers: the first with 64 neurons, followed by layers with 32 and 16 neurons, all using ReLU activation. The final layer has 1 neuron with linear activation, ideal for regression tasks.

## Training and Optimization

The model was trained using the Adam optimizer, which combines the best properties of the AdaGrad and RMSProp algorithms to provide an adaptive learning rate. The objective was to minimize the Mean Squared Error (MSE) between the predicted and actual load values.

## Performance Evaluation

The model's performance was evaluated using the R² score, which measures the proportion of variance in the dependent variable predictable from the independent variables. The model achieved an R² score of approximately near to **0.93** on the testing dataset, indicating high predictive accuracy.

## Conclusion

The developed ANN model successfully automates power system load forecasting with high accuracy. The preprocessing steps, including outlier removal and data scaling, significantly contributed to the model's performance. This project demonstrates the potential of machine learning techniques in enhancing power system operations.

## References

- [Adam: A Method for Stochastic Optimization](https://arxiv.org/abs/1412.6980)

---
