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


