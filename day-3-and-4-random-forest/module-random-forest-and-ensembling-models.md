# Module: Random Forest and Ensembling Models

### Learning Objectives

* Random Forest
* Ensembling Models
* Session Details

### **Random Forests**

* Random forest is a ﬂexible, easy to use machine learning algorithm that produces, a great result most of the times even without hyper-parameter tuning.
* It is also one of the most used algorithms, because of its simplicity and diversity (it **can be used for both classiﬁcation and regression tasks**).
* Random forest **builds multiple decision trees and merges them together** to get a more accurate and stable prediction.

![](https://lh5.googleusercontent.com/bUs0NIKlLZR9mBYLP99T-QblexIzdBwHVUNixiRAdqp2cryzR-5cZexBHd8feH5Q9szEwjNnPaLTR-vOxOoTtv2\_7ptRVoMPDHSs0qmH\_6noMN0\_ZpB7T1wxS0nKwdbFqeeIEjZoU7U)

### Applications

* The random forest algorithm is used in a lot of diﬀerent ﬁelds, like banking, the stock market, medicine and e-commerce.
* In ﬁnance, for example, it is used to detect customers more likely to repay their debt on time, or use a bank's services more frequently. In this domain it is also used to detect fraudsters out to scam the bank. In trading, the algorithm can be used to determine a stock's future behavior.
* In the healthcare domain it is used to identify the correct combination of components in medicine and to analyze a patient’s medical history to identify diseases.
* Random forest is used in e-commerce to determine whether a customer will actually like the product or not.

### Real - life Analogy

* Andrew wants to decide where to go during one-year vacation, so he asks the people who know him best for suggestions. The ﬁrst friend he seeks out asks him about the likes and dislikes of his past travels. Based on the answers, he will give Andrew some advice.
* This is a typical decision tree algorithm approach. Andrew's friend created rules to guide his decision about what he should recommend, by using Andrew's answers.
* Afterwards, Andrew starts asking more and more of his friends to advise him and they again ask him diﬀerent questions they can use to derive some recommendations for him. Finally, Andrew chooses the places that are recommend the most to him, which is the typical random forest algorithm approach.

### Ensemble Models - "The wisdom of crowds"

* Let’s pause and think what Andrew did. He took multiple opinions from a large enough bunch of people and then made an informed decision based on them. This is what Ensemble methods also do.
* You might have two models that each are good at predicting a certain (diﬀerent) portion of your dataset. Combining the 2 models into 1 seems like a good idea to increase performance
* “ensemble” = Combination of models
* Ensemble models in machine learning **combine the decisions from multiple models to improve the overall performance.**
* So basically ensembling/combining two or more algorithms could improve or boost your performance. But there is a logic behind ensembling…you cannot just randomly combine two models and demand an increase in performance….there is a math behind everything.
* So let’s dive into the several ensembling methods that you can try out.

### **Simple Ensemble Techniques**

* In this section, we will look at a few simple but powerful techniques, namely:
  * Max Voting/ Mode
  * Averaging
  * Weighted Averaging
* The max voting method is generally used for classiﬁcation problems. In this technique, multiple models are used to make predictions for each data point. The predictions by each model are considered as a ‘vote’. The predictions which we get from the majority of the models are used as the ﬁnal prediction.
* For example, when you asked 5 of your colleagues to rate your movie (out of 5); we’ll assume three of them rated 4 while two of them gave a 5. Since the majority gave a rating of 4, the ﬁnal rating will be taken as 4. You can consider this as taking the mode of all the predictions.

### Max Voting

* The max voting method is generally used for classification problems. In this technique, multiple models are used to make predictions for each data point. The predictions by each model are considered as a ‘vote’. The predictions which we get from the majority of the models are used as the final prediction.
* For example, when you asked 5 of your colleagues to rate your movie (out of 5); we’ll assume three of them rated 4 while two of them gave a 5. Since the majority gave a rating of 4, the final rating will be taken as 4. You can consider this as taking the mode of all the predictions.

![](https://lh4.googleusercontent.com/5OEO-\_x-\_EBIAdS5FbgitlFo7abhtNEwHjRwoCYd9A2Hcd13doxl8-iexi81d-1\_qo6IcbIONjrvvOG\_7NzRaNYGYsLtzs0\_d0c0tjYvFxbsDRevDzOQqh\_iv3uXtILhJRhwXxfEyRg)

### Averaging

* In this technique, we take an average of predictions from all the models and use it to make the ﬁnal prediction.
* Averaging can be used for making predictions in regression problems or while calculating probabilities for classiﬁcation problems.
* For example, in the below case, the averaging method would take the average of all the values. i.e. (5+4+5+4+4)/5 = 4.4

![](https://lh4.googleusercontent.com/MyYsJlfb7tiiKWGv10c2K6VvjUpeqdBtXpSaOvUHK2d5BgwkwLtO534NCLw-NURomH2eNGu3rVW7a4TcQoiyRN8mEOwja3hHHk7ad6skDrt6OQf6KBbnQGkwKz9ndRgesFXiRG9vTus)

### Weighted Average

* This is an extension of the averaging method. All models are assigned diﬀerent weights deﬁning the importance of each model for prediction.
* For instance, if two of your colleagues are critics, while others have no prior experience in this ﬁeld, then the answers by these two friends are given more importance as compared to the other people.
* The result is calculated as \[(5\*0.23) + (4\*0.23) + (5\*0.18) + (4\*0.18) + (4\*0.18)] = 4.41.

![](https://lh6.googleusercontent.com/5pzdbsZqVmQVfaasu67a4oXKipqo6Bsh6SHlKENyXM\_XIF-KdOeWu0s1agIMOhmZmDPop2GkjlGcminl1xzh-2pKeiMdRIiuoPL3qYLjTajcx3mjRdEqwMnsL2C5KGTyKWOEg4tAJuc)

### Advanced Ensemble Techniques

* Now that we have covered the basic ensemble techniques, we can move on to understanding the advanced techniques, namely:
  * Stacking
  * Blending
  * Bagging Eg: Random forest
  * Boosting Eg: Adaboost, Gradient Boost, Extreme Gradient Boost
* We’ll learn about Bagging and Boosting techniques. There is nothing to worry about them they are just like any other algorithms like linear, logistic and decision tree.

### Bagging ( Bootstrap AAregatING )

* The idea behind bagging is combining the results of multiple models (for instance, all decision trees) to get a generalized result.
* Here’s a question: If you create all the models on the same training data and combine it, will it be useful? There is a high chance that these models will give the same result since they are getting the same input. So how can we solve this problem? A technique called bootstrapping helps us with that.
* Aggregating = Summing or Combining
* Bagging combines the diﬀerent models created by bootstrapping on diﬀerent sets of training data and hence the name Bootstrap Aggregating.
* Random forest is a famous bagging model which uses variations of multiple trees. If same trees are used then it’s a bagged decision tree.

### Boosting

* Here’s another question for you: If a data point is incorrectly predicted by the ﬁrst model, and then the next (probably all models), will combining the predictions provide better results? Such situations are taken care of by boosting.
* Intuitively, each new model focuses its eﬀorts on the most diﬃcult observations to ﬁt till now and attempts to correct the errors of the previous model. So at the end of the process, we obtain a strong learner.
* Boosting, like bagging, can be used for regression as well as for classiﬁcation problems.
* There are various types of Boosting algorithms which we’ll study about soon.

### Reading Material

* MUST READ - Simple guide for ensemble learning methods: [https://towardsdatascience.com/simple-guide-for-ensemble-learning-m](https://towardsdatascience.com/simple-guide-for-ensemble-learning-methods-d87cc68705a2) [ethods-d87cc68705a2](https://towardsdatascience.com/simple-guide-for-ensemble-learning-methods-d87cc68705a2)

