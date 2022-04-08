# Day 2: Regression Algorithms & It's Evaluation Metrics

* **Difference between Classiﬁcation and Regression**
* **Regression Algorithms & Model Evaluation Metrics**
* **Which evaluation metrics to use when?**

### **Disclaimer**

* We haven’t taught all the algorithms as the Bootcamp was of 5 weeks and we wanted learners to have a good grasp on the concepts that are being taught and not overwhelm them with all the concepts available. Once you know how to handle data and build models, you can easily build diﬀerent kinds of models.
* Through this module, we’ll be providing material around some of the popular algorithms. In addition, we will sharing some more resources soon.

### Classification vs Regression

![](https://lh5.googleusercontent.com/B9PD8h6-NmNF5hZ1KRbCi8hXvH8bgxeXHTZU7JZDXO54Vx0qVFEoat5\_jp5dtac50mEfS\_5ZmG3iNnDgeYvklGaS1MsC1eMpIZdgMXy6unXLhZpK6tdRP1-nHuIijXNADmy5pHqVEiQ)

* In order to decide whether to use a regression or classiﬁcation model, the ﬁrst questions you should ask yourself is:
* Does your target variable have a continuous value or is it discrete (binary or multi-class)?

### Regression

* If your answer is continuous values, you’re dealing with Regression.
* This means that if you’re trying to predict quantities like height, income, price, or scores, you should be using a model that will output a continuous number.
* So if your objective is to determine tomorrow’s temperature (or let’s stock price tomorrow), you should use a regression model.

### Classification

* Let’s come to the second case where if you can clearly see that the target variable is divided into classes. You’ll be using Classiﬁcation here.
* When the number of classes is 2, it is known as Binary Classiﬁcation.
* Eg. Will it be hot or cold tomorrow is a binary classiﬁcation problem with 2 classes: Hot and Cold.
* When it is more than 2, it is known as Multi Class Classiﬁcation.
* Eg. Classifying movies in Good, Average or Bad according to reviews.

### Classification vs Regression

![](https://lh5.googleusercontent.com/j6pG3ncKELiId7pNVXZ306Jz5etQu1fzpNbf5R8Vx5T-P-GkLXoZlFxZ2mPcsKudDI\_bfnC2qAoMmCMcn2zA-\_66Z01wQZMbi2Laq4uwMJyWjDTWDRFv6cdIkImE4gnP4OoU74X0\_f0)

* It’s important to understand the characteristics of your target variable before you begin running models and forming predictions.

### Types of Regression Algorithms

1. Linear Regression
2. Decision Trees (DecisionTreeRegressor)
3. Random Forest (RandomForestRegressor)
4. Other Algorithms
   1. Polynomial Regression
   2. Lasso, Ridge and Elastic Net Regression
   3. Support Vector Regressor
   4. And many more….

### Linear Regression

* Linear regression is a linear model i.e. a model that assumes a linear relationship (straight-line relationship) between the input variables (x) and the single output variable (y). Below are some useful resources that would help you with Linear Regression
  * **Linear Regression Module:** [https://docs.google.com/presentation/d/1Vhgfhjc3Ye90wjgy\_R](https://docs.google.com/presentation/d/1Vhgfhjc3Ye90wjgy\_RPt-G2ModxN1O9EI4kfOa2SS0M/edit#slide%3Did.p1) [Pt-G2ModxN1O9EI4kfOa2SS0M/edit#slide=id.p1](https://docs.google.com/presentation/d/1Vhgfhjc3Ye90wjgy\_RPt-G2ModxN1O9EI4kfOa2SS0M/edit#slide%3Did.p1)
  * **Beginners guide to Linear Regression in Python:** [https://dphi.tech/a-beginners-guide-to-linear-regression-in-pyt](https://dphi.tech/a-beginners-guide-to-linear-regression-in-python-with-scikit-learn/) [hon-with-scikit-learn/](https://dphi.tech/a-beginners-guide-to-linear-regression-in-python-with-scikit-learn/)
  * **Simple linear Regression implementation in sklearn:** [https://www.youtube.com/watch?v=b0L47BeklTE](https://www.youtube.com/watch?v=b0L47BeklTE)

### Decision Trees for Regression -Regression Trees

{% embed url="https://www.youtube.com/watch?t=1s&v=g9c66TUylZ4" %}

### Decision Trees

* Regression tree analysis is used when the predicted outcome can be considered a real number (e.g. the price of a house, or a patient's length of stay in a hospital).
* **Note:** Something that we didn’t address earlier, Decision Trees are called as Classiﬁcation And Regression Trees (CART).
* **Reason:** They can be used in both a regression and a classiﬁcation context. For this reason they are sometimes also referred to as Classiﬁcation And Regression Trees (CART).
* **Module on Decision Trees:** [https://docs.google.com/presentation/d/1BCwLdFQqFLHR2-7APyo](https://docs.google.com/presentation/d/1BCwLdFQqFLHR2-7APyoWh5u1b6Jo3wq17nj-8s2H\_mg/edit#slide%3Did.p1) [Wh5u1b6Jo3wq17nj-8s2H\_mg/edit#slide=id.p1](https://docs.google.com/presentation/d/1BCwLdFQqFLHR2-7APyoWh5u1b6Jo3wq17nj-8s2H\_mg/edit#slide%3Did.p1)

### Resources on Decision Tree Regressor

* **Implementation of Decision Tree Regression:** [https://heartbeat.fritz.ai/implementing-regression-using-a-deci](https://heartbeat.fritz.ai/implementing-regression-using-a-decision-tree-and-scikit-learn-ac98552b43d7) [sion-tree-and-scikit-learn-ac98552b43d7](https://heartbeat.fritz.ai/implementing-regression-using-a-decision-tree-and-scikit-learn-ac98552b43d7)

### Random Forest for regression - Regression Forest

* Random forest builds multiple decision trees and merges them together to get a more accurate and stable prediction.
* Regression Forests (or Random forest Regressors) are an ensemble (combination) of diﬀerent regression trees (decision trees for regression). Each leaf contains a distribution for the continuous output variable/s.

![](https://lh5.googleusercontent.com/V4XB8sUzYznlzOEXZp1LOrPBEiUb8eXLEO3EFtkHuaTICvwhHdXqChyZYJwkgamMZBghbm5tUsC50ShCAZLWwT2ZefOTbTrua3diBLrf59oLQ3iw5wpNneV15AV67\_0cUuU-xeaSbXI)

### Other Regression Algorithms

* **POLYNOMIAL REGRESSION:**

Polynomial Regression is a form of linear regression in which the relationship between the independent variable X and dependent variable y is not linear (cannot be represented by a straight line).

![](https://lh5.googleusercontent.com/jy457xgx14y7I\_J7JxuAUVNGYJDdAx2iWNhrBof4tHlLxhNsyljDvVIVxt-ZgneD3o5MhX0jgn5kAGivwQx4jvBOMFCcwZsa0yYwxqH4CINCMCBwmBSah5B\_X5KvufUxj5HwrWm5cjo)

Which of the following do you think is a better ﬁtted line for the green data points?

The second one. The only diﬀerence is that instead of using the equation of a straight line, we are using a diﬀerent equation of higher order polynomial.

Learn more about Polynomial Regression: [https://towardsdatascience.com/polynomial-regression-bbe8b9d97491](https://towardsdatascience.com/polynomial-regression-bbe8b9d97491)

* **LASSO, RIDGE AND ELASTIC NET REGRESSION:**

There are extensions of the linear regression model training called as **regularization methods**. They aim to minimize the error, while keeping the complexity of the model low.

Two popular examples of regularization procedures for linear regression are:

1. **Lasso Regression** (called **L1 regularization**).
2. **Ridge Regression:** (called **L2 regularization**).

These methods are eﬀective to use when there is collinearity in your input variables and there’s a chance of overﬁtting the training data.

There is another commonly used model of regression called **Elastic Net**. It **incorporates penalties from both L1 and L2 regularization**.

You can read more about Lasso, Ridge and Elastic Net Regression here:

[https://hackernoon.com/an-introduction-to-ridge-lasso-and-elastic-ne](https://hackernoon.com/an-introduction-to-ridge-lasso-and-elastic-net-regression-cca60b4b934f) [t-regression-cca60b4b934f](https://hackernoon.com/an-introduction-to-ridge-lasso-and-elastic-net-regression-cca60b4b934f)

* **SUPPORT VECTOR REGRESSOR (SVR)**

Support Vector Machines (SVMs) are well known in classiﬁcation problems. However, the use of SVMs in regression is not as well documented. These types of models are known as Support Vector Regression (SVR).

SVR **gives us the ﬂexibility to deﬁne how much error is acceptable** in our model and will ﬁnd an appropriate line to ﬁt the data.

SVR Tutorial:

[https://www.analyticsvidhya.com/blog/2020/03/support-vector-regression-tut](https://www.analyticsvidhya.com/blog/2020/03/support-vector-regression-tutorial-for-machine-learning/) [orial-for-machine-learning/](https://www.analyticsvidhya.com/blog/2020/03/support-vector-regression-tutorial-for-machine-learning/)

### MUST READ - Regression Algorithms and their applications:

* [https://analyticsindiamag.com/top-6-regression-algorithm](https://analyticsindiamag.com/top-6-regression-algorithms-used-data-mining-applications-industry/#%3A\~%3Atext%3DToday%2C%20regression%20models%20have%20many%2Classo%20regression%20and%20multivariate%20regression) [s-used-data-mining-applications-industry/#:\~:text=Today%](https://analyticsindiamag.com/top-6-regression-algorithms-used-data-mining-applications-industry/#%3A\~%3Atext%3DToday%2C%20regression%20models%20have%20many%2Classo%20regression%20and%20multivariate%20regression) [2C%20regression%20models%20have%20many,lasso%20r](https://analyticsindiamag.com/top-6-regression-algorithms-used-data-mining-applications-industry/#%3A\~%3Atext%3DToday%2C%20regression%20models%20have%20many%2Classo%20regression%20and%20multivariate%20regression) [egression%20and%20multivariate%20regression](https://analyticsindiamag.com/top-6-regression-algorithms-used-data-mining-applications-industry/#%3A\~%3Atext%3DToday%2C%20regression%20models%20have%20many%2Classo%20regression%20and%20multivariate%20regression).
* [https://www.analyticsvidhya.com/blog/2015/08/comprehe](https://www.analyticsvidhya.com/blog/2015/08/comprehensive-guide-regression/) [nsive-guide-regression](https://www.analyticsvidhya.com/blog/2015/08/comprehensive-guide-regression/)

### Regression Model Evaluation

1. Cost function
2. What is predicted and expected/true value?
3.  Evaluation Metrics

    1. RMSE
    2. MAE
    3. MSE



### Cost Function

**What?**

* Now that we built a model, we need to measure its performance right? and understand if it works well or not. Cost function measures the performance of a Machine Learning model for given data. It quantiﬁes the error between predicted values and expected values and presents it in the form of a single real number.
* Depending on the problem Cost Function can be formed in many diﬀerent ways. The purpose of this function is to be either:
* **Minimized** - then returned value is usually called **cost, loss or error.** The goal is to ﬁnd the values of model parameters for which Cost Function return as small number as possible.
* **Maximized** - then the value it yields is named a **reward**. The goal is to ﬁnd values of model parameters for which returned number is as large as possible.

### What is predicted and expected value?

* **Predicted value:** As the name says is the predicted value of your machine learning model.
* **Expected/Actual value:** Is the true value(or the label present in your data)
* Often machine learning models are not 100% accurate or perfect, then tend to deviate from the true value or expected value.
* **Explaining with an example:** If we are predicting the age of a person based on few input variables or features.
* Our machine learning model predicted the age as 28 years
* However, the actual age of the person is 29 years.
* Here **28 years is predicted value** and **29 years is expected value or true value.** As data scientists, we try to minimize the error while building models.

### Cost Function

![](https://lh4.googleusercontent.com/FEhy2bKK3axpdfj2d0YAourphmgCE6Oc4rSz9mIOL-pTfynBNbiqquJPMjV5VLACrzUBBJEsipOg1nq2LfIfM\_WFn6maRXXClQtDDkxEFeltKmRit-8c52OyjbcyDNl7ghahhFM4\_Kc)

* The diﬀerence between the true value and the model’s predicted value is called **residual.**

### **Cost Function Types / Evaluation Metrics**

* There are three primary metrics used to evaluate linear models (to ﬁnd how well a model is performing):
  * Mean Squared Error:
  * Root Mean Squared Error
  * Mean Absolute Error

### Mean Squared Error ( MSE )

* MSE is simply the average of the squared diﬀerence between the true target value and the value predicted by the regression model.
* As it squares the diﬀerences, it **penalizes** (gives some penalty or weight for deviating from the objective) **even a small error** which leads to **over-estimation of how bad the model is.**

![](https://lh4.googleusercontent.com/zUD5J9b0rHyGJXtmVNs\_HqRn-EVDLG87kSdV97oO6m3csUlZAh3ikGtY7O5X2APzx2B4RuIk24vMAQBU0lWb2FhcI7-pix685SlxkCeoqyj2bh\_r01FXvSBeankxta7IpwuUUIUimb0)

### Root Mean Squared Error (RMSE)

* It is just the square root of the mean square error.
* It is preferred more in some cases because the errors are ﬁrst squared before averaging which poses a high penalty on large errors. This implies that **RMSE is useful when large errors are undesired.**

![](https://lh6.googleusercontent.com/MWOnWy6VxzdWlun40AvytGT6k8HhFLuvAR9WKtvI6UcVX4kfFTl3y3GjUWmNS9d-qEmHovWZghvCvEEhaqIhALWZtJTT-s3VXDKgRNdQuPvXcLRJSCdZ1zNpWlvRIfy3cIcbVI7nKSs)

### Mean Absolute Error(MAE)

* MAE is the absolute diﬀerence between the target value and the value predicted by the model.
* MAE **does not penalize the errors as eﬀectively as mse** making it not suitable for use-cases where you want to pay more attention to the outliers.

![](https://lh4.googleusercontent.com/M2Q\_SDYSxsIJlfrvlo1JsBXC0R9sYs7paFJJFaRfLvz2RhBtLXnzAn3n-4bIUQnOkpLyb-p3\_PjlJGc2OYLOHAnG8l\_e7L61BuYUO57Dg8qj1RbDB3jPoEvj0d5Ms6f30z-mHURUy-o)

### R Squared ( Coefficient of determination)

{% embed url="https://www.youtube.com/watch?t=3s&v=-fgYp74SNtk" %}

* R-squared is a goodness-of-ﬁt measure for linear regression models.
* It represents the coeﬃcient of **how well the values ﬁt compared to the original values**. The values from 0 to 1 are interpreted as percentages.
* The higher the value is, the better the model is.
* Going by the name, you might think R2 cannot be negative. However, it can. A Negative R2 means you are doing worse than the mean value.

### **Which metrics to use when?**

This is an important question and we get used to learning these measures over time. Sharing some resources with you all so that it helps you understand what metrics to be used in the context of solving a regression problem.

* [https://medium.com/usf-msds/choosing-the-right-metric-for-](https://medium.com/usf-msds/choosing-the-right-metric-for-machine-learning-models-part-1-a99d7d7414e4) [machine-learning-models-part-1-a99d7d7414e4](https://medium.com/usf-msds/choosing-the-right-metric-for-machine-learning-models-part-1-a99d7d7414e4)

(you may ignore “Bonus” section in the article for time being)
