# Linear Regressions
[Read](https://www.activestate.com/resources/quick-reads/how-to-run-linear-regressions-in-python-scikit-learn/)
### Can you explain the basic concept of linear regression and its purpose in the context of machine learning and data analysis?
  The basic idea behind linear regression is to fit a straight line that best represents the relationship between the independent variables (also called features or predictors) and the dependent variable (also known as the target or response variable). The line's equation is expressed as:
    `y = mx + b`
#### Regergetated from the reading answer...
  Linear regression can be thought of as finding the straight line that best fits a set of scattered data points: 
        - Best Fit – the straight line in a plot that minimizes the deviation between related scattered data points.
        - Coefficient – also known as a parameter, is the factor a variable is multiplied by. In linear regression, a coefficient represents changes in a Response Variable (see below).
        - Coefficient of Determination – the correlation coefficient denoted as 𝑅². Used to describe the precision or degree of fit in a regression. 
        - Correlation – the relationship between two variables in terms of quantifiable strength and degree, often referred to as the ‘degree of correlation’.  Values range between -1.  0 and       1.0. 
        - Dependent Feature – a variable denoted as y in the slope equation y=ax+b. Also known as an Output, or a Response. 
        - Estimated Regression Line – the straight line that best fits a set of scattered data points.
        - Independent Feature – a variable denoted as x in the slope equation y=ax+b. Also known as an Input, or a predictor. 
        - Intercept – the location where the Slope intercepts the Y-axis denoted b in the slope equation y=ax+b. 
        - Least Squares – a method of estimating a Best Fit to data, by minimizing the sum of the squares of the differences between observed and estimated values.
        - Mean – an average of a set of numbers, but in linear regression, Mean is modeled by a linear function.
        - Ordinary Least Squares Regression (OLS) – more commonly known as Linear Regression. 
        - Residual – vertical distance between a data point and the line of regression (see Residual in Figure 1 below).
        - Regression – estimate of predictive change in a variable in relation to changes in other variables (see Predicted Response in Figure 1 below).
        - Regression Model – the ideal formula for approximating a regression.
        - Response Variables – includes both the Predicted Response (the value predicted by the regression) and the Actual Response, which is the actual value of the data point (see   Figure      1 below).
        - Slope – the steepness of a line of regression. Slope and Intercept can be used to define the linear relationship between two variables: y=ax+b.
        - Simple Linear Regression – a linear regression that has a single independent variable.

### Describe the process of implementing a linear regression model using Python’s Scikit Learn library, including the necessary steps and functions.
This example demonstrates a simple case where there is only one independent variable. For multiple independent variables, the process remains the same, but the data should be appropriately shaped (e.g., a 2D array) and prepared before fitting the model:

        import numpy as np
        from sklearn.linear_model import LinearRegression

        # Step 2: Prepare the data
        X = np.array([[1], [2], [3], [4], [5]])  # Independent variable
        y = np.array([2, 4, 6, 8, 10])           # Dependent variable

        # Step 3: Create an instance of LinearRegression
        regressor = LinearRegression()

        # Step 4: Fit the model to the training data
        regressor.fit(X, y)

        # Step 5: Make predictions
        X_test = np.array([[6], [7], [8]])  # Test data for independent variable
        y_pred = regressor.predict(X_test)  # Predict dependent variable

        print(y_pred)  # Print predicted values

### What is the purpose of splitting the dataset into train and test sets, and how does this contribute to the evaluation of a machine learning model’s performance?

      Typically, the dataset is split into a training set (around 70-80% of the data) and a test set (the remaining 20-30%). However, in some cases, additional splits like validation sets or cross-validation may be used for more comprehensive performance evaluation. Splitting the dataset into train and test sets facilitates performance estimation, simulates real-world scenarios, detects overfitting, enables hyperparameter tuning, and allows for the calculation of performance evaluation metrics, all of which are essential for evaluating a machine learning model's performance accurately.

## Things I want to know more about
Data scraping for 'rabbit-hole' datasets like if I wanted to have a Wikipedia search that would keep randomly selecting from keywords I give it