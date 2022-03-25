# Day 2: Decision Tree

### Learning Objectives

* **Decision Trees**

### Understanding Decision Trees

* The following video explains clearly what a decision is and how it works with bunch of live examples.
* Alongside it will talk about some mathematical aspects such as gini impurity. It would be good to understand them in long run, though you may not want to overwhelm yourself with too many jargons at the moment.

{% embed url="https://youtu.be/7VeUPuFGJHk" %}

* A simple non-technical explanation of decision tree: [https://towardsdatascience.com/a-beginners-guide-to-d](https://towardsdatascience.com/a-beginners-guide-to-decision-tree-classification-6d3209353ea) [ecision-tree-classification-6d3209353ea](https://towardsdatascience.com/a-beginners-guide-to-decision-tree-classification-6d3209353ea)
* A comprehensive article on decision trees that talks about optimisation criteria, pros and cons etc: [https://www.datacamp.com/community/tutorials/decisio](https://www.datacamp.com/community/tutorials/decision-tree-classification-python) [n-tree-classification-python](https://www.datacamp.com/community/tutorials/decision-tree-classification-python)

### Let’s do some practice

* Now that we know how to build a simple decision tree model on one of the datasets that we used previously.
* **Objective:** Imagine you were hired as a Data **** Scientist/Analyst by the Central Police Oﬃce of Metropolitan areas and your job is now to create a predictive model for crime\_rate. For now, let’s focus on building a simple decision tree.
* **Link to the Dataset:** [https://docs.google.com/spreadsheets/d/12C585fc6rZu9c-GbrPIZLKo1nB1ZjSAGuiaR9fxibSY/edit?usp=sharing](https://docs.google.com/spreadsheets/d/12C585fc6rZu9c-GbrPIZLKo1nB1ZjSAGuiaR9fxibSY/edit?usp=sharing)
* Download the dataset as a CSV file.

### Hints

* This is a regression problem as the outcome variable is continuous. Hence, you need to use a Regressor instead of classifier in the below lines of code. A reference example of regressor problem can be found [here](https://www.kaggle.com/dansbecker/your-first-machine-learning-model).
* from sklearn.tree import DecisionTree**Classifier** model = DecisionTree**Classifier**() model.fit(X\_train, y\_train)

### What next?

* If you were able to build a model then don’t forget to share it here with fellow learners:
* **You surely deserve a praise for your first Machine Learning Model!**
