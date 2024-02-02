# Medical Insurance Causal Inference

## Overview

This project performs causal analysis on a health insurance dataset to determine the effect of smoking on healthcare costs. It utilizes various causal inference techniques like randomized controlled trials (RCTs), instrumental variables (IV), propensity score matching (PSM), and difference-in-differences (DiD) to estimate the causal impact.

The dataset contains information on age, gender, BMI, number of children, region, smoking status, and healthcare charges for 1,338 patients.

## Code Overview

The Jupyter notebook walks through the following steps:

1. Imports libraries and reads in the dataset
2. Performs exploratory data analysis and visualization 
3. Applies four causal inference methods:
   - RCTs: Compares charges for smokers vs non-smokers
   - IV: Uses BMI as an instrument variable 
   - PSM: Matches smokers and non-smokers using propensity scores 
   - DiD: Uses region as a treatment variable
4. Extracts and visualizes the causal effects from each method

## Key Findings

The analysis estimates the increase in healthcare costs due to smoking between $23,594 and $39,612 depending on method. This suggests smoking significantly increases annual healthcare expenditures by $24k to $40k per patient.

Propensity score matching creates the most balanced smoker/non-smoker groups for comparison. The DiD method differences out time-invariant unobserved factors.

## Requirements

The analysis requires Python 3 and the following key libraries:

- Pandas, NumPy 
- Matplotlib, Seaborn
- Scikit-learn, Statsmodels
- causalnex

The notebook is designed to run in Colab with all dependencies included.
