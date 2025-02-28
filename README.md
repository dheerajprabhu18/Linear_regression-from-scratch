# Linear Regression from Scratch 🚀

This repository contains an implementation of **Linear Regression** from scratch using NumPy. The goal is to understand how linear regression works under the hood without relying on libraries like scikit-learn.

## Features
- Supports **batch gradient descent** for optimization.
- Adjustable **learning rate** (`lr`) and **epochs** for training.
- Handles **bias (intercept) inclusion** automatically.
- Works with **multiple features** (multivariate regression).

## Key Observations
- Works efficiently for **large datasets**, where scikit-learn might struggle with high values of `X`.
- For smaller datasets (thousands of rows), **scikit-learn is faster**.
- The learning rate (`lr`) should be **between 0.1 and 0.5**, as higher values cause instability.
- The **loss function reduces gradually**, showing proper convergence.

## Sample Usage
```python
import numpy as np
from linear_regression import LinearRegression

# Sample dataset
X = np.array([[1, 2], [3, 4], [5, 6], [7, 8]])
y = np.array([[3], [7], [11], [15]])

# Initialize and train model
model = LinearRegression(lr=0.1, epochs=500)
model.train(X, y)

# Make predictions
predictions = model.predict(X)
print("Predictions:", predictions)
