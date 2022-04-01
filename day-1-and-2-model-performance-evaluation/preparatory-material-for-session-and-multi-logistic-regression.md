# Preparatory Material for Session & Multi-Logistic Regression

### Learning Objectives

* Multi- Logistic Classiﬁcation
* Why not Accuracy?
* Evaluating the Performance of Logistic Regression model
* Confusion Matrix

### What is Classiﬁcation?

**Let’s learn with some examples:**

* In **Classiﬁcation we** classify the outcome
* **Examples:**
  * Predict whether a transaction is fraud or not fraud
  * Predict whether to give loan or not
  * Predict whether to give college admission or not
  * Predict the grade (Grade A, B, C, D)
  * Note: Classiﬁcation can be more than two

![](https://lh3.googleusercontent.com/ja4Yd0IGe6MpB\_3Cul\_--oPIQ08Z4AaHdb\_UKspx-VUfzLUZnp51ZVEXSp6AXLReKZ91wSKIfaHDP42HY4sKE9GEllqrtCNzAun1ENyIEjTX6NZiWkJdazJX3uTlY\_sXMsfI6ayb7wc)

### What is Multi-Classiﬁcation?

**It is as simple as dividing waste into 4 categories - plastic, glass, metal, paper**

![](https://lh3.googleusercontent.com/BhRjOv5NmtWNeME2JKhF7oeCxgT7zxQ3DwDmZGSBtl1jMYf\_SYWORWzZ1dYpYaxj-8lKNUZxCvuhLSTyJAINVNgHhOoxTC0FoRjVsSPJK5Ii7SX7sK1b9xkP4ZBHDG5q7oq6QUHdJR0)

### Understanding Multi-Class Logistic Regression

{% embed url="https://www.youtube.com/watch?t=8s&v=J5bXOOmkopc" %}

### **Evaluating the Performance of Logistic Regression model**

* **Model Evaluation is a very important part in any analysis to answer the following questions:** _How well does the model ﬁt the data?, Which predictors are most important?, Are the predictions accurate?_
* **Guess what, evaluating a Classiﬁcation model is not as simple as Linear Regression.**
* But why?
* You must be wondering ‘Can’t we just use accuracy of the model as the holy grail metric?’

### Notebook

* Link to notebook: [https://dphi.tech/notebooks/893/manish\_kc\_06/multicla](https://dphi.tech/notebooks/893/manish\_kc\_06/multiclass\_logistic\_regression)[ss\_logistic\_regression?](https://dphi.tech/notebooks/893/manish\_kc\_06/multiclass\_logistic\_regression)

### Accuracy

* Classiﬁcation Accuracy is what we usually mean, when we use the term accuracy. It is the ratio of number of correct predictions to the total number of input samples.

![](<../.gitbook/assets/Screen Shot 2022-04-01 at 9.53.06 PM.png>)

### Why not Accuracy?

* Accuracy is very important, but it might not be the best metric all the time. Let’s look at why with an example -:
* Let’s say we are building a model which predicts if a transaction is fraudulent or not
* Let’s imagine, we build a basic model which always predicts that a transaction is not fraudulent. Guess what would be the accuracy of this model?
* **\~99% !!** (You may ask why? Well, less than 1% transactions are usually fraudulent and there is a huge class imbalance. So even if you ﬁt a wrong model that always predicts a transaction to be not fraudulent, the accuracy will remain 99% owing to class imbalance)
* Impressive, right? Well, the probability of a bank buying this model is absolute zero. 😆
* In a problem where there is a large class imbalance, a model can predict the value of the majority class for all predictions and achieve a high classification accuracy.
* While our model has a stunning accuracy, this is an apt example where accuracy is definitely not the right metric.
* **Watch till 1 min 14 secs to understand why accuracy is bad metric for model performance**

{% embed url="https://www.youtube.com/watch?v=XeJZbCT84Js" %}

**Is confusion matrix confusing or it resolves the confusion? You decide!**

### Confusion Matrix

A confusion matrix is a table that is often used to describe the performance of a classiﬁcation model (or "classiﬁer") on a set of test data for which the true values are known. The confusion matrix itself is relatively simple to understand, but the related terminology can be confusing.

Let's start with an example confusion matrix for a binary classiﬁer for disease prediction (though it can easily be extended to the case of more than two classes):

![](https://lh3.googleusercontent.com/r7D43OGOShGQ-Z0zmJSDVKaRaH5ikBRbjxG\_xH\_9ofMm7Id-CcrxYj9omf7D3A2aYn3A-Yq0h5rqVW8mBOWGKGaxRrIpggwmh9CiPVPRYECI2I3QINxHhwtumZpjgcksTN32BXd2sY8)

### Confusion Matrix

Let's now deﬁne the most basic terms, which are whole numbers (not rates):

* **true positives (TP):** These are cases in which we predicted yes (they have the disease), and they do have the disease.
* **true negatives (TN):** We predicted no, and they don't have the disease.
* **false positives (FP):** We predicted yes, but they don't actually have the disease. (Also known as a "Type I error.")
* **false negatives (FN):** We predicted no, but they actually do have the disease. (Also known as a "Type II error.")

I know these seem hard to memorise. One thing that has helped me remember these are by putting it in a better way:

**false positives = falsely classiﬁed as being positive.**

### Confusion Matrix

**This is a list of rates that are often computed from a confusion matrix for a binary classiﬁer:**

* **Precision:** Correctly predicted as positives compared to total predicted as positives

Precision = **TP/(TP+FP)** = 100/110 = 0.91

* **Sensitivity/Recall:** Correctly predicted as positives compared to total number of positives

**= TP/(TP + FN)** = 100/(100+5) = 0.95

**Note: Mostly we have to pick one over other, it’s almost impossible to have both high Precision and Recall.**

* **Speciﬁcity:** Correctly predicted as negatives compared to total number of negatives **= TN/(TN + FP)** = 50/(50+10) = 0.83

### Understanding Precision and Recall

* Think about the search box on Amazon home page.

![](https://lh3.googleusercontent.com/rLI34yXrzfnXa2A2U24XlMOVbj\_Ody4A-1RzNQsM0OKIT7XkOLMONFI9j5217jlYfKovs-mDl6ttmFtHlR5O9JQHcwDUBBHS5f6qqWIWpV8Q2TQ5o5A0PFC66\_IMYR6MhmHBjdrhWeQ)

* The precision is the proportion of relevant results( correctly predicted yes) in the list of all returned search results(total predicted yes).
* The recall is the ratio of the relevant results( correctly predicted yes) returned by the search engine to the total number of the relevant results that could have been returned (total actual yes).

### Choosing between Sensitivity and Speciﬁcity

* Often, the sensitivity and speciﬁcity of a test are inversely related. Selecting the optimal balance of sensitivity and speciﬁcity depends on the objective of the problem that needs to be solved.

![](https://lh4.googleusercontent.com/aeb-T58vVF36d2x5V-al2UtXcKlUNrW\_LKKhS2nkQOf9g7glafBsdMdtahaxmNglUIHeKk8N6lS0yXH\_pRnHj282krSYedn0BMBmfHmagcD5xFVKuOcgEiyoDmxiUh-D5rtSfk1FzW8)

* If correctly identifying positive class is important for us, then we should choose a model with higher Sensitivity. However, if correctly identifying negative class is more important, then we should choose speciﬁcity as the measurement metric.

### Sensitivity or Speciﬁcity - an example

* Let’s say we are predicting if a patient has cancer or not. The default probability threshold is kept at 0.5 i.e&#x20;
  * Class 0 (No cancer) – Below 0.5&#x20;
  * Class 1 (Cancer) – Above 0.5

![](https://lh3.googleusercontent.com/Saeooh7vaZLvQkAojAT7RlAiW\_7C4pSem7bNhmhNe-9eH43z9pQS8xpLeuOQX9XhhNCI19Ixi8gfkVXb4H29u2JZaB5WeV-C8bY11JDoIhLybAv\_LCKqyutgUfLjnpj9bMuMeygX5lQ)

### Case 1: Higher Speciﬁcity

* Suppose we want to predict Class 1 (Ci.e patient has cancer) only if we are VERY conﬁdent. (To avoid giving the patient a shock and to avoid unnecessary treatment)
* We can instead change this threshold to 0.7. Thus, we’ll tell someone they have cancer only if we think they have greater than or equal to 70% chance of having a cancer.
* Look at the graph below. SInce the threshold has shifted to the right, so the number of people correctly guessed as having cancer have increased. Thus, the speciﬁcity has increased. ( We are being very speciﬁc with declaring patients with cancer).

![](https://lh4.googleusercontent.com/cfHCXYNLaUZtdy8swcALQXBmLCgHwrsko3tEJE9fiwTdfxH0Uocpj2JFANpLeKrg9FzhrF1TIe7mIqQR8dehU9D1rzHZzVQJk-uENgdvdhGeaBTlA45M0jMc\_5P5o6Zk9kNv2nF-hcY)

### Case 2: Higher Sensitivity

* Suppose we want to avoid missing too many cases of cancer ( avoid false negatives). If a person with cancer is told that he’s well, it can cause a delay in treatment and aﬀect the health badly).
* In this case we can set a lower threshold, say 0.25. Even if a patient has 25% chance of having cancer, we’ll inform him/her.
* Looking at the graph you can see that the threshold has shifted to the left. Most of the people with cancer will be detected in advance in this case. We have completely (or almost) eliminated False Negatives. It will thus result in higher Sensitivity/ Recall. (We are being sensitive in detecting a disease i.e a really sensitive test).
*

![](https://lh4.googleusercontent.com/sF-PIevQY4FOntzsC9WXmGrk-Z\_Jpk18LJJ\_VaC77-qRgF9H6Mtjp5lflFwETbn8kZVkf0bkDghOhTFB-EFkBn88ICOxNDNdBEv5aXK1YjHxzzpmmi3KvtxwIsoUlchOW750a2Ep2BA)



You can watch this video from 00:58 to 5:32 explaining the Sensitivity and Specificity trade off

{% embed url="https://www.youtube.com/watch?t=58s&v=yr73lr4W7Mc" %}

### Confusion Matrix

* Talking about accuracy, our favourite metric!
* Accuracy is deﬁned as the ratio of correctly predicted examples by the total examples.

![](https://lh5.googleusercontent.com/LGSb2pPVXrCTvJMSOwEzH1VIVtUvxldAZP2Ohf5E6DyHGTHkq-m9ipl4f2u4IbRkkFuIWv6dlt6saCNM6soMyjpUt3enakWm4MJ1uN4zxfuoFtrMGg3x-GVY\_\_bgrvBgctf9KKSXEBE)

* **Accuracy:** Overall, how often is the classiﬁer correct?

**= (TP+TN)/total** = (100+50)/165 = 0.91

* Remember, accuracy is a **very useful metric when all the classes are equally important.**
* But this might not be the case if we are predicting if a patient has cancer. In this example, we can probably tolerate FPs but not FNs.
* If a cancerous patient is wrongly reported as being ﬁne, it can result in delaying of treatment. Which is not good!
