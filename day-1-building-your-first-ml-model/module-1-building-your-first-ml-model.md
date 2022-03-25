# Module 1: Building your First ML Model

### Learning Objectives

* Machine Learning & its use-cases
* ML Keywords
* Building our First ML Model
* The ABC of Machine Learning

### What is Machine Learning?

* Machine learning provides systems the ability to **automatically learn and improve from experience without being explicitly programmed**.
* It allow computers to discover hidden and useful insights
* **In nutshell, Machine Learning is a new way of communicating your wishes to a computer.**

### What is a Machine Learning (ML) model?

* For now, let’s consider it is a Magical box that help us to predict what we want. In the below case we want to predict whether an incoming email should land in our inbox or spam box. We will discuss more about ML models soon.

![](https://lh6.googleusercontent.com/6C1t6wAMbv0xWe7jeT4ubjIEwxwh\_C1NO2Zj583c8BM6EnGJSfV692H4ax\_B4VsvWH2ysKMcd7tLamOnyPRERpLJID4duE8v6MkJ2IhDXvmmK7\_rQ6kcks92e60yCSl\_\_1nzbwOGKNA)

### Machine Learning is used in..

* **Fraud detection** - **Eg:** Credit card fraud detection. It will help us to detect whether a transaction is fraud or not.
* **Email spam ﬁltering** - **Eg:** Helps in categorising whether a particular email should go in inbox or spam box.
* **Recommendation engines** - **Eg:** E-commerce platforms like Amazon can recommend you a similar product based on your previously browsed list of products and many more!!!

**Let’s understand some keywords in ML**

### Variables/features

* **Features or Variables:** These are the the most common terms that we would come across from now on.
* **Features and Variables both are the same in a dataset**, they are often interchangeably used. So there is no need to worry about it!

![](https://lh5.googleusercontent.com/5\_t8Ii2-2ppXa-j6aEJDD7wW70MdPF9lBSF61HaYT\_TOk0r1IUb837JC3jWgM\_bMhO4T0bD4anMkha3yzKhGjhaEcyilq4lwyf\_dt\_FJEl4oUcYVSm74W\_Uo93Ykyo-hzm-JDTPqWZ8)

### Label/Target Variable

* The target variable or label of a dataset is the feature of a dataset about which you want to gain a deeper understanding.
* It is the variable that is, or should be the output.
* In the example of detecting spam emails, the label will be the category the email belongs to, i.e it will be either ‘spam’ or ‘not spam’.

![](https://lh4.googleusercontent.com/5XMegCOmzDt5uy3wy2p\_qaEoYBv\_TyodI5ODgKjkwjeZoDYZCHSgRzyjvqk\_EMgMc7gFe6AKSahbnYN3FBjSx6UGZHTERr\_PLIsKv1FgknfAuBCH7qJPXehuZlrwKU4ymDKxiZFFv7c)

### Predictor/Input Variables

* One or more variables that are used to determine (or predict) the 'Target Variable' are known as Input Variables. They are sometimes called Predictor Variable as well.
* In the spam detector example, the features could include the following:
* words in the email text
* sender's address
* time of day the email was sent
* email contains the phrase "congrats you won $1 billion - share your bank details."

&#x20;                                       &#x20;

![](https://lh6.googleusercontent.com/qn77bAasoGbqBMvbwF7032Pg6o5R8d5IlBG6W7FPh-bLwIVLl1DOrTJb4pnQSapSzR8dY3H0ewAigv08kuxvGzZUFo17-dVyi7LmA5JjGBBFXM31goZfhAdzEMmuFkTZ5-6J9a0PQ4s)

### Target and Input variables

* Remember the Standard Metropolitan Areas Data used in previous slides? In that dataset **we might be curious to predict “crime\_rate” in future**, so that becomes our target variable and rest of the variables become input variables for building a machine learning model.

![](https://lh3.googleusercontent.com/uvLkUlvXcib9YkhlSLYTenIXxrRBVlieVfbS6VD7SbfGt-NNv3MvvEzWRw0wioZuFMmesUlAcDiaWg1jzXs1mz7w6jpdLYtuJB2cQMOuVdra5uKp0iI0MwoZlrDFC8DCp\_uCIro6uhY)

### Train and Test Set

![](<../.gitbook/assets/image (10).png>)

### Exams

**Case 1:**

* You end up reading everything in the textbook
* You performed well in the test

**Case 2:**

* You got the test questions through some means and you ended focusing more on it
* And obviously, you performed well

**Is there any learning in case 2? - will you be able to perform well if you are exposed to new questions?**

There might be some learning (we end up learning those few questions) and we might end up getting good grades too as we know the test questions. But we don’t know want will happen if we are exposed to new questions that are outside the leaked test questions right?

Let’s say the school authorities learnt about the test paper leak and changed the questions (which you would know only after starting your exam and you are under prepared). Then we might end up getting not so great score. Because we have trained ourselves on those speciﬁc test questions that are leaked. Implying we just trained ourselves on a speciﬁc test paper and our learning was bad when move out of our comfort zone and expose ourself to new set of questions.

**Crux of the story:** We should never expose test data while training a model as it might lead to overﬁtting that might give you good results for that particular data but when exposed to new data we might get bad results.

### Sports

* **Train:** We get trained at our local sports centers
* **Internal matches (Test):** For preparation
* **Future:** Get ourselves exposed to the real matches - national and international championship

### Train and Test Dataset

* This is exactly why we need to test machine learning models on **unseen data or test data.** Otherwise, we have no way of knowing whether the algorithm has learned a generalizable pattern or has simply memorized the training data.
* **TRAINING DATA:** The observations in the training set form the experience that the algorithm uses to learn.
* **TEST DATA:** The test set is a set of observations used to evaluate the performance of the model using some performance metric. **It is important that no observations from the training set are included in the test set.** If the test set does contain examples from the training set, it will be diﬃcult to assess whether the algorithm has learned to generalize from the training set or has simply memorized it.

### Train Test Split

* Consider an Example where our Original Dataset has 1000 rows.
* When we start building our ML model we will split our datatset into two parts (70% train data and 30% test data).
* We will train our model on 70% of data i.e 700 rows and then test our model performance on 30% of data i.e 300 rows. As discussed above while testing our model we will not provide the outcome to our model for the test data although we know the outcome and instead let our model give us the outcome for those 300 rows.
* Later we will compare the outcome of our model to the original outcome of our test data to get the accuracy of our model predictions.
* For splitting our data to training and testing set we use **train\_test\_split method of scikit-learn library.**

### Understanding Target Variable

To identify whether it is a classiﬁcation or regression problem

### Target Variable Classiﬁcation vs Regression

Classiﬁcation:

* Classify the outcome
* Examples:
  * Predict whether a transaction is fraud or not fraud
  * Predict whether to give loan or not
  * Predict whether to give college admission or not
  * Predict the grade (Grade A, B, C, D)
  * Note: Classiﬁcation can be more than two

### Regression

* Regression is the problem of predicting a continuous outcome (a numeric outcome)
* Examples:
  * Predict house price
  * Predict crime rate

### Machine Learning Classiﬁcation Vs Regression

![](https://lh4.googleusercontent.com/qduW-NSU3iDq0rEgfcUCL6IyvLZli9faZcqCwWLAeyxafL-8uRP41yGP2caTHwuB\_\_SS7rE2n7KzsjuWW0oGyNbety0UGJc7eGOucoJSaED4RwU306kdjjySbjtH9iUiMV1Qm-nnb0Q)

### Data Science Modeling Process

![Credits: https://towardsdatascience.com/data-science-modeling-process-fa6e8e45bf02](https://lh6.googleusercontent.com/nZqGT4s66lj2bqoiehpyS9uYvVze2XuHyHjLZ9ugL8MiMOB1LnTtenaYNpSETqSX3K6T3344q57TibABoqsRu8ICQqoIqIXEkQ8F5PYN7RszI3qpWaWy\_SSGCmldf1w35t3YKJd-9Ds)

### Problem Solving

* Deﬁne Objective or understand the problem statement
* Data Requirements
* Data Collection
* Exploratory Data Analysis
* Data Pre-processing
* Build a model
  * Understand whether it is a regression or classiﬁcation problem
* Evaluate
* Optimise
* Production
* Monitor
* You keep Optimising it every now and then

### Objective/Problem Statement

* The goal of the model is to **predict whether a passenger survived or not in the Titanic disaster**, given their age, class and a few other features.

![](https://lh4.googleusercontent.com/aFhJVO3XnWb-gaYwHVvPb4Pp8I7-CNqtqhyYctwxLLO53Vf1JhgSeChXhBBeYIQQHmp3mYwV46Wqym\_kLYjZmNlaVjC1sywaKm02oy-8YOny4PGVYFS8ugnRBTpKPB6Vk5wLkLRInj8)

### Data

* We have the data!

### Understanding the Data

* PassengerId - this is a just a generated Id
* Pclass - which class did the passenger ride - ﬁrst, second or third
* Name - self explanatory
* Sex - male or female
* Age
* SibSp - were the passenger's spouse or siblings with them on the ship
* Parch - were the passenger's parents or children with them on the ship
* Ticket - ticket number
* Fare - ticket price
* Cabin
* Embarked - port of embarkation
* Survived - did the passenger survive the sinking of the Titanic?

### Explore the data

* Let’s get to the notebook [https://github.com/dphi-oﬃcial/Data\_Science\_B](https://github.com/dphi-official/Data\_Science\_Bootcamp/tree/master/Week3)[ootcamp/tree/master/Week3](https://github.com/dphi-official/Data\_Science\_Bootcamp/tree/master/Week3)

### Omitting Irrelevant Variables/Columns

* You shouldn’t drop columns or variables just like that! Unless there is a strong premise.
* Id, port, cabin and name

### Split the data into train and test

![](<../.gitbook/assets/image (7).png>)

### Model Building - Decision Tree

* Now what is this decision tree?
* Well, we all might have seen it by now!
* Decision Tree Examples

![](https://lh6.googleusercontent.com/F\_VOLwD3xz5yBl0WV29tQJnX4ObZfwozOSCiuoDVRNIT1Y7DWOJjHlWdpQuNnfeLb2J9l4JNQcEfyKhj9JvgaC9NRfjF1LYk2-76Utb5JUWcx1XxO6ks7Tt6cTnqcuzEul8o8AYOcG8)

![](https://lh6.googleusercontent.com/qaYfqCzctiGOQt\_a94CoYoMyFxzH4eyTcrUVwqbhLmc5Dgf5kNJHRozV3qOd7I40UXk2tlBrqSOLJGs5nPBwMKj33Eu-T9V1SU9a3MlnFLuHjTPn2PEJ-m8IirQ\_KEvluNwWFvXSWTc)

### Now what next?

![](https://lh4.googleusercontent.com/aFhJVO3XnWb-gaYwHVvPb4Pp8I7-CNqtqhyYctwxLLO53Vf1JhgSeChXhBBeYIQQHmp3mYwV46Wqym\_kLYjZmNlaVjC1sywaKm02oy-8YOny4PGVYFS8ugnRBTpKPB6Vk5wLkLRInj8)

Let’s do it!

### Model Evaluation

* **Evaluate on test dataset to check the performance!**
* Well, we build a model on historical data and expose them to new data that we would see in future. Technically they will be exposed to unseen data

### Overﬁtting - Underﬁtting

![](https://lh3.googleusercontent.com/QyS3P7n53Wwdtq\_LuwFYta3aTtMEvdcYuX1\_J4rz3bjoGrvJcf8BEHcH3RKoeJT9Fm4\_ZvYk8GufUMH9cE75exCVJcHUys02f9V2gnJoU7tNyiXqT6XYJaPNYlY0p0b21Zzs8tCsyIw)

![](https://lh5.googleusercontent.com/ylQSLxOPDMs4PmrUMLrTIPi4l3ksQoNjfJf1hTd5SJXUunvjXRSDxZPY01QbdhMkhP-mPiBEY4W9gTAg0raPwhr38oVK\_\_4zp7q-lHs6r4b1H2tSvGIWd6oLLBR2Rn6UDnGGEcDuGYU)

### Model Evaluation

**!!** We are not done yet, We can improvise it signiﬁcantly.

How? It will be followed in due course!

### What else can be done in general?

* Feature Selection
* Cross validation
* Applying diﬀerent ML Models
* Hyper parameter tuning etc

And as data scientist we must keep optimising and building better models that derives meaningful results.
