## 1.2 Basic Classification and Regression

## Study Guide

After the reading you should be able to:

- explain how to choose the “k” in k-nearest neighbors.
- explain why it is an issue if the nearest neighbor is far away.
- explain which error function is minimized in linear regression, and why it is chosen.

### Pre-Class Work Guide

Feel free to adapt code that you have found on the internet to answer these questions, but make sure that you understand every line. Here are some links to help you with today's pre-class work:

- [An introduction to machine learning with scikit-learn](https://scikit-learn.org/stable/tutorial/basic/tutorial.html)
- [Recognizing hand-written digits](http://scikit-learn.org/stable/auto_examples/classification/plot_digits_classification.html)
- [Nearest Neighbors Classification](https://scikit-learn.org/stable/auto_examples/neighbors/plot_classification.html)
- [Linear Regression Example](http://scikit-learn.org/stable/auto_examples/linear_model/plot_ols.html)

In general, [scikit-learn.org](http://scikit-learn.org/) is a great resource that you should use!

## Pre-class work

### 1. Moore's Law

Use the scripts from [here](https://github.com/preshing/analyze-spec-benchmarks) to download a large amount of data relating to CPU specs. The scripts might take as long as an hour, depending on your connection speed. (Pay attention to the line "If you want to skip the steps in this section, you can simply download the aggregated result files from http://preshing.com/files/specdata20120207.zip and extract them to this folder." This will be faster and save you some troubles while providing the same dataset.)

This will save the data in the following format:

| `testid`               | `benchName`   | `base` | `peak` |
| ---------------------- | ------------- | ------ | ------ |
| `cpu95-19990104-03254` | `101.tomcatv` | `19.4` | `27.1` |
| `cpu95-19990104-03254` | `102.swim`    | `27.2` | `34.8` |
| `cpu95-19990104-03254` | `103.su2cor`  | `10.1` | `9.98` |
| `cpu95-19990104-03254` | `104.hydro2d` | `8.58` | `8.61` |

Now do the following:

- Extract the date and base speed for a benchmark of your choice.
- Plot the data in a semi-log plot.
- Now train a linear model to fit your plot.
- How well is Moore's Law holding up?

### 2. MNIST Digits

No machine learning course would be complete without using the MNIST dataset. This dataset was a hugely influential dataset of handwriting digits (0-9). 

- Using scikit-learn, load the MNIST digits (see [here](http://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_digits.html#sklearn.datasets.load_digits)).
- Plot some of the examples. 
- Choose two digit classes (e.g. 7s and 3s), and train a k-nearest neighbor classifier.
- Report your error rates on a held out part of the data. 
- (_optional_) Test your model on the full dataset (available from [here](http://yann.lecun.com/exdb/mnist/)).

Keep a record of your figures and results, and make sure that they are easily accessible when you come to class (e.g. be able to state your error rate, or paste your code/figure into a group doc.)
