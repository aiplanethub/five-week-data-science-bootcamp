# Module 1: Introduction to Machine Learning

### Learning Objectives

* The ABC of Machine Learning
* Imbalanced Dataset
* One-hot encoding
* Session Details

### What is Machine Learning?

* Machine learning provides systems the ability to **automatically learn and improve from experience without being explicitly programmed**.
* It allow computers to discover hidden and useful insights
* **In nutshell, Machine Learning is a new way of communicating your wishes to a computer.**

### Machine Learning is used in..

* **Fraud detection** - **Eg:** Credit card fraud detection. It will help us to detect whether a transaction is fraud or not.
* **Email spam ﬁltering** - **Eg:** Helps in categorising whether a particular email should go in inbox or spam box.
* **Recommendation engines** - **Eg:** E-commerce platforms like Amazon can recommend you a similar product based on your previously browsed list of products

### What is a Machine Learning (ML) model?

* For now, let’s consider it is a Magical box that help us to predict what we want. In the below case we want to predict whether an incoming email should land in our inbox or spam box. We will discuss more about ML models soon.

![](https://lh5.googleusercontent.com/mOSQ3UUeRbhWgcJjD9Hu1OEqCAEB2go0Uk5EbMNOm9ddlvPoFhkKfdAOjgaNS1pLPOL3NuSRLi4PzjZAoUuOZY7KfgYTve8qyi7JJyVB3fljMzi0FG1MW3L1p5rvYv1-aeCKGy0RPLY)

### Variables/features

* **Features or Variables:** These are the the most common terms that we would come across from now on.
* **Features and Variables both are the same in a dataset**, they are often interchangeably used. So there is no need to worry about it!

![](https://lh5.googleusercontent.com/p2Pg0DD\_IhExzWxYrq5GZnCnH\_AyQRHqe4cF0L9rxO3mwgKVj2IfKYq1K\_n926wKt6qTvKDnahXalnFOfaf10b7SfyX5-Zp4KDegu3P0Awqz0NmBlKNcgsTVbQIEcCHPyM8KzsAqv3Q)

### Target/Label Variable

* The target variable or label of a dataset is the feature of a dataset about which you want to gain a deeper understanding.
* It is the variable that is, or should be the output.
* In the example of detecting spam emails, the label will be the category the email belongs to, i.e it will be either ‘spam’ or ‘not spam’.

![](https://lh3.googleusercontent.com/T0JEWSQIc-Gk1hidwSEz7IVzA3-dJD1POWpyjBj43NkB4-5YPlhj5mKMNcSWVe5-\_AQuXceBTGN78qXEnqXMYhMqX-pbVONnzUEtJidOpAYDcl4xavX4egrCE0ohfsCjXn3FPrtNXF0)

### Predictor/Input Variables

* One or more variables that are used to determine (or predict) the 'Target Variable' are known as Input Variables. They are sometimes called Predictor Variable as well.
* In the spam detector example, the features could include the following:
  * words in the email text
  * sender's address
  * time of day the email was sent
  * email contains the phrase "congrats you won $1 billion - share your bank details."

![](https://lh6.googleusercontent.com/4WD0kCk6rKCmVV1dBH9M83v6qAEDVAdwBakCaQgpMOEOSujp6COnoG8I7KtNFl9FrZIdolF9rFnWtso0abjEdUuMLMvX9TeP4X-4anuXao0Zbk9BxPcrDIUFQ4S\_1QY6uzFExGiNN7A)

### Target and Input variables

Remember the Standard Metropolitan Areas Data used in previous slides? In that dataset **we might be curious to predict “crime\_rate” in future**, so that becomes our target variable and rest of the variables become input variables for building a machine learning model.

&#x20;                     &#x20;

![](https://lh4.googleusercontent.com/EI1TRgV5YcrEkFaXfVrdFNMt2PUVw\_cD0EhKS6NulfzpWzwOz\_d0vs-U7ncDfflsTehfIdAulL5I7TKa0XWuVamAEDS0hCWKEE4Dwm4i5RDNpwToRxp37MzTJ0xWt8oLuscJ58X5VYk)

### Train and Test Set

![](https://lh4.googleusercontent.com/vmm6HV-ZSgw0-WBlS3564rZwgXL\_MxS3ISwvBti1j0rppLKl1deoudh\_HvGciTBb7NG76ElZcOq2K7-i9xNQbsFjQB16oJw5o5IFGsQ\_MmLgW4JkvX22U13IyJi6mhJeSaOaEg9uLx8)

* To use an analogy, let’s say you teach a child to multiply by letting the kid train on the small multiplication table, i.e. everything from 1\*1 __ to 9\*9.
* Next, you test whether the kid is able to perform the same multiplications. The result is a success. The kid gets it right almost every time.

![](https://lh4.googleusercontent.com/udcg0PbNqsYXySLKdx8S8ZJrBrr9hfS4zYSe3uhFR1fyeRGTuzsuX0uOQIJ8L5qctJxIe6lTTMNnmPPiHVQA0\_KXNhiYZf\_9dHi2RrwZHNRuYa83Co\_U4RqAkyC7mLvQzVOSbaOVILE)

* What’s the problem here?
* You don’t know if the kid understands multiplication at all, or has simply memorized the table!
* So what you would do instead is test the kid on multiplications like 11\*12, that are outside of the table.
* This is exactly why we need to test machine learning models on **unseen data or test data.** Otherwise, we have no way of knowing whether the algorithm has learned a generalizable pattern or has simply memorized the training data.
* **TRAINING DATA:** The observations in the training set form the experience that the algorithm uses to learn.
* **TEST DATA:** The test set is a set of observations used to evaluate the performance of the model using some performance metric. It is important that no observations from the training set are included in the test set. If the test set does contain examples from the training set, it will be diﬃcult to assess whether the algorithm has learned to generalize from the training set or has simply memorized it.

### Train Test Split

* Consider an Example where our Original Dataset has 1000 rows.
* When we start building our ML model we will split our datatset into two parts (70% train data and 30% test data).
* We will train our model on 70% of data i.e 700 rows and then test our model performance on 30% of data i.e 300 rows. As discussed above while testing our model we will not provide the outcome to our model for the test data although we know the outcome and instead let our model give us the outcome for those 300 rows.
* Later we will compare the outcome of our model to the original outcome of our test data to get the accuracy of our model predictions.
* For splitting our data to training and testing set we use **train\_test\_split method of scikit-learn library.**

### Data Splitting

* We **separate the data into input and target variable**
* We further **divide them into train and test datasets**

![](https://lh3.googleusercontent.com/\_iksSyu-FVF-Mecj7i8fInqaxztlQ9vdI1xIIBTJow8WgSIK3bIEohZ4dRM3UwMvQmfDd5CFw51irUsDso65POc9TZUIsQ9jxGayM\_5jNSC56cUE7owTHWsO3-SSNsTUCBxzu8hG5Po)

* Let’s consider the following data with 10 entries and our objective is to predict whether someone has purchased a product or not i.e “ProductPurchase” column = Yes or No

![](https://lh3.googleusercontent.com/5HDHEQSh5NSiYH1lnpKt3fx81Dxz29FRfMFubSQ5cGztTBNbacHpH1rtQ5xAMep71HQktFPtxX7Od-KClloppuEtNp7Kp5GbHPs3yo8UBEH-4Us1agh8zuMEdeECGvol5ZXlZXYz8\_E)

* Here, **Country, Age and Salary are the Input variables** used to predict the **target variable - ProductPurchase**.

### Separate Input and Target Variables

* We separate the dataset into two new datasets: one with input variables - X (Country, Age and Salary) and the other with target variable - y (ProductPurchase).
* Adding a snippet from that we used in [our first model building exercise](https://github.com/dphi-official/Data\_Science\_Bootcamp/blob/master/Week3/First\_ML\_Model/ML\_with\_Titanic\_Data.ipynb).

![](https://lh5.googleusercontent.com/viTOP\_S\_nUuvdHXsrvZfBNB6DsnmtFXcIj-lQB1RR2AT-r4JIVkTHLGiKLlqihJpZQ7xmy30Q4pCU62hVK23vsm\_oSXEdGW9LbyX8Fz1fslNiUbL\_3kVgS5h277fPkkkDo8KZYTtAeA)

### Splitting into train and test datasets!

* We’ll now split the x dataset into two separate sets — X\_train and X\_test.
* Similarly, we’ll split the dataset y into two sets as well — y\_train and y\_test.

![](https://lh6.googleusercontent.com/JYxObt\_azo9IXa7tUKHPdsp23xk6AE1ojsPPy4nYeOKuIgQPpG9jV12cE9p5dL2o9f\_-\_BU8bkvu3NPMXD8exuoJV1Ng\_rYG5m8LeBo5nHfEHzKHLnfD\_\_vj\_uPA4nF9GWveuWmcGGM)

* Reference here: [https://github.com/dphi-official/Data\_Science\_Bootcamp/blob/master/Week3/First\_ML\_Model/ML\_with\_Titanic\_Data.ipynb ](https://github.com/dphi-official/Data\_Science\_Bootcamp/blob/master/Week3/First\_ML\_Model/ML\_with\_Titanic\_Data.ipynb)

### One Hot Encoding

![](https://lh6.googleusercontent.com/yZSCqsjVzwVZpEZ6tKjwfVQlWunyDrAV-U6dyW6tp7PiiVwTn76RNDw2AnKZvUV\_\_NASwgXAfW\_d7-qbalRuh78GF8d6MCWbC0r\_B5aZ013xoMCBq5PLQKjql4P33Fv1u5XJz34J5Q0)

****

* **Binary is nothing but assign 0 or 1**
* One hot encoding is a process by which categorical variables (do you remember what categorical variables mean from the stats module?) are converted into a form that could be provided to ML algorithms to do a better job in prediction.
* Let’s consider the dataset in the previous slide
* The Categoricalvalue is just a number assigned to each car company name.
* The problem with this is that it assumes higher the categorical value, better the category. But that’s deﬁnitely not the case, right?
* This is why we use one hot encoder to perform “binarization”(representation in 0 and 1) of the category and include it as a feature to train the model.
* Now what do the 0s and 1s actually represent?
* Look closely at the table on the right in previous slide. In the company name variable example, there are 3 categories (3 car companies) and therefore 3 binary variables are needed ( VW, Acura, Honda).
* A “1” value is placed in the binary variable at the same position at which the particular company name is present in the left table. The rest are kept “0” in that variable’s column. The remaining 2 variable columns are ﬁlled in similar manner.
* In short, all the elements of the vector are 0 except one, which has 1 as its value.
* MUST READ: The following resource justiﬁes the necessity of one hot encoding our data: [https://machinelearningmastery.com/why-one-hot-encode-data-in-machine-lear](https://machinelearningmastery.com/why-one-hot-encode-data-in-machine-learning/) [ning/](https://machinelearningmastery.com/why-one-hot-encode-data-in-machine-learning/)

### Imbalanced Dataset

![](https://lh3.googleusercontent.com/dBl6QENNQtoouq6Zy6JyQzZhscc411b2pHZbVXEv4Wq8zFnEt581Uk71LgKkeIppZtCaxNv6wRzlZGwbPea10FYlQzCqijjqhl96qRjvi689HuQo6MSD0SKoM7qFBTswViP5z2xVb9M)

![](https://lh4.googleusercontent.com/rwit8IImMOU0HadNenmTNH-Uv2r75GitSFp-V17DjLioJmY565H8h\_GBvudxCUE9nD812jQyM\_\_YELPwFwYNit40mzRatdgwW4psWiEHuCaAeeM9DtutL3mXfOpTVXf4Xx21DQlSGeg)

* For example, suppose you have a credit card transaction data and you are supposed to predict fraudulent transactions. You'll likely have 10,000 authentic transactions for every 1 fraudulent transaction, that's quite an imbalance!
* **In machine learning terms:** Often you'll have a large amount of data/observations for one class (referred to as the majority class), and much fewer observations for one or more other classes (referred to as the minority classes).

![](https://lh5.googleusercontent.com/O3AnK5IZbgrI24yEv2ErcvHrfGfsnNLJGuC30tolZa07IIZ9Z3pz6rp74BZSVddIG-sEGX7Fi0RVLBd09um2t\_LiMyAkeO81D\_i8DTCLfoCbN9pzjFSNlmijrJOXbc6IataHv8lLD0w)

*   The problem is that machine learning models trained on unbalanced datasets often have poor results when they have to generalize (predict a class or classify unseen observations). Despite the algorithm you choose, some models will be more susceptible to unbalanced data than others. Ultimately, this means you will not end up with a good model, and the reasons include:

    * The algorithm receives signiﬁcantly more examples from one class, prompting it to be biased towards that particular class.
    * It does not learn what makes the other class “diﬀerent” and fails to understand the underlying patterns that allow us to distinguish classes.

    ****

**Can you think of any other example where there is class imbalance?**

### Data Pre-Processing

* Instructors’ recommended article: [https://towardsdatascience.com/data-preprocessing-con](https://towardsdatascience.com/data-preprocessing-concepts-fa946d11c825)c[epts-fa946d11c825](https://towardsdatascience.com/data-preprocessing-concepts-fa946d11c825)****
* **P.S:** Try opening in incognito if it is asking for a premium subscription upgrade

### Download Dataset

* **Download IEEE Fraud Dataset:** [https://github.com/dphi-oﬃcial/Datasets/blob/maste](https://github.com/dphi-official/Datasets/blob/master/fraud\_data.csv) [r/fraud\_data.csv](https://github.com/dphi-official/Datasets/blob/master/fraud\_data.csv)****
* **!!! - it is a huge dataset so opening it in excel might be diﬃcult, so please open it via python environment - (Colab or Jupyter notebook)**
* Read about this dataset here: [https://www.kaggle.com/c/ieee-fraud-detection/data](https://www.kaggle.com/c/ieee-fraud-detection/data)

### **About the Dataset - IEEE Fraud Dataset**

* The data is broken into two ﬁles identity and transaction, which are joined by TransactionID

**Transaction Table \***

* **TransactionDT:** timedelta from a given reference datetime (not an actual timestamp)
* **TransactionAMT:** transaction payment amount in USD
* **ProductCD:** product code, the product for each transaction
* **card1 - card6:** payment card information, such as card type, card category, issue bank, country, etc.
* **addr:** address of the customer
* **dist:** distance
* **P\_ and (R ) emaildomain:** purchaser and recipient email domain
* **M1-M9:** match, such as names on card and address, etc.

**Categorical Features:**

* ProductCD
* card1 - card6
* addr1, addr2
* Pemaildomain Remaildomain
* M1 - M9 (bank sensitive data)

Note: Some of the feature/variable description is not given as

**Identity Table \***

* Variables in this table are identity information – network connection information (IP, ISP, Proxy, etc) and digital signature (UA/browser/os/version, etc) associated with transactions.
* They're collected by Vesta’s fraud protection system and digital security partners.
* (The ﬁeld names are masked and pairwise dictionary will not be provided for privacy protection and contract agreement)
* Categorical Features:
  * DeviceType
  * DeviceInfo
  * id12 - id38

### Notebook Link

* [https://dphi.tech/notebooks/2646](https://dphi.tech/notebooks/2646)&#x20;
* **!! The dataset takes a lot of time to upload on colab. You might prefer using Jupyter Notebook for this one.**

