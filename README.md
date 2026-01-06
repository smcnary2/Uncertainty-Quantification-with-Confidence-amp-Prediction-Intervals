# Uncertainty-Quantification-with-Confidence-amp-Prediction-Intervals
## Objective
The goal of this analysis is to demonstrate linear regression and interval estimation using simulated data. The project highlights the distinction between confidence intervals for the mean response and prediction intervals for individual observations.

---

## Data
Data were generated from the linear model:

y = β₀ + β₁x + ε

where:
- β₀ = 0.5
- β₁ = 5
- ε ~ N(0, 25)

The predictor variable `x` was sampled evenly over the interval [1, 15].

---

## Methodology
A simple linear regression model was fit using ordinary least squares. Model parameters were estimated and residuals were analyzed to compute the residual standard error.

Both confidence and prediction intervals were calculated:
- Manually, using standard regression formulas
- Using R’s built-in `predict()` function

This dual approach verifies theoretical results against software output.

---

## Results
The fitted regression line closely matches the true data-generating relationship. Confidence intervals are relatively narrow and centered around the regression line, reflecting uncertainty in estimating the mean response. Prediction intervals are wider, reflecting both estimation uncertainty and random noise in individual observations.

---

## Conclusion
This analysis demonstrates that prediction intervals are always wider than confidence intervals due to the presence of irreducible error. The results reinforce the importance of distinguishing between estimating an average trend and predicting individual outcomes in regression analysis.

---

## Tools
- R (base functions only)
