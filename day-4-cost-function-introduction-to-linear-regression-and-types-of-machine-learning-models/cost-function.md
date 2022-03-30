# Cost Function

### Learning Objectives

* Statistics Refresher
* Cost Function
* Gradient Descent

### Statistics Refresher

* **Mean:** The mean is the [average ](https://www.statisticshowto.com/arithmetic-mean/)of a data set. For example, take a list of numbers: 10, 20, 40, 10, 70 \
  Mean = (10 + 20 + 40 + 10 + 70) / 5 = 30\

* **Median:** The median is the middle of the set of numbers. To ﬁnd the median, ﬁrst we sort the list of numbers: 10, 10, 20, 40, 70\
  The exact middle number i.e. 20 is the median.\

* **Mode:** The mode is the most common number in a data set.\
  In above list of numbers, 10 has occurred 2 times while other three numbers are occurred one time each.\
  So, the mode is 10 here.\

* **Range:** It is the diﬀerence between highest value and the lowest value in the data set.\
  For a given list of numbers: 10, 20, 40, 10, 70 the range is 70 - 10 = 60.\

* **Variance:** The average of the squared diﬀerences from the mean. Steps to calculate variance:
  * Calculate mean (mean is nothing but average)
  * Find diﬀerence of each data from mean
  * Square all the diﬀerences
  * Take the average of the squares.\

* **Standard Deviation:** It shows you how much your data is spread out around the mean. Its symbol is 𝛔 (the greek letter sigma). **It is the square root of the variance.**

![](https://lh3.googleusercontent.com/jO1jZl2ssSa2dJjSAvtFOXV\_Ect9zg1DcCILj\_ZZp-T1M5IsBf-K3NpFlGzqbtF1DmDB9chwnQai-22xKdSmr0o91sBy0ujxqjg\_CmUNMtNN4AAdb7zWnzIa0Pji5fETc66HxvZdP08)

### Normal Distribution

{% embed url="https://youtu.be/iMak-EW4HtM" %}

{% embed url="https://youtu.be/1EGtm3ClkIc" %}

### Unimodal and Multimodal Distribution

{% embed url="https://youtu.be/7kw9dlAJmA8" %}

### Now coming back to Linear Regression

**This will be in-continuation of our yesterday’s slides!**

### Cost Function

**What?**

Now that we built a model, we need to measure its performance right? and understand if it works well or not. Cost function measures the performance of a Machine Learning model for given data. It quantiﬁes the error between predicted values and expected values and presents it in the form of a single real number.

Depending on the problem Cost Function can be formed in many diﬀerent ways. The purpose of Cost Function is to be either:

* **Minimized** - then returned value is usually called **cost, loss or error.** The goal is to ﬁnd the values of model parameters for which Cost Function return as small number as possible.
* **Maximized** - then the value it yields is named a **reward**. The goal is to ﬁnd values of model parameters for which returned number is as large as possible.
* **Predicted value:** As the name says is the predicted value of your machine learning model.
* **Expected value:** Is the true value(or the label present in your data)

Often machine learning models are not 100% accurate or perfect, they tend to deviate from the true value or expected value.

**Explaining with an example:** If we are predicting the age of a person based on few input variables or features.

* Our machine learning model predicted the age as 28 years
* However, the actual age of the person is 29 years.
* Here **28 years is predicted value** and **29 years is expected value or true value.** As data scientists, we try to minimize the error while building models.

![](https://lh6.googleusercontent.com/Gpw2GaR\_TR1tTmO7RQVEKb1OJ8D\_G01-R3Gz4ldkWCD2VFMAWeCxqjbroN9zW7Q-LFFldp5NBL6QKINUPjxJ572i1yPp24AwjZ7pmIG62fAkqPrgOSLqgN7BZtFOjIC8U1j2Iwbk35Q)

The diﬀerence between the true value and the model’s predicted value is called **residual.**

### Cost Function Types/ Evaluation Metrics

There are three primary metrics used to evaluate linear models (to ﬁnd how well a model is performing):

1. Mean Squared Error:
2. Root Mean Squared Error
3. Mean Absolute Error

* MSE is simply the average of the squared diﬀerence between the true target value and the value predicted by the regression model.
* As it squares the diﬀerences, it **penalizes** (gives some penalty or weight for deviating from the objective) **even a small error** which leads to **over-estimation of how bad the model is.**

![](https://lh3.googleusercontent.com/wQzMvemV6IDaDGpitO9z9hoWw9QvmMjf4Ct-Latgf2Q\_Qxc5s-dA--4csYEMDNloWbacNrvpy6xGpxs73Fs2uJrhIgHVtZqqHwWWsDknedhRx6LfIR2wAjyBs0IKZRbAVpAy45RPnSI)

### Root Mean Squared Error (RMSE)

* It is just the square root of the mean square error.
* It is preferred more in some cases because the errors are ﬁrst squared before averaging which poses a high penalty on large errors. This implies that **RMSE is useful when large errors are undesired.**

![](https://lh5.googleusercontent.com/t6t8RyGZy8b1W8ykd465qJpH-sw\_JKHXmNv0XseU6JrmZ-2GzIT0HMMYkH7k\_y3tSJ4eDBHn2tqNPIdwqZJSFTnFvjQO2A337blZi1gp-DNP17S644aku2dLT7jlj2o59bhzX1cbLx8)

### Mean Absolute Error(MAE)

* MAE is the absolute diﬀerence between the target value and the value predicted by the model.
* MAE **does not penalize the errors as eﬀectively as mse** making it not suitable for use-cases where you want to pay more attention to the outliers.

![](https://lh4.googleusercontent.com/4qrBlv85ARfJ5eadFSfX0MEDgtCzRySrM0c3q3ifZ5NKzOIMSCRXcYNHO7k0Au8Nz1w6jfMaACQ6m3U5IXxRJ8dhEFiUnJXaB6PH4F6zaq385Ff8WkhXH2jJvodPC28zHj9ANksleFY)

### Gradient Descent

* As Data Scientists, we always want to optimise our algorithms and go for the best ones. Gradient Descent is one of those that helps us do this!
* Gradient Descent is an optimization technique in the machine learning process which minimizes the cost function. Every machine learning algorithm has a cost function.
* For now, we are not getting too much into how it works. We will learn about it as we proceed. Below is the link to a video for further understanding: [https://www.youtube.com/watch?v=vsWrXfO3wWw](https://www.youtube.com/watch?v=vsWrXfO3wWw)&#x20;

### Recap

* Linear regression is used to predict a value (like the sale price of a house).
* Given a set of data, ﬁrst try to ﬁt a line to it.
* The cost function tells you how good your line is.
* You can use gradient descent to ﬁnd the best line.

### Optional Reading Material

If you are inquisitive to learn more about gradient descent refer the below video:

* [https://www.youtube.com/watch?v=sDv4f4s2SB8](https://www.youtube.com/watch?v=sDv4f4s2SB8)
