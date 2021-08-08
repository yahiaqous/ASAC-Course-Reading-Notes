# Linear regression in Python and scikit-Learn

Linear regression is one of the **fundamental statistical** and **machine learning techniques**.

**Scikit-learn** is a powerful **Python module for machine learning**. It contains functions for regression, classification, clustering, model selection, and dimensionality reduction.

Regression problems usually have **one continuous and unbounded dependent variable** The inputs, however, can be continuous, discrete, or even categorical data such as gender, nationality, brand, and so on.

Regression is needed to answer whether and how some phenomenon influences the other or how several variables are related.

Residual plots are a good way to visualize the errors in your data. If a good job has been done then the data should be randomly scattered around line zero. If the structure is seen in the data, that means the model is not capturing something. Also useful when you want to forecast a response using a new set of predictors

Linear regression is implemented with the following:

- **scikit-learn** if you don’t need detailed results and want to use the approach consistent with other regression techniques

- **statsmodels** if you need the advanced statistical parameters of a model

Problems that might follow the choice of the degree:

- **Underfitting** occurs when a model can’t accurately capture the dependencies among data, usually as a consequence of its own simplicity.

- **Overfitting** happens when a model learns both dependencies among data and random fluctuations. In other words, a model learns the existing data too well. Complex models, which have many features or terms, are often prone to overfitting.

There are five basic steps when **implementing linear regression**:

1. Import the packages and classes needed.

2. Provide data to work with and eventually do appropriate transformations.

3. Create a regression model and fit it with existing data.

4. Check the results of model fitting to know whether the model is satisfactory.

5. Apply the model for predictions.
