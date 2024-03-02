# Mutinominal-Losigtic-Regression

## 3 Types of Logistic Regression Model
- In a nutshell, a logistic model relates the probability that a target category will occur as a linear function of the predictors

<img width="503" alt="Screenshot 2024-03-02 at 3 50 14 PM" src="https://github.com/ColleenJung/Mutinominal-Losigtic-Regression/assets/119357849/db6fda28-259a-4655-b4c3-081980429d9e">

## Odds vs Probability

<img width="536" alt="Screenshot 2024-03-02 at 3 58 14 PM" src="https://github.com/ColleenJung/Mutinominal-Losigtic-Regression/assets/119357849/b15be811-c45d-4328-a123-695cc1e550af">

- The log-scale chart on the right suggests that the logarithm of Odds is approximately linear in the probability within a certain range (e.g., between 0.2 and 0.8) of probability.

## Multinomial Logistic Regression
-  Multinomial Logistic Regression is an extension of binary logistic regression(yes/no, success/failure)
-  Multinomial Logistic Regression deals with outcomes having three or more categories.(sunny/cloudy/rainy)


## Python Library: StatsModels- The MNLogit Function
- It trains a multinomial logistic model.
- By default, it arranges the target categories in ascending lexical order.
- It takes the FIRST target category as the reference category.
- It does neither detect nor handle aliased parameters.  Therefore, we need to manually find the aliased parameters, and not pass them to the function.

## Terminology for a Statistical Model
- Degrees of Freedom of a Model: The number of non-aliased parameters excluding the Intercept term, if specified
- Degrees of Freedom of Residuals: The number of observations minus the number of non-aliased parameters (including the Intercept term)
- Log-Likelihood of a Model: The log-likelihood of the current model
- Log-Likelihood of a Null Model: The log-likelihood of a model that only has the Intercept term
- Log-Likelihood p-Value: The p-value from performing a Chi-Square statistical test that compares the current model from the Null model

## Feature Selection(Select Predictors into Model)

<img width="531" alt="Screenshot 2024-03-02 at 4 07 31 PM" src="https://github.com/ColleenJung/Mutinominal-Losigtic-Regression/assets/119357849/1ded7377-27ed-4ca5-9f92-7b071a6a21b4">

## Less Noise is Better Quality 
**- Can we improve the prediction accuracy? Without Re-selecting Features?**
- A common tactic to raise up the signal-to-noise balance is to **assign values of interval predictors into bins.**
- To put it another way, **we will gain accuracy by sacrificing data details.**

## Assign Values of Interval Predictors into Bins!

- Quintiles of Interval Predictors

<img width="404" alt="Screenshot 2024-03-02 at 4 14 55 PM" src="https://github.com/ColleenJung/Mutinominal-Losigtic-Regression/assets/119357849/22ac77ed-b686-4810-baa7-996337ef87cd">

- Champion Versus Challenger Model

<img width="495" alt="Screenshot 2024-03-02 at 4 15 28 PM" src="https://github.com/ColleenJung/Mutinominal-Losigtic-Regression/assets/119357849/1582f2fe-306e-4a9f-b0eb-a2d61aad9162">

<img width="552" alt="Screenshot 2024-03-02 at 4 15 48 PM" src="https://github.com/ColleenJung/Mutinominal-Losigtic-Regression/assets/119357849/3b6e67ee-9516-498c-b460-488341515627">

