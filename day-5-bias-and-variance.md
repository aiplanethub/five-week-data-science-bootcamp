# Day 5: Bias and Variance

### Learning Objectives

* Bias and Variance

### **Bias and Variance in real world**

In dictionary terms :

* **Bias :** Prejudice in favor of or against one thing, person, or group compared with another, usually in a way considered to be unfair.
* **Variance:** The state or fact of disagreeing or quarreling.

In short, Bias represents how unfair is something towards others, and Variance represents how likely something changes with respect to others.

Confusing ? Worry not. The next example will clarify all your doubts.

### Example

* Let’s assume you have called two weather examiners, Mr. Bishop and Mr. Varian to test if it will rain or not.
* Mr. Bishop loves rain a lot. And Mr. Varian is a bookworm. Let us talk about the conditions for rain.
  * **It rains only if it’s little humid.**
  * **It does not rain if it's windy, hot or freezing.**

### **Mr Bishop representing Bias**

You ask Mr. Bishop (Despite of his training, he is too biased towards rain) :

* Me :Sir, its extremely hot out here, will it rain ? \
  Mr. Bishop : Yup.
* Me :Sir, its little windy, will it rain ? \
  Mr. Bishop : May be not.
* Me :Sir, its freezing will it rain ? \
  Mr. Bishop : Yes of course.
* Me :Sir, its little humid, will it rain ? \
  Mr. Bishop : Damn sure.

Did you notice, Mr. Bishop is highly Biased towards chances of having rain. During the test, he is unable to predict most of them correctly.

This condition is called **under ﬁtting**.

### Mr Varian representing Variance

Now let us see your conversation with Mr. Varian (a bookworm who completely remembers the training he had ):

* Me :Sir, its extremely hot out here, will it rain ? \
  Mr. Varian: Nope.
* Me :Sir, its little windy, will it rain ? \
  Mr. Varian: No way.
* Me :Sir, its freezing, will it rain ? \
  Mr. Varian: No way.
* Me :Sir, its little humid, will it rain ? \
  Mr. Varian: Yes it will.

Mr. Varian successfully predicted whether it will rain or not. But being a bookworm, Mr. Varian is unknown to the conditions not described in the book during training.

Now, we ask Mr. Varian :

* Me :Sir, there is a giant sitting on the cloud who lost his candy. Will it rain ?&#x20;
* Mr. Varian: Not sure, since the answer is “No” to most of the conditions, there is a high possibility that it will not rain .

Now, although the decision of Mr. Varian varies perfectly with the input conditions, he is not able to predict for the new and unseen condition (other general conditions apart from the given speciﬁc conditions while training).

This condition is called **over ﬁtting.** And it oﬀers **poor generalizability**.

### High Bias or High Variance?

* Then what is better, high bias (high generalizability) or high variance (high accuracy on training data) ?
* Well, the answer is, “Best of both worlds”. We neither need high bias nor high variance. We would want our algorithm to perform better on training set and also oﬀer best result on unseen data (the test set).
* In general, **having high bias reduces the performance of the algorithm on training set while having high variance reduces performance on unseen data.**
* This is known as **Bias Variance Trade oﬀ**.

### Reading Material

* MUST READ Understanding the Bias Variance Tradeoﬀ: [https://towardsdatascience.com/understanding-the-bias-variance-trade](https://towardsdatascience.com/understanding-the-bias-variance-tradeoff-165e6942b229) [oﬀ-165e6942b229](https://towardsdatascience.com/understanding-the-bias-variance-tradeoff-165e6942b229)
