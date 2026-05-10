# Linear Regression from Scratch

Most people learn linear regression by calling `.fit()`. This skips that.

Built the entire optimizer by hand - loss function, partial derivatives, 
gradient descent loop - using only NumPy and pandas. No sklearn until the 
end, where I run the same data through it to verify my MSE matches.

## What's in the notebook

- MSE loss function defined and explained
- Partial derivatives of the loss w.r.t slope and bias derived manually
- Gradient descent loop implemented from scratch
- Learning rate experiments — what happens when it's too big or too small
- Final comparison against sklearn's solution

## Math at the core

The update rules driving everything:

m = m - α · (∂L/∂m)
b = b - α · (∂L/∂b)

Where α is the learning rate and the gradients tell us which 
direction to step to reduce the loss.

## Run it

```bash
pip install -r requirements.txt
# then open linear_regression_from_scratch.ipynb
```

## Stack
Python · NumPy · pandas · Matplotlib · Seaborn
