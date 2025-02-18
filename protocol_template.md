# Wednesday, 18.02.2025
<span style="color:grey">
Daily Review : Linear Regression
</span>

---
## <span style="color:black"> __Basic Overview__ </span>
 

* <span style="color:grey"> short bullet points
* <span style="color:grey"> for what you did
* <span style="color:grey"> example: more practice with python

---
##  __Schedule__
<span style="color:grey">

|Time|Content|
|---|---|
|09:00 - 10:00|Daily Review|
|10:00 - 11:30|Lecture|
|11:30 - 12:30|Other theoretical inputs|
|12:30 - 13:30|Lunch Break| 
|13:30 - 15:00|Practical exercises|
|15:00 - 16:00|Exercises and Ending|
|16:00 - 17:00|Stand-up, Exercises and Ending|


## <span style="color:black"> __Who Invented Linear Regression?__ </span>

<span style="color:grey">

* Sir Francis Galton introduced linear regression in the late 19th century.   Sir Francis Galton (1885) introduced the idea of “regression” to the research community in a study examining the relationship between fathers' and sons' heights.
* Karl Pearson and Sir Ronald Fisher, who contributed significantly to its mathematical foundation, later formalized the method. 

</span>

## <span style="color:black"> Motivation for Linear Regression </span>

* Linear regression helps in understanding and quantifying relationships between variables. It is widely used for:
  * Prediction: Forecasting values based on past data - introduction to ML.
  * Explanation: Identifying relationships between variables.
    
---
## <span style="color:black"> __Goals of Linear Regression__ </span>

<span style="color:grey">

* Establish the relationship between dependent and independent variables.  
* The aim is to utilize this relationship for prediction and decision-making.
* Analyze the effect of one or more explanatory variables on an outcome.
* The model assumes linearity, zero-mean error, exogeneity, homoscedasticity, and no multicollinearity.
    * Linearity: The target variable and the coefficients of the explanatory variables are linearly related.
    * Zero-Mean Error: The mean of all residuals is zero.
    * Strict Exogeneity: All the explanatory variables are uncorrelated with the residual.
    * Homoscedasticity: The variance of the residuals across a single observation remains the same.
    * No Multicollinearity: All the explanatory variables are linearly independent.

<span style="color:grey">

---
## <span style="color:black"> __Use Cases in Business Life__ </span>

<span style="color:grey">

* Marketing & Sales: Predicting customer spending based on demographics. 
* Finance: Forecasting stock prices based on historical trends.
* Whenever a linear relationship exists between variables. Surprise surprise!
* Linear regression might be used in domains like economics, medicine, finance, and marketing where there is a data set of variables.
* For predictive modeling :) , trend analysis, and risk assessment.
  
<span style="color:grey">

---
## <span style="color:black"> __Relationship to Statistical Significance__ </span>

<span style="color:grey">

* Linear regression relies on statistical significance to validate relationships. P-values and confidence intervals are used to determine if coefficients are meaningful. 
* Does A/B Testing use Linear Regression?
* A/B tests typically use statistical hypothesis testing (e.g., t-tests). However, linear regression can be used to analyze the effect of multiple factors on the outcome of A/B tests.

<span style="color:grey">

---
## <span style="color:black"> __How?__ </span>

<span style="color:grey">

* Linear Regression model uses training data to establish a general rule for estimation.
* Understand whether an independent variable (X) is associated with a dependent variable (Y) and quantify this relationship.

<span style="color:grey">

---
## <span style="color:black"> Why and When do I Need to Train a Regression Model? </span>

<span style="color:grey">

* To explain the data using a regression model.
* To make predictions based on known inputs. E.g., - Notebook5 - Solution includes 20% of test data to train the model 

<span style="color:grey">

---

## <span style="color:black"> __The Linear Equation__ </span>

<span style="color:grey">

* A simple linear regression model follows this equation: Y = β0 + β1X + ε Where:
* Y = Dependent variable (target)
* X = Independent variable (feature)
* β0 = Intercept
* β1 = Coefficient (slope)
* ε = Error term

<span style="color:grey">

---
## <span style="color:black"> __Types of Linear Regression__ </span>

<span style="color:grey">

* Simple Linear Regression: One independent variable.
* Multiple Linear Regression: More than one independent variable.

<span style="color:grey">

---
## <span style="color:black"> __Least Squares Criterion__ </span>

<span style="color:grey">

To find the best-fitting line, we minimize the sum of squared residuals (SSR):
* SST (Total Sum of Squares) = Total variability in Y.
* SSE (Explained Sum of Squares) = Variability explained by the model.
* SSR (Sum of Squared Residuals) = Remaining unexplained variability.

<span style="color:grey">

---
## <span style="color:black"> __Evaluation Metrics__ </span>

<span style="color:grey">

* Root Mean Squared Error (RMSE): Measures model accuracy.
* Adjusted R²: Adjusts R² for the number of independent variables. 
    * Adjusted R²: will penalize us for adding more features that don't improve our existing model. For a simple linear regression and adjusted will be nearly the same. MSE (Mean Squared Error): SSR divided by sample size.
* R (Correlation Coefficient): Measures relationship strength (-1 to 1).
* R² (Coefficient of Determination): Measures variance explained by the model.

<span style="color:grey">

## <span style="color:black"> __| Summary |__ </span>

<span style="color:grey">

* Linear regression models the relationship between a dependent variable and one or more independent variables.
* We can divide linear regression into two categories:
    * Simple linear regression: cases in which we only have one explanatory variable
    * Multiple linear regression: cases in which we have more than one explanatory variable - multiple linear regression is not so easy to display Linear Regression can approximate a relationship, but it cannot prove causality.
* The model assumes linearity, zero-mean error, exogeneity, homoscedasticity, and no multicollinearity.
    * Linearity: The target variable and the coefficients of the explanatory variables are linearly related.
    * Zero-Mean Error: The mean of all residuals is zero.
    * Strict Exogeneity: All the explanatory variables are uncorrelated with the residual.
    * Homoscedasticity: The variance of the residuals across a single observation remains the same.
    * No Multicollinearity: All the explanatory variables are linearly independent.
* Key evaluation metrics include RMSE, MSE, R², and adjusted R².
* Multiple regression allows for more than one predictor.
* Least squares criterion minimizes prediction errors to find the best fit.


<span style="color:grey">




