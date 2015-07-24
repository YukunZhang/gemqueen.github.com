---
layout: post
title: Something about Bootstrap
modified: 2015-07-24

---
We can approximate the sampling distribution of some statistic by booststapping.

There are three major ways of doing this

1. Parametric bootstrap: Estimate the model and then simulate from the estimated model.
 In this case, it trusts that we have the right shape for the regression function and the right distribution for the noise.
2. Resampling residuals: Estimate the model and then simulate by resampling residuals to that estimate and adding them back to the fitted values.
In this case, it assumes the shape of the regression function right but not the distribution of residuals. It is more secure than parametric bootstrap
3. Resampling cases or whole data point: ignore the estimated model, just re-sampling whole rows from the data frame. 
   In this case, it is the safest, but there is a bias-variance trade-off. it gives the narrowest intervals.
