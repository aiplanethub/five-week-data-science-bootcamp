# Day 3: Classiﬁcation Algorithms & It's Evaluation Metrics

### **Learning Objectives**

* Difference between Classiﬁcation and Regression
* Classiﬁcation Algorithms & Model Evaluation Metrics
* Which evaluation metrics to use when?

### Disclaimer

* We haven’t taught all the algorithms as the Bootcamp was of 5 weeks and we wanted learners to have a good grasp on the concepts that are being taught and not overwhelm them with all the concepts available. Once you know how to handle data and build models, you can easily build diﬀerent kinds of models.
* Through this module, we’ll be providing material around some of the popular algorithms. In addition, we will sharing some more resources soon.

### Classification vs Regression

![](https://lh3.googleusercontent.com/J-t\_\_YvhZVwiwVmpoh3GGwg54Coak8TiCWNlWVqvq8DQcJEuBY4WOsrqdLiR-FOreqMQtGx9GV5nzxxNVQrDZlje3LCI8KaK-iUaH\_-oGGRseNZFiR2xQlZiVb--vCpKl47UIwufCOc)

In order to decide whether to use a regression or classiﬁcation model, the ﬁrst questions you should ask yourself is: Does your target variable have a continuous value or is it discrete (binary or multi-class)?

### Regression

* If your answer is continuous values, you’re dealing with Regression.
* This means that if you’re trying to predict quantities like height, income, price, or scores, you should be using a model that will output a continuous number.
* So if your objective is to determine tomorrow’s temperature, you should use a regression model.

### Classification

* Let’s come to the second case where if you can clearly see that the target variable is divided into classes. You’ll be using Classiﬁcation here.
* When the number of classes is 2, it is known as Binary Classiﬁcation.
* Eg. Will it be hot or cold tomorrow is a binary classiﬁcation problem with 2 classes: Hot and Cold.
* When it is more than 2, it is known as Multi Class Classiﬁcation.
* Eg. Classifying movies in Good, Average or Bad according to reviews.

### Classification vs Regression

![](https://lh4.googleusercontent.com/FmeOUts7a02ZDwL3RjENVsTZB2trmfIK8WoPcz7Du7K2yt3k7XpsIdyLPo0i1UPFa\_WDmBVA3yA-VDCd2Fd8Lb5NE0Plgi0\_f9xo47h-G\_X1WrDP-uTAEfYnB4Db2Kb-7aMlvBgPBUY)

* It’s important to understand the characteristics of your target variable before you begin running models and forming predictions.

### Classiﬁcation Model Evaluation

Evaluation Metrics

1. Accuracy (Not in case of imbalanced classes)
2. Confusion Matrix
3. Precision
4. Recall/ Sensitivity
5. Speciﬁcity
6. F1 Score
7. AUC ROC

### Accuracy

Classiﬁcation Accuracy is what we usually mean, when we use the term accuracy. It is the ratio of number of correct predictions to the total number of input samples.

![](<.gitbook/assets/image (8).png>)

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
* So you’ve already learnt how to calculate Precision and Recall and how changing the threshold can aﬀect their values. (SImilar to Sensitivity, Speciﬁcity threshold)
* But do we necessarily need to spend time on varying the threshold to get the perfect Precision and Recall? Or is there a way to choose this threshold automatically?
* Let’s take 3 algorithms and try to ﬁnd a metric for combining Precision and Recall.
* How about taking an average of Precision and Recall? (P+R)/2

|             | **Precision (P)** | **Recall (R)** | **Average** |
| ----------- | ----------------- | -------------- | ----------- |
| Algorithm 1 | 0.5               | 0.4            | 0.45        |
| Algorithm 2 | 0.7               | 0.1            | 0.4         |
| Algorithm 3 | 0.02              | 1.0            | 0.51        |

* Average tells us that Algorithm 3 is the best (highest value). Whereas Algorithm 3 is a dumb model that predicts y=1 each time and thus gives a recall of 1 (FN =0, TP=1).
* That means average isn’t a good metric.
* Researchers found a metric that solves our purpose: The F1 Score!

![](https://lh3.googleusercontent.com/svtia\_TltPdvspIUUbqpkjuUbDzl1XmEfNVKKF6yYHeh7osE7bzDtlAGNRxcHPd\_NdsmIFdA-QPnbshAi53Ob3qEbetOIAGThIufwjD\_83o5TkjfFrgBw9Ydfl42quYWW\_BdaigP1q8)

Let’s apply F1 Score to our problem:

|             | **Precision (P)** | **Recall (R)** | **Average** | **F1 Score** |
| ----------- | ----------------- | -------------- | ----------- | ------------ |
| Algorithm 1 | 0.5               | 0.4            | 0.45        | 0.444        |
| Algorithm 2 | 0.7               | 0.1            | 0.4         | 0.175        |
| Algorithm 3 | 0.02              | 1.0            | 0.51        | 0.0392       |

The F1 score tells us that Algorithm 1 is the best (highest F1 Score).

* **For F1 Score to be large, both P and R need to be large.**
* It’ll be highest(1) when both P and R are 1
* Accuracy can be used when the class distribution is similar while F1-score is a better metric when there are imbalanced classes.

### ROC (Receiver Operator Characteristic) Curve

* An ROC curve is a commonly used way to visualize the performance of a binary classiﬁer, meaning a classiﬁer with two possible output classes.
* It shows the performance of a classiﬁcation model at all threshold values.
* It plots 2 parameters:

1. True positive rate /Recall (TPR)

![](https://lh4.googleusercontent.com/\_EbMv-I5S9CoagiEO1fwWRc-CfjpXTxI4hXNFx2Rfyc5OpD3rL\_kAUh3dLUT5IAvHBaJMIg4wzE0XU23ZAjay9lSjvHqNnBoLpb7GFUeIyEYxnwHdssPSFAMM7e0kFomo3JWvq\_QfBo)

1. False Positive rate (FPR)

![](https://lh5.googleusercontent.com/q4\_T6DgsyTylvq67MExjhUSjw7JkiUpv7Rylm\_6k1p\_jiYdtY7OfmEPfJF33D9rxUyr7LQ0PdX19xGR4oHZgJh3swu4TgEUiGklvc1\_FfOPujy6uf5vGflZPU\_UyDeO\_xNZRBKtw60Q)

### AUC Curve

* AUC stands for "**Area under the ROC Curve**." That is, AUC measures the entire two-dimensional area underneath the entire ROC curve

![](https://lh6.googleusercontent.com/gNTI-fJJmK-Sgb17pNFVbi9zo5MbygMtJQpQhjfm4yrOmB6cOSyyEqGknU\_K5xMXWCD8V8RMNKX4BfrDTFpw69p0WyicVLpmTo2y7E9srZZvxgipW-KhW\_2xmevFYXMSz5xaBRT7yhA)

* AUC provides an aggregate measure of performance across all possible classiﬁcation thresholds.

### ROC and AUC Explained

{% embed url="https://www.youtube.com/watch?feature=emb_title&v=OAl6eAyP-yo" %}

### Reading Material

MUST READ - An excellent article explaining Threshold, ROC and AUC in a simple manner: [https://towardsdatascience.com/understanding-the-roc-and-auc-curves](https://towardsdatascience.com/understanding-the-roc-and-auc-curves-a05b68550b69)[-a05b68550b69](https://towardsdatascience.com/understanding-the-roc-and-auc-curves-a05b68550b69)

**Which metrics to use when?**

This is an important question and we get used to learning these measures over time. Sharing some resources with you all so that it helps you understand what metrics to be used in the context of solving a regression problem.

* 5 Classiﬁcation Metrics every data scientist must know [https://towardsdatascience.com/the-5-classiﬁcation-evalua](https://towardsdatascience.com/the-5-classification-evaluation-metrics-you-must-know-aa97784ff226) [tion-metrics-you-must-know-aa97784ﬀ226](https://towardsdatascience.com/the-5-classification-evaluation-metrics-you-must-know-aa97784ff226)
* [https://medium.com/usf-msds/choosing-the-right-metric-f](https://medium.com/usf-msds/choosing-the-right-metric-for-evaluating-machine-learning-models-part-2-86d5649a5428) [or-evaluating-machine-learning-models-part-2-86d5649a5](https://medium.com/usf-msds/choosing-the-right-metric-for-evaluating-machine-learning-models-part-2-86d5649a5428) [428](https://medium.com/usf-msds/choosing-the-right-metric-for-evaluating-machine-learning-models-part-2-86d5649a5428)
