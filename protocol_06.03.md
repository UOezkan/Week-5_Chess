# Daily Review | Designing Data Products
<span style="color:grey">
Friday, 07.03.2025
</span>

---
## <span style="color:black"> __Basic Overview__ </span>
 

* <span style="color:grey"> Exploratory analysis - understand what happened in the past
* <span style="color:grey"> Predictive analyis - predict what will happen
* <span style="color:grey"> Predict what, for whom and for what purpose?

---
##  __Schedule__
<span style="color:grey">

|Time|Content|
|---|---|
|09:00 - 10:00|Daily Review|
|10:00 - 12:30|Working on Team Project|
|12:30 - 13:30|Lunch Break| 
|13:30 - 16:00|Working on Team Project|
|16:00 - 16:20|Stand-up|
|16:20 - 18:00|Working on Team Project|

## <span style="color:black"> __Product = Customer x Business x Technology__ </span>

<span style="color:grey">

* Usability
* Business viability
* Feasibility
  
Value = product of the three
  
</span>

## <span style="color:black"> Measuring Success </span>

* The first model you build should be the simplest model that could address the product needs.
* Business performance: measured usually by one KPI (key performance indicator)
* Model performance: an offline metric that captures how well the model will fit the business need


## <span style="color:black"> _Note: The business metric is independent from the model metric... It is a measure of the product success._ </span>

---
## <span style="color:black"> __Examples of Measuring Business Performance__ </span>

<span style="color:grey">

Business metrics:
* Click through rate (CTR) - for recommenders
* Usage - model that generates html from hand drawn diagrams
* Adoption by finance team - internal revenue forecasting

</span>

## <span style="color:black"> Measuring Success </span>

Regression:
* RMSE, RMSLE
* MAPE ( mean absolute percentage error) - accuracy as a ratio

Classification:
* Accuracy
* Precision
* Recall


<span style="color:grey">

---
## <span style="color:black"> __Business Performance vs. Model Performance__ </span>

<span style="color:grey">

![alt text](Business_vs_Model_Performance_4.png)

<span style="color:grey">

---
## <span style="color:black"> __Relationship Between Business Performance & Model Performance__ </span>

<span style="color:grey">

* Thinking of the business value of your model and the cost of being wrong can help you choose the right model metric.
* Always start from the value!
  
<span style="color:grey">

---
## <span style="color:black"> __Error Analysis__ </span>

<span style="color:grey">

Going beyond aggregated metrics
* Most model performance metrics we’ve seen are aggregated metrics
* They help determine whether a model has learned well from a dataset or needs improvement
* Next step: examine results and errors to understand why and how is the model failing or succeeding
* Validation and Iteration
* Note: Performance metrics can be deceptive, on highly imbalanced datasets a classifier can reach very high accuracy without any predictive power

<span style="color:grey">

---
## <span style="color:black"> __Types of supervised learning__ </span>

<span style="color:grey">

![alt text](img_p15.png)

<span style="color:grey">

---
## <span style="color:black"> Validate The Model | Inspect How It Is Performing </span>

<span style="color:grey">

* Regression: looking at residuals, for example doing EDA on residuals and inspecting the outliers
* Classification: one can start with a confusion matrix, breaking results in true class and predictions

<span style="color:grey">

---

## <span style="color:black"> __Confusion Matrix for Classification__ </span>

<span style="color:grey">

Counts how often the model predicted correctly and how often it got confused.
* False Positive: false alarm / type I error
* False Negative: missed detection / type II error



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

## <span style="color:black"> __| - Key Takeaways -|__ </span>

<span style="color:grey">

* Linear regression models the relationship between a dependent variable and one or more independent variables.
* We can divide linear regression into two categories:
    * Simple linear regression: cases in which we only have one explanatory variable
    * Multiple linear regression: cases in which we have more than one explanatory variable - multiple linear regression is not so easy to display
    * Linear regression can approximate a relationship, but it cannot prove causality.
* Linear regression can approximate a relationship, but it cannot prove causality.
* Correlation measures the strength of the relationship
* Regression quantifies the nature of the relationship
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




