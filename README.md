# MNP
This repository contains the practical exercises for the course "Nonparametric Methods". The exercises are provided in both R Markdown (`.rmd`) and PDF (`.pdf`) formats. Below is a summary of the tasks covered in each exercise.

---

## Exercise 1

This exercise focuses on **goodness-of-fit tests** for detecting deviations from a standard normal distribution. The tasks include:

1. **Empirical Evaluation**:
   - Generate 500 random samples of size \( n = 30 \) from a specified normal distribution \( N(0, \sigma) \) where \( 0 < \sigma < 0.5 \).
   - Apply the **Kolmogorov-Smirnov**, **Cramer-von Mises**, and **Anderson-Darling** tests to each sample.
   - Calculate the relative frequency of rejections at a significance level of \( \alpha = 0.05 \).

2. **Analysis of p-values**:
   - Analyze the p-values obtained from each test using histograms, box plots, and descriptive statistics.
   - Compare the performance of the three tests and discuss the results.

3. **General Function**:
   - Develop a function to perform the above steps for arbitrary values of \( n \), \( \sigma \), and \( \alpha \).

4. **Type I Error Probability**:
   - Verify that the probability of Type I error is approximately \( \alpha = 0.05 \) by generating 500 samples from \( N(0, 1) \).
   - Perform a similar analysis of the p-values to confirm the results.

---

## Exercise 2

This exercise involves the analysis of a dataset (`RIKZ.rda`) containing species richness data from 45 locations across 9 beaches in the North Sea. The tasks include:

1. **Nonparametric Estimation**:
   - Estimate the cumulative distribution function (CDF) of species richness (\( Richness \)) and compare it with a normal distribution.
   - Estimate \( P(Richness \leq r) \) for \( r = 7 \) and \( 21 \).
   - Test the normality of \( Richness \) using a nonparametric test.

2. **Density Estimation**:
   - Provide nonparametric kernel density estimates of \( Richness \) using two different smoothing parameters (\( h_1 \) and \( h_2 \)).
   - Compare the density estimates with a normal distribution and estimate the density at \( r = 7 \) and \( 21 \).
   - Test the normality of \( Richness \) using a density-based test.

3. **Modeling Relationship**:
   - Model the relationship between \( Richness \) and \( NAP \) (height relative to mean low tide) using:
     - Local linear regression.
     - Nadaraya-Watson estimator.
   - Compare the results and check for linearity.

4. **LOESS Fit**:
   - Fit the relationship between \( Richness \) and \( NAP \) using the LOESS algorithm.
   - Determine an appropriate span value, interpret its meaning, and analyze the degrees of freedom and residual variance of the fit.
