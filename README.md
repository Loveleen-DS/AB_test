# Conversion Rate Analysis

## Overview

This notebook provides a detailed analysis of conversion rates through a step-by-step approach. By leveraging A/B testing and logistic regression techniques, the analysis aims to assess whether introducing a new landing page leads to an increase in user conversions. The methods used in this notebook can help businesses optimize key performance indicators (KPIs) such as conversion rates, customer acquisition costs, and overall revenue.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Analysis Workflow](#analysis-workflow)
- [Methods Used](#methods-used)
- [Conclusion](#conclusion)
- [Future Considerations](#future-considerations)
- [Dependencies](#dependencies)

## Introduction

In today's data-driven business landscape, understanding what drives customer behavior is crucial. This notebook explores whether a new landing page design can positively impact user conversions, using a combination of simple conversion analysis, A/B testing, and regression analysis. These techniques not only provide a straightforward comparison but also delve into the relationships between multiple variables, offering deeper insights.

## Dataset

The analysis uses two datasets:

1. **Main Conversion Data**: Contains information on user interactions with the landing pages, including whether a conversion took place.
2. **Country Data**: Provides information on the country of origin for each user, used for additional regression analysis.

## Analysis Workflow

The notebook is divided into three main parts:

1. **Simple Conversion Analysis**: This section explores the conversion rates between the control and treatment groups to see if the new landing page shows an improvement over the old one.
   
2. **One-Tailed T-Test (A/B Test)**: A statistical test is performed to determine if the new landing page leads to a statistically significant increase in conversions compared to the control page.

3. **Regression Analysis**:
   - **Univariate Logistic Regression**: Assesses the impact of the new landing page on conversions.
   - **Multivariate Logistic Regression**: Adds additional variables (e.g., country) to see if there are other factors that influence conversion rates.

## Methods Used

- **Conversion Rate Analysis**: Basic comparison of conversion rates between groups.
- **One-Tailed T-Test**: A statistical test to compare the means of two groups.
- **Logistic Regression**: A statistical model used to predict the probability of a binary outcome (conversion vs. no conversion) based on one or more predictor variables.

## Conclusion

All three methods—simple conversion analysis, one-tailed t-test, and logistic regression—converge on the same conclusion: the introduction of the new landing page does not significantly impact conversion rates. However, this conclusion should be carefully considered, especially since the p-value was not examined in detail step-by-step as data was received but rather at a later stage.

## Future Considerations

While this analysis provides valuable insights, there are limitations:
- **Model Complexity**: Adding more variables to the regression model could make it more complex and less interpretable.
- **Overfitting Risk**: Incorporating too many variables, such as timestamps, may lead to overfitting.
- **P-Value Sensitivity**: Future analyses should monitor p-values as data is received to ensure accurate real-time insights.

Additional features, such as user behavior patterns or time-based effects, could be explored in future iterations to refine the model further.

## Dependencies

The following Python libraries are required to run the notebook:

- pandas
- numpy
- statsmodels
- matplotlib (optional, for data visualization)

## How to Use

1. Clone the repository.
2. Ensure that the necessary datasets are in the correct directory.
3. Run the notebook step-by-step to reproduce the analysis.
