# Logistic_Regression
We'll create a model for a telecommunication company, to predict when its customers will leave for a competitor, so that they can take some action to retain the customers.

In this notebook, you will learn Logistic Regression, and then, you'll create a model for a telecommunication company, to predict when its customers will leave for a competitor, so that they can take some action to retain the customers.


# What is different between Linear and Logistic Regression?
While Linear Regression is suited for estimating continuous values (e.g. estimating house price), it is not the best tool for predicting the class of an observed data point. In order to estimate the class of a data point, we need some sort of guidance on what would be the most probable class for that data point. For this, we use Logistic Regression.

<font size = 3>Recall linear regression:</font>

As you know, Linear regression finds a function that relates a continuous dependent variable, y, to some predictors (independent variables x1, x2, etc.). For example, Simple linear regression assumes a function of the form:

                                                 y=θ0+θ1∗x1+θ2∗x2+...
 

and finds the values of parameters θ0, θ1, 𝜃2, etc, where the term 𝜃0 is the "intercept". It can be generally shown as:

                                                   hθ(x)=θTX
 
</div>

Logistic Regression is a variation of Linear Regression, useful when the observed dependent variable, y, is categorical. It produces a formula that predicts the probability of the class label as a function of the independent variables.

Logistic regression fits a special s-shaped curve by taking the linear regression and transforming the numeric estimate into a probability with the following function, which is called sigmoid function 𝜎:

                                 hθ(x)=σ(θTX)=e(θ0+θ1∗x1+θ2∗x2+...)1+e(θ0+θ1∗x1+θ2∗x2+...)
 
Or:
ProbabilityOfaClass1=P(Y=1|X)=σ(θTX)=eθTX1+eθTX
 
In this equation,  θTX
  is the regression result (the sum of the variables weighted by the coefficients), exp is the exponential function and  σ(θTX)
  is the sigmoid or logistic function, also called logistic curve. It is a common "S" shape (sigmoid curve).

So, briefly, Logistic Regression passes the input through the logistic/sigmoid but then treats the result as a probability:

The objective of Logistic Regression algorithm, is to find the best parameters θ, for ℎ_θ(𝑥) = 𝜎({θ^TX}), in such a way that the model best predicts the class of each case.
