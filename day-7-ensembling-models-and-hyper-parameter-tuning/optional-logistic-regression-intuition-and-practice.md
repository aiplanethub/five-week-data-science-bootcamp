# (Optional): Logistic Regression Intuition and Practice

### Learning Objectives

* Data Splitting Recap
* Logistic Regression

### **Quick recap of some keywords! Back to basics ;)**

* **Features or Variables:** These are the the most common terms that we would come across from now on.
* **Features and Variables both are the same in a dataset**, they are often interchangeably used. So there is no need to worry about it!

![](https://lh5.googleusercontent.com/NfjBXMquDNhi3ubaDrVz3ysDM1xAoya9gAoBAdOdpJQqsebDQRj0In8zXmHzGBtjvPis9PqD70r0RpFYs6CzWU5ounWIa7xsWKa1qoYR4Yq-aLRfBH3CSQObCfTYnstk2dtS-8DzfkU)

* Remember the Standard Metropolitan Areas Data used in previous slides? In that dataset **we might be curious to predict “crime\_rate” in future**, so that becomes our target variable and rest of the variables become input variables for building a machine learning model.

![](https://lh4.googleusercontent.com/UBvcA3yM2AO5Tmr1Gbyagm14XJs0YE01r1BPbISLCT0DrPe1zAC0yPQMTPRgfMzJJDpyICYqlqRVZn5rBGQGpBTOQqOr-mcgU2qF4M1ZU-Av-EHB7vIvRnjMgka14Z6vUBDfndfsaio)

### Train and Test Set

![](<../.gitbook/assets/image (4).png>)

### Data Splitting

1. We **separate the data into input and target variable**
2. We further **divide them into train and test datasets**

![](https://lh6.googleusercontent.com/bSmPKkh4F5GaD5-F9FLVQ-8xlM3yw5OqFpZYDZ-Zm8GOY9hKDMIk\_n4U8pPSW1Y72LuzCwxmMvMToj8QPcsSPBfWCTkWgRw7Xh2QyBon76QDffWBohUd8wImVGIgmyaVi2MOnmX4MOE)

* Let’s consider the following data with 10 entries and our objective is to predict whether someone has purchased a product or not i.e “ProductPurchase” column = Yes or No

![](https://lh3.googleusercontent.com/mMnd6S0q00pSTgHfxnchZiYb\_xspi4yhnJX6SH6\_UpgBlAZg-9fZavICbq6wrCqKQMCNCdMGkPLmgz5PGvNBRtDMg6q9RLNXwlZlJ0y0MG4JAZbbWGKQC0VFxTB\_CqbRQMBN-6qK9Yk)

Here, **Country, Age and Salary are the Input variables** used to predict the **target variable - ProductPurchase**.

### Separate Input and Target Variables

* We separate the dataset into two new datasets one with input variables - X (Country, Age and Salary) and the other with target variable - y (ProductPurchase).
* Adding a snippet from that we used in [our ﬁrst model building](https://github.com/dphi-official/First\_ML\_Model/blob/master/ML\_with\_titanic\_data.ipynb) [exercise](https://github.com/dphi-official/First\_ML\_Model/blob/master/ML\_with\_titanic\_data.ipynb).

![](https://lh4.googleusercontent.com/opbbmGXwyAEw5g3P2X27TJd6ZVdLs9SWz8wxtGjyHPufuO501irJDj0H29wqyt3XTig6i9Uvl7X71hynhL34twy99NC9aF0MSCx-dcMKKQk6x5bSEyyNAUj9IMRE7xjYYc1UJe80Vgo)

* We’ll now split the x dataset into two separate sets — X\_train and X\_test.
* Similarly, we’ll split the dataset y into two sets as well — y\_train and y\_test.

![](https://lh6.googleusercontent.com/XhI6oPBnc9IkVRPtEcgXtFsokfE5CTPGNci4lW\_v4jnZSAUYOYbRqzpo2Q8B\_YRCqnrHcCQTgwpozW4L3tHoZaxxoz8UKorQguRErDr4jofkNgE9JkoTYWEBpe4fyWKR6PDX4\_zLWVY)

* Reference here: [https://dphi.tech/notebooks/858/manish\_kc\_06/day-1-notebooks-m](https://dphi.tech/notebooks/858/manish\_kc\_06/day-1-notebooks-ml-with-titanic-dataset) [l-with-titanic-dataset](https://dphi.tech/notebooks/858/manish\_kc\_06/day-1-notebooks-ml-with-titanic-dataset)

### **Logistic Regression!**

* Thing to note! Never jump the gun!

![](https://lh5.googleusercontent.com/Iz2JCmJmgeAo4RMgXH9IiJOp7ZoTYZ45fnR9QcUM6c8o0mfYSJ6yDYYIRlmvd2FId38Ny2YzofdCRV-QUMllfk83YGAYXd5EU8LO3jx4gkf3Il8eeStzejbHhfLgXksDpFG9NxSUKj0)

* We can take baby steps and learnt things over time!

![](https://lh3.googleusercontent.com/ZfrE7irI\_qSCrMQX1NKy3t93k2TGxxLkd1aoR9sk64yumWyspXtVXubIXykI9z2LeujDFLAJe8T2FtnKRT8i\_5raB4g68i0H-oEDJOH3057XIlopFnrWQzQFW9FcNG9ZfuUyQPJ3cxY)

### What’s next?

* We learnt to build our ﬁrst machine learning and also learnt about the 2 other ML models (Linear and Logistic Regression). This means we are already in the game and we know how to build models.
* Ofcourse, there will be ifs and buts, we might be confused because of too many terminologies, many models etc. That is totally common!
* Now, let's take some baby steps to understand Logistic Regression. We learn the intuition behind the algorithm ﬁrst and once we understand it well, we ourselves would be curious to learn the maths behind overtime.

**Please note:** Getting overwhelmed with maths or coding or tools shouldn’t be a blocker to learn data science!

### What is Classification?

Let’s learn with some examples:

* In **Classiﬁcation we** classify the outcome
* **Examples:**
  * Predict whether a transaction is fraud or not fraud
  * Predict whether to give loan or not
  * Predict whether to give college admission or not
  * Predict the grade (Grade A, B, C, D)
  * Note: Classiﬁcation can be more than two

![](https://lh4.googleusercontent.com/odoUcn2-bFiTvLe2fiT-WWPM8SENJtVNLoPYf7V5pJVLZBWq4IL-BZDj2GWJmmMZ1D9GGKZD3Cp9HkYiITUN691MBEGl4-k37oMiCJZhPuruLaAbZyPqiamq09uOukdFh8eQeY8Uk3c)

### Logistic Regression

* Logistic Regression is one of the basic and popular algorithms to solve a binary classification problems
* For each input, logistic regression outputs a probability that this input belongs to one of the 2 classes
  * Set a probability threshold boundary and that determines which class the input belongs to
* Binary classification problems (2 classes):
  * Emails (Spam / Not Spam)
  * Credit Card Transactions (Fraudulent / Not Fraudulent)
  * Loan Default (Yes / No)
* Now, you may ask why don’t we use Linear Regression? Why do we need a new algorithm?
* Well, you would ﬁnd all the answers in the video in the next slides.
* The video below is a must watch, the instructor has brilliantly explained about logistic regression!

### **Must Watch:** Understanding Logistic Regression

{% embed url="https://youtu.be/zM4VZR0px8E" %}

### Linear Regression vs Logistic

* Linear regression is used to solve regression problems with continuous values
* Logistic regression is used to solve classification problems with discrete categories
  * Binary classification (Classes 0 and 1)
  * Examples: Emails (Spam / Not Spam), Credit Card Transactions (Fraudulent / Not Fraudulent), Loan Default (Yes / No)
* Let’s say a data scientist named John want to predict that whether a customer will buy insurance or not
* Remember that linear regression is used to predict a continuous value where the output (y) may vary between +∞ (positive infinity) to -∞ (negative infinity) whereas in this case, the target variable (y) takes only two discrete values, 0 (No insurance) and 1 (Yes, got the insurance).
* John’s decides to extend the concepts of linear regression to fulfil his requirement. One approach is to take the output of linear regression and map it between 0 and 1, if the resultant output is below a certain threshold (say 0.5), classify it as No (didn’t buy the insurance) whereas if the resultant output is above a certain threshold, classify it as bought the insurance (yes)
* We then plot a simple linear regression line and set the threshold as 0.5
  * Negative class (Insurance = No)– Age on the left side
  * Positive class (Insurance = Yes) – Age on the right side

![](https://lh3.googleusercontent.com/vYIl0NDOqZzhhZllBYoqczhwUQoml6Asopkz1wNVN4Q83SD36WWyV3JTxGDWai0ouqEIuotunUoPFlZ4AsFkcqoU8gsIngKuIYQBNQB1YAq9x5\_17EtgbVbRW8tx33mcfj9lkv\_jUxY)

**Imagine there is an outlier to towards right**

![](<../.gitbook/assets/image (6).png>)

* As we can see outlier in the data and will distort the whole linear regression line.
* Clearly the line is unable to diﬀerentiate the classes with the linear line fit
* The line should have been at the vertical yellow line which is able to divide the positive and negative classes i.e yes or no for insurance

**Well, life would be much simpler if we had a algorithm that would fit the points like below right? It is a much better fit compared to regression line!**

![](https://lh4.googleusercontent.com/jsJ1nwL1kXcg9t5zXp-1cvk0OoV\_sr0m2TEcKjXr7ZRoW1Y-nvGjXicyFBUkgPUxZNDeQw2POZYVsX3uC0Qn0FqxA77m6EsXOvpFW80JYCEMdwzZHlP-uytGpB3SIVvycB8lmgE7fLg)

### Solution

* Solution – Transform linear regression to a logistic regression curve
* Logistic regression is a Sigmoid function
* Now what does this sigmoid function do?
  * Sigmoid function takes in any real value and gives a output probability between 0 and 1

![](https://lh4.googleusercontent.com/jsJ1nwL1kXcg9t5zXp-1cvk0OoV\_sr0m2TEcKjXr7ZRoW1Y-nvGjXicyFBUkgPUxZNDeQw2POZYVsX3uC0Qn0FqxA77m6EsXOvpFW80JYCEMdwzZHlP-uytGpB3SIVvycB8lmgE7fLg)

### What are we doing in Logistic Regression?

* We will use the real-valued output obtained from a linear regression model between 0 and 1 and classify a new example based on a threshold value. The function used to perform this mapping is the **sigmoid function**
* The Sigmoid Function is represented by the formula:

![](https://lh3.googleusercontent.com/EHmrO6EWXDg4Q2c5E\_xLDozrLRlJVHWIGEfvD115StKSvyZEXibDtpMV1GSS\_ZhBCjr31p\_a7KrgkOlPKqS1OXx6tBHRriYidqmAvpT5HEwXyCkeZYndAz5AWWalmgZ3vEx3m8ey1rs)

* There’s no need to go into the depth of how we obtained this formula right now.

### Sigmoid Function (Logistic Function/ Logit)

* Take linear regression function and put it into the Sigmoid function
* Sigmoid function outputs probability between 0 and 1

![](https://lh5.googleusercontent.com/zqg\_v7KKlN-OnL9eFMusr9JzlzhdqEW-OCmIoj7ghgxOaD0g-meCDzTSWx6IRk\_YY01tMMJ2D5Yi16KjrLhh913ZUK4vNR3mhw9TI3jnEnviuV2Q100rlT6rGRt3UA5TzDyBjkitxTw)

* Sigmoid function outputs probability between 0 and 1 (y axis)
* Default probability threshold is set at 0.5 typically&#x20;
  * Class 0 – Below 0.5
  * Class 1 – Above 0.5

![](https://lh5.googleusercontent.com/Sn\_69j3JusUmdbl87c-PQCBGTF82Oy4xmsXt40-ZV\_t6IfhMlW66T4NLK-JZMdV-dyIh0xIWh2RNF4gaHQJ2mLIDgYYv-RASkSBa8xLNDRLnag57D6RrZyO3R34VZpdimXFukZy7\_M4)

### Types of Logistic Regression

Logistic Regression model can be classiﬁed into three groups based on the target variable categories:

* **Binary Logistic Regression**
  * The target variable has two possible categories.
  * Common examples : 0 or 1, yes or no, true or false, spam or no spam, pass or fail, Transactions (Fraudulent / Not Fraudulent), Medical Condition (Diseased/ Not diseased)
* **Multi- Class Logistic Regression**
  * **Multinomial Logistic Regression**
    * The target variable has three or more categories which are not in any particular order. So, there are three or more nominal categories.
    * Examples: Fruits (apple, mango, orange and banana), profession (e.g., with ﬁve groups: surgeon, doctor, nurse, dentist, therapist)
* **Ordinal Logistic Regression**
  * The target variable has three or more ordinal categories. So, there is intrinsic order involved with the categories.
  * For example, the student performance can be categorized as poor, average, good and excellent.

We will be discussing about Multi-Class Logistic Regression in the next module!

### Notebook on Logistic Regression

* [https://dphi.tech/notebooks/891/manish\_kc\_06/logistic\_re](https://dphi.tech/notebooks/891/manish\_kc\_06/logistic\_regression\_insurance) [gression\_insurance](https://dphi.tech/notebooks/891/manish\_kc\_06/logistic\_regression\_insurance)

### Let’s do some practice

**Instruction:**

* Use the raw data github link: [https://raw.githubusercontent.com/dphi-official/Datasets/master/HR\_comma\_sep.csv](https://raw.githubusercontent.com/dphi-official/Datasets/master/HR\_comma\_sep.csv)
* Or you can download it here from [here](https://www.kaggle.com/giripujar/hr-analytics)

**Exercise:**

* Load libraries and data.
* Do some exploratory data analysis to ﬁgure out which variables have direct and clear impact on employee retention (i.e. whether they leave the company or continue to work)
* Plot bar charts showing impact of employee salaries on retention
* See the correlation between department and employee retention
* Separate dependent and independent variables.
* Split the data into train set and test set
* Now build Logistic Regression model and do prediction for test data
* Measure the accuracy of the model
