# Module: Input Variables, Target Variable, Train and Test Data Intuition and Building a ML Model

### **Learning Objectives**

* **Input variables, target variable, train and test data intuition and Building a ML Model**

In this module, we will give a quick recap that would help you to solidify the concepts that you learnt so far with some intuitive examples. This will be focused more towards Model Building

### **Building a ML Model (Quick Recap)**

### **Data Science Modelling Process**

![](https://lh4.googleusercontent.com/QBkgygllpsNQ2OJDuOZrRPnp7R6j-O3-x32XYZrl9uSkjdI5T-eIo90FYtoctZZ2gj933oQlTnqD6LggTu2s1TWwjFxI3eEQby\_YYxI4YtwjE\_D-3EDp5lqyD3ngNb6mDkaR3HYA6x0)

**Credits:** [https://towardsdatascience.com/data-science-modeling-process-fa6e8e45bf02](https://towardsdatascience.com/data-science-modeling-process-fa6e8e45bf02)

## Problem Solving steps

* Deﬁne Objective or understand the problem statement
* Data Requirements
* Data Collection/Preparation
* Exploratory Data Analysis
* Data Pre-processing
* Build a model
  * Understand whether it is a regression or classiﬁcation problem
* Evaluate
* Optimise
* Production
* Monitor
* You keep Optimising it every now and then

### Problem Statement

HR department wanted to seek support of analytics team to get possible salary predictions given they have information about employees Career Seniority Level and years of experience.

In other words, they need a machine learning model that would predict the possible salary that one should be provided if they feed information about their seniority level and years of experience.

### **Data Preparation**

* Given that, we have a problem of predicting the salary of a person based on years of experience.
* We have a dataset that looks like:

![](https://lh5.googleusercontent.com/dQzQixg\_qnZvzXOzgWBTrULX6bJXCZ4ajQU3kLdVvZkgsbcQUw0zta2KiCscHcSa0j-a7usR0WU\_VrbJ9NOTsbz3pOpYGavW0YJAqxzSPF\_ABHHZlSTOWDzzh6KDc0YGzkTB64E5Y8k)

* What features do we have here?
* We have 3 features: Seniority\_Level, Years\_of\_Experience and Salary.
* What do you think our target variable(value to be predicted) will be in this case?
* Since Salary needs to be predicted, our model will take that to be the target variable and the rest (Seniority\_Level, Years\_of\_Experience) as input variables.
* In short, we’ll predict the target variable using input variables.

![](<../.gitbook/assets/Screen Shot 2022-04-08 at 7.30.09 PM.png>)

### Separating input and target variable

* Now how do you actually separate the input and target variables?
* Since there’s only one target variable in the DataFrame, we can simply drop it and choose the rest of the variables. We do this using the drop( ) function by simply providing column name inside it.

![](https://lh5.googleusercontent.com/-Uwmlq7kaMKSt3JKnYxwM6sAWlU9G6aUCdR78FJVpqq0vqR8NpV22Dc7VyLKWBJbUZaNj\_i0qjXVN22kMfOTG2f9jnhfvJNOzG\_mslQ49M3RUvoirZ6\_L3oaDeD3jUQ7XBEmw1euME0)

### Train and Test Data

* Another data splitting that we need to do is dividing the data into Train and Test Sets.
* Imagine drawing a horizontal line between the table, let’s say, after the 8th entry. That’s what Train Test Split looks like. The whole table is now divided into 4 parts.
* PLEASE NOTE: The dataset should always be shuﬄed before splitting. We’ve used an unshuﬄed version here just for the explanation purpose.

![](https://lh3.googleusercontent.com/fLGQopk4BraL\_\_-EguWfyok2Z1cvC5lLPU64LYiyJPNHkkzTPpqwqVueGCaVUJIFbXZbPGfcFlipy-6geBZQJv6Po4QeLedQF-Y8iIv6cax0AKdKIAsXGEbs3y34AEZhrbsMizVHUzI)

* The upper part of the table becomes the Train Set which consists of X\_train (The input variables) and y\_train (The output variable).

![](https://lh3.googleusercontent.com/orfClVOWTDaDnm-VVlupUCWzAr63Hc3VbN1XjYnUO6AEU-n6bgdvvKSTMaLxtjbOVjhCr7bglhDiY4PNHoK3Bb5GRO6xxf9CvOf6y9nC\_WIHL-agVwlvRgTxqYK4sY\_bjthBVfS0hy0)

* The lower part of the table becomes the Test Set which consists of X\_test (The input variables) and y\_test (The output variable).

![](https://lh4.googleusercontent.com/mNA0FIvPeWQQ0eZVnO6c9fhd\_Gfec7IxQzF8kDWhz8G1D0-1q7WD5jZxzPAcyPRe2U5jsG95lWwMEntmCmAZRhesw6FqJ3vHWY69quHO9RJDM1XPRsx5ytW4Plv-KhjGG1ca6EG4HRI)

* The sklearn’s function used for splitting the dataset is known as train\_test\_split

![](https://lh4.googleusercontent.com/rsLV\_ITOEKEX3g8JIDcHr2jcSnB\_8AiIS4jct3gQoioXfCXUplnR3fZeIhGSgtwN-OiCMJkPK8pjnTQnwyPa5oXuOYpK\_-ECdQ0\_PfuNdL6ST0CGjr0s3w9z1BD4AAGHztVkec\_lyOQ)

* The 4 variables that we learned about in the previous slides are assigned values using the above piece of code. Let’s understand what the values inside the brackets mean:
  * **X** = Input variables
  * **y** = Target variable
  * **test\_size** = The ratio of the dataset that’ll be used in test set. If there are 100 rows, 70 rows will be used in train set and 30 in test set.
  * **random\_state** = It is provided just for the sake of obtaining the same result every time we run the code. It ensures that the rows in train and test set remain same each time.

### Model Building

Let’s build the simplest of all regression models using Linear Regression now.

* Import the model from sklearn
* Initialise and store the model in a variable (linear\_regressor in this case)
* Train the model on Train Data(X\_train and y\_train) using the ﬁt method.

![](https://lh6.googleusercontent.com/aqpbpFwrV329dqdBjQk8llpi3TSva6nmQzi1C-SqLrm\_5S6G-1j4FikxQBAdkiApSOkC1-bcELul3Dt0miiWOYC5-\_kX\_QUo5HG3SWW\_gYGrIL9-6Ob3DoZw3xQkxlveznxET9C-E10)

### Understanding the type of Problem

* For understanding the type of problem, we need to see the target variable we are dealing with.
* What kind of variable is Salary? Does it have classes? No, right?
* Salary is numerical and diﬀerent salaries are not divided into classes but are rather continuous values.
* The technique used for determining relationship between the input and target variables where the target variable is numerical (or continuous) is known as **Regression.**

### Model Evaluation

* Our model has been created! But how do we know if it works well? By testing it on the Test Data we created.
* Remember the test data is also split into 2 parts - X\_test and y\_test?
* We’ll ﬁrst put the X\_test(input variables) in our model and see what Salary predicts for those input values. The actual values of the salaries(y\_test) are not shown to the model.

![](https://lh5.googleusercontent.com/Vo3cI-d91tFfggmjzx59q23V2gnuXkFq39eQpXoM6EDoYreuFcpT\_K6xCSOsYHxjAz4nILYCYnoK5UTMgMTbQmyBQ0gPT2lXqO3SdUApSqVSRaZ0OJygUoGyqYf\_cKhPmpoXly5I\_xk)

* Let’s say our model predicts the following salaries:

![](https://lh3.googleusercontent.com/SPOJqMltbDoNnu0MJySvZKc3yKc4FeCQDqRUoPC9UrcVozpVjntuX3NCU\_n46F5Q0MYkZmAYFVDrlYX\_oropq1C9ly6Yn\_eUAWLk8k\_ACx-2KsVUrMLTthCj3ZYxAOU9JcoB\_nPdmNM)

* This prediction is done using the predict function of sklearn. Inside the predict function, we’ll provide X\_test to the model.

![](https://lh4.googleusercontent.com/Bz-\_5ecO5hivCX6aYxDvQpF7pVSAK0rzdEC7EPyANt8bKwEXDfLybwmum0xYG-UHE-cde5iguqXPC-zuZSCsqoNk\_SuF8bHL\_lFHa9gFVYATdH4EG72Epgln6Rj5mTJtG5DBrfXcrLE)

* To know how good these predictions (y\_pred) are, we’ll have to compare them to the actual salary values (y\_test).

**ACTUAL VALUES                                 PREDICTED VALUES**

![](https://lh6.googleusercontent.com/jg0mEgt6EWVD4b-jgtip\_eyGeHKVhVr\_0wpN2hKS7MNPylIZeQV77opnWyy-QhZ\_eksRQWovvqYYpnfWaBub5dEQKAoorgKOsx5\_8CGy-ZI-IT-xYQpyv8Qw\_\_zC3nrtiK4G5h5QN-w)                                       ****                                       ![](https://lh3.googleusercontent.com/SPOJqMltbDoNnu0MJySvZKc3yKc4FeCQDqRUoPC9UrcVozpVjntuX3NCU\_n46F5Q0MYkZmAYFVDrlYX\_oropq1C9ly6Yn\_eUAWLk8k\_ACx-2KsVUrMLTthCj3ZYxAOU9JcoB\_nPdmNM)

* There are a lot of evaluation metrics for regression problems. Let’s use Root Mean Squared Error for this case.

### Root Mean Squared Error (RMSE)

* It is just the square root of the mean square error.
* It is preferred more in some cases because the errors are ﬁrst squared before averaging which poses a high penalty on large errors. This implies that **RMSE is useful when large errors are undesired.**

![](https://lh3.googleusercontent.com/wR6LQRmLfdGUCCGkrOy7yd9Tj-81da1TkHqqSNuZwqyZgphTK77ZRmLfjbc1gO9m4A16LKzbMuoXlaSrEkogpMUzyKNkinvnpPS097j0GU4VXpjGIyjPuXm7q3PN1Da5OhUU4WGxCq0)

* For using RMSE, we’ll ﬁrst import metrics library from sklearn.

![](https://lh3.googleusercontent.com/EHHVQYW24GY7ob6IqWyImzKZ1Jjjm79d3u8EstkvmcMNWMQZyVjHyZ5YmkiOi-4eOOG2TztJqAwrDEypWjZU27hpy\_1BS34AvVSHLzwgoz6tCRBfZWlQZwgUePpBBMw5B8y0jnOMlf8)

* RMSE is not present as a function in sklearn. So we’ll just use the mean\_squared\_error function and take its square root . The main thing to note is what we provide inside the function - y\_test (actual value) and y\_pred(predictions made by our model).

![](https://lh4.googleusercontent.com/Gw256hWo-6hViV6SWg9vr\_6\_ZAE8YZs3M3mlUxVhWCeSlIOWtvj1kWj9eUXF3ljG8SYJyPpuDwU-uCQ9BMa1T\_xiAc3GR9g\_kMCeUnzRlhD0c9V\_ZZu33mzpod2WfAwOgOHBSBkdLVA)

### Video Tutorial

{% embed url="https://www.youtube.com/watch?t=1s&v=y_SdBb2_Hiw" %}

### Transformations on Train and Test

* Now let’s say we performed some feature selection techniques and found out that Seniority\_Level is not an important feature, the model can perform better when only Years\_of\_Experience is used.
* We’ll then transform our train data to a dataset with only Years\_of\_Experience as input variable to predict our target variable Salary.
* Now what about test data? Should we remove the Seniority\_Level feature from that as well?
* The answer is yes.
* The **Train and Test data must undergo the same data preparation steps**. Otherwise, the predictive model will not make sense. This means that the number of features for both the training and test set should be the same and represent the same thing.
* Similarly, **if normalization is required, then it should be done on both the train and test sets.**
