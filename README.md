# Email-Spam-Detection-using-ML

* AIM : To detect spam emails
* DATA SOURCE : https://www.kaggle.com/harshsinha1234/email-spam-classification
* MODEL USED : Naive Bayes Classifier
* ACCURACY OF MODEL ON TEST DATA : 0.9850877192982456

# My YouTube video where I explain the code 

[![Email-Spam-Detection-using-ML](https://img.youtube.com/vi/Mz8OuK3Qf3I/0.jpg)](https://www.youtube.com/watch?v=Mz8OuK3Qf3I)

# What is Naive Bayes Classifier ?
Naive Bayes classifiers are a collection of classification algorithms based on Bayes’ Theorem. It is not a single algorithm but a family of algorithms where all of them share a common principle, i.e. every pair of features being classified is independent of each other. They are fast and easy to implement but their biggest disadvantage is that the requirement of predictors to be independent. In most of the real life cases, the predictors are dependent, this hinders the performance of the classifier. 

For example, a fruit may be considered to be an apple if it is red, round, and about 3 inches in diameter. Even if these features depend on each other or upon the existence of the other features, all of these properties independently contribute to the probability that this fruit is an apple and that is why it is known as ‘Naive’.

Naive Bayes model is easy to build and particularly useful for very large data sets. Along with simplicity, Naive Bayes is known to outperform even highly sophisticated classification methods.

# Why is Naive Bayes Classifier used ?
Naive Bayes Classifier is used because this model is suitable for classification with discrete features so something like word count for a text is exactly what we have here.

# How Naive Bayes algorithm works?
Let’s understand it using an example. Below I have a training data set of weather and corresponding target variable ‘Play’ (suggesting possibilities of playing). Now, we need to classify whether players will play or not based on weather condition. Let’s follow the below steps to perform it.

Step 1: Convert the data set into a frequency table

Step 2: Create Likelihood table by finding the probabilities like Overcast probability = 0.29 and probability of playing is 0.64.

![naive bayes, probability, example](https://github.com/NeerajHazarika/Email-Spam-Detection-using-ML/blob/main/READ%20ME%20IMG/Bayes_41.png)

Step 3: Now, use Naive Bayesian equation to calculate the posterior probability for each class. The class with the highest posterior probability is the outcome of prediction.

Problem: Players will play if weather is sunny. Is this statement is correct?

We can solve it using above discussed method of posterior probability.

P(Yes | Sunny) = P( Sunny | Yes) * P(Yes) / P (Sunny)

Here we have P (Sunny |Yes) = 3/9 = 0.33, P(Sunny) = 5/14 = 0.36, P( Yes)= 9/14 = 0.64

Now, P (Yes | Sunny) = 0.33 * 0.64 / 0.36 = 0.60, which has higher probability.

Naive Bayes uses a similar method to predict the probability of different class based on various attributes. This algorithm is mostly used in text classification and with problems having multiple classes.

# Reference

* https://www.analyticsvidhya.com/blog/2017/09/naive-bayes-explained/
* https://www.geeksforgeeks.org/naive-bayes-classifiers/
* https://towardsdatascience.com/naive-bayes-classifier-81d512f50a7c
