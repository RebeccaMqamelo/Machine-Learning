## 2.2 Quantifying Model Quality

## Study Guide

After completing the readings, make sure that you understand the following metrics for regression (and when it is appropriate to use them):

- Mean squared error (MSE)
- Mean absolute error (MAS)
- Median absolute error
- The coefficient of determination (or R²)

And make sure that you understand the following metrics for classification (and when it is appropriate to use them):

- Accuracy
- Precision and recall
- (*optional*) Mutual information

## Pre-class work

### 1. Facebook Regression

We're going to use the same dataset and model from the last seminar (2.1), and use a variety of metrics to quantify the performance of our predictions.

Now using your model, measure its performance on the following metrics:

- Mean squared error (MSE)
- Mean absolute error (MAS)
- Median absolute error
- The coefficient of determination (or R²)

Bring to class any relevant graphs or results that you produce, and be prepared to paste small sections of your code into a poll.



### 2. Casualty Classification

We're going to use the same dataset and model from the last seminar (2.1), and be prepared to paste small sections of your code into a poll.

Now using your model, measure its performance on the following metrics:

- Accuracy
- Precision and recall
- Receiver Operating Characteristic (ROC)
- (*optional*) Mutual information

Bring to class any relevant graphs or results that you produce, and be prepared to paste small sections of your code into a poll.



### 3. (*optional*) Mutual Information of a Classifier

Mutual information is a concept from information theory which tells us about how much information we find out about X on average when we observe the outcome of a correlated variable Y. In a classification task we can then quantify how much we learn about the true state (X) when we observe the output from our model (Y).

**Attempt Exercise 44.1 from:**

*MacKay, D. J. (2003). Information theory, inference, and learning algorithms. Cambridge, UK: Cambridge University Press.*
