# Bayesian-Classifier

Implemented a Bayesian Classifier using Bayes Theorem for five different classes(continuous features -- Z-score and Gaussian Normal Distribution) on the available dataset using Python, Numpy, Pandas, Matplotlib.

This is based on the Bayes theorem to find the probability of any class given some information.

### Z-Score

A z-score describes the position of a raw score in terms of its distance from the mean, when measured in standard deviation units. The z-score is positive if the value lies above the mean, and negative if it lies below the mean.

It is also known as a standard score, because it allows comparison of scores on different kinds of variables by standardizing the distribution. A standard normal distribution is a normally shaped distribution with a mean of 0 and a standard deviation of 1.

It is useful to standardized the values of a normal distribution by converting them into z-scores because:
- It allows researchers to calculate the probability of a score occurring within a standard normal distribution;
- Enables us to compare two scores that are from different samples.

The formula for calculating a z-score is is z = (x-μ)/σ, where x is the raw score, μ is the population mean, and σ is the population standard deviation.

### Gaussian Naive Bayes

When the predictors take up a continuous value and are not discrete, we assume that these values are sampled from a gaussian distribution. 

![alt text](https://github.com/aadlakha12/Bayesian-Classifier/blob/master/Images/gd.gif?raw=true)

The conditional probability formula for continuous value gets changed to,

![alt text](https://github.com/aadlakha12/Bayesian-Classifier/blob/master/Images/Pdf.png?raw=true)

### Multinomial Naive Bayes

When the predictors take up a discrete values.

![alt text](https://github.com/aadlakha12/Bayesian-Classifier/blob/master/Images/bayes.png?raw=true)

P(y|X) - Probability of event y happens given that event X happens which is also known as Prosterior Probability.

P(X|y) - Probability of event X happens given that event y happens which is also known as Likelihood.

P(y) - Probability of event A which is known as Prior Probability.

P(X) - Probability of event B which is Evidence.

![alt text](https://github.com/aadlakha12/Bayesian-Classifier/blob/master/Images/features.png?raw=true)

X represents features/predictors. They are mapped to the features in the dataset.

By substituting for X and expanding using the chain rule we get,

![alt text](https://github.com/aadlakha12/Bayesian-Classifier/blob/master/Images/naive_features.png?raw=true)

We can obtain the values for each by looking at the dataset and substitute them into the equation. For all entries in the dataset, the denominator does not change, it remain static. Therefore, the denominator can be removed and a proportionality can be introduced.

![alt text](https://github.com/aadlakha12/Bayesian-Classifier/blob/master/Images/pr.png?raw=true)

To find the class y with maximum probability, we the below function, and we can obtain the class, given the predictors.

![alt text](https://github.com/aadlakha12/Bayesian-Classifier/blob/master/Images/arg.png?raw=true)

Prosterior = (Prior*Likelihood)/Evidence.


