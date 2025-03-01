# Deep Learning Project: Linear Regression with PyTorch

This repository contains a PyTorch implementation of a linear regression model, trained on the advertising dataset.  The project demonstrates a step-by-step approach to building and training a basic neural network model.

## Project Structure

The project is structured as a Jupyter Notebook (`linear_regression_project.ipynb`), which includes the following sections:

1.  **Data Loading and Preparation:**
    *   Loads the `advertising.csv` dataset using pandas.
    *   Converts the data into PyTorch tensors.
    *   Splits the data into training (80%) and testing (20%) sets.
    *  Visualize the raw data.

2.  **Model Definition:**
    *   Defines a custom `LinearRegressionModel` class that inherits from `nn.Module`.
    *   Implements the `__init__` method to initialize the weights (as a single tensor) and bias.
    *   Implements the `forward` method to perform the linear transformation:  `y = w^T x + b`.

3.  **Model Training:**
    *   Creates an instance of the `LinearRegressionModel`.
    *   Selects the Adam optimizer and sets a learning rate.
    *   Uses Mean Absolute Error (MAE) as the loss function.
    *   Implements a training loop that performs:
        *   Forward pass
        *   Loss calculation
        *   Backpropagation
        *   Parameter updates (using the optimizer)
        *   Testing loss Evaluation
        *   Loss Tracking
    *   Prints the training and testing loss periodically.

4.  **Visualization:**
    *   Plots the training and testing loss curves over iterations.
    *   Plots the training data, testing data, and the fitted regression line, using the first dimension ('TV' advertisement) from dataset.

## Dependencies

*   Python 3
*   PyTorch (>= 1.3)
*   NumPy
*   Pandas
*   Matplotlib
*   scikit-learn
