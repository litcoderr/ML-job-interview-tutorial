# ML job interview tutorial
This tutorial is for those who have no idea how to prepare for machine learning job interview. This repository contains general interview questions and answers. Please contribute with more questions and answer corrections.

### Contents
1. [General Questions](#general-questions)

### Reference
1. [Data Science and Machine Learning Interview Questions](https://towardsdatascience.com/data-science-and-machine-learning-interview-questions-3f6207cf040b)

## General Questions
#### 1. What is gradient descent?
#### 2. What's the trade-off between bias and variance?
#### 3. Explain over and under fitting and how to combat them?
#### 4. How do you combat the curse of dimentionality?
#### 5. What is regularization and why do we need it? What are some common methods?
#### 6. Explain Principal Compponent Analysis(PCA)?
#### 7. Why is ReLU better and more often used than Sigmoid in Neural Networks?
#### 8. What is data normalization and why do we need it?
Data normalization is used to rescale values to fit in a specific range to assure better convergence during backpropagation. In general you subtract the mean of each data point to center the dataset to 0 and devide by its standard deviation. This is to make all the features have similar magnitude and have bigger learning rates to converge faster.
#### 9. Explain dimentionality reduction, where it's used and its benefits?
Dimentionality reduction is the process to reduce the number of features variables under consideration by obtaining a set of principal variables(important features). The importance of a feature depends on how much it contributes to the information representation of the data. There are linear and non linear techniques. Benefits are (1) more storage space (2) speed up computation (3) remove redundant features (4) easy plotting (5) reduce overfitting.

