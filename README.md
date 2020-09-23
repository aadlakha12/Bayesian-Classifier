# Bayesian-Classifier

Implemented a Bayesian Classifier using Bayes Theorem for five different classes(continuous features -- Z-score and Gaussian Normal Distribution) on the available dataset using Python, Numpy, Pandas, Matplotlib.

This is based on the Bayes theorem to find the probability of any class given some information.

Multinomial Naive Bayes

When the predictors take up a discrete values.

P(A|B) =  P(A).P(B|A)/P(B)

P(A|B) - Probability of event A happens given that event B happens which is also known as Prosterior Probability.

P(B|A) - Probability of event B happens given that event A happens which is also known as Likelihood.

P(A) - Probability of event A which is known as Prior Probability.

P(B) - Probability of event B which is Evidence.

B =(b1,b2,b3.....bn)

B represents features/predictors. They are mapped to the features in the dataset.

Prosterior = (Prior*Likelihood)/Evidence.

Gaussian Naive Bayes

When the predictors take up a continuous value and are not discrete, we assume that these values are sampled from a gaussian distribution. 


