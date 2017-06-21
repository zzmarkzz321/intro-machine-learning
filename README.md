# Machine Learning Practice

## intro-machine-learning: Rithm School intro
Introduction to machine learning through different resources.
I will record my journey to learning ML here. 

## History of Machine Learning:
min-max algorithm

Need good amount of data before trying to solve problem with Machine Learning

Vocabulary:
- Features: the data set (not the numbers, but what the data represents. IE: sepal Length = 10, sepal width = 5, etc)
- Class: classification/label of the data
- M = number of examples in the data set
- n = number of features in a given example
- training set: a group of data used to generate the function 

## ML Methods
### Supervised Learning:
    machine learning task of inferring a function from labeled training data.

    Mortgage Example.

### Unsupervised Learning:
    No more labels, just data.

    Credit Card Anomaly Detection Example.

### Reinforcement Learning:
    learning in an environment where the label is delayed or delivered over time
    (hot)

## What do you need to know for machine learning:
1. Calculus
2. Linear Algebra
    - matrix multiplications
3. Programming Language (python)

## Supervised learning (in detail):

Regression (predicting real numbers) vs Classification (preficting a finite set of classes)

Predicting a real value y, given a data point x (predicting a line)

```plaintext
y = theta0 + theta1 * X1
```

[Stack overflow](https://stackoverflow.com/questions/12146914/what-is-the-difference-between-linear-regression-and-logistic-regression)

### Linear Regression:

#### Cost Function:
The "margin of error"
Algorithm: take all data points, plug into algorithm, subtract differnce, square it

j(theta0, theta1) = 1/2m * sum(h(X) - y)^2 

#### Cost Function - visualization:
want cost function to be convex (a global minima)

Want to design an algorithm that results in a convex graph to easily solve for the **global** minima 

**Gradient Decent**: used in a lot of places (look into this). Applies to deep learning, neural networks, etc. Applies on a cost function, to find a better hypothesis.

```plaintext
theta1 = theta0 - alpha * d/dtheta * J(theta0)
```

Theta just changes X to get a better and better hypothesis 
alpha will determine how fast we increase or decrease the step of our change
- worst case of having a too large alpha would to jump to the opposite and then come back (back and forth)
- worst case of having a too small alpha would be slow computation

### Classification : Logistic regression 
Rather than trying to fit a line to our data set, we want to produce a decision boundry.

Instead of predicting housing prices (regression), we predict whether an email is spam or not. 

The Example:
    imagine a graph of data (# of headers x # of charcters) - cartesian plane
    Instead of predicting a value, we try to fit a line

predicting a class value *y*, given a data point x

```plaintext
htheta(x) = g(theta'x)

z = theta'x

g(z) = 1/1+e^-z
```
where ' is transpose


## Overfitting:
A modeling error which occurs when a function is too closely fit to a limited set of data points. 

Overfitting the model generally takes the form of making an overly complex model to explain idiosyncrasies in the data under study.

**How to avoid overfitting?**
Training vs Testing

Assuming we have M = 100. 
1. Run a test without 30 of the data points
2. After you have your hypothesis, run another test with the 30 points

## Underfitting:
Occurs when a statistical model or machine learning algorithm cannot capture the underlying trend of the data.

Hypothesis is not powerful enough to fit our data

Not enough data could result in underfitting 

## Deep Learning: Neural Networks With Hidden Layers:

[Good Overview](http://machinelearningmastery.com/what-is-deep-learning/)

## Questions:

What is the best case for a function that has a lot of local minimas

## Resources:
https://www.coursera.org/learn/machine-learning
http://www.deeplearningbook.org/
http://www.fast.ai/
http://deeplearning.stanford.edu/tutorial/

## Contact Information:
**Tim Garcia:**
Co-Founder/Lead Instructor at Rithm School
@timgarcia0     tim@rithmschool.com

