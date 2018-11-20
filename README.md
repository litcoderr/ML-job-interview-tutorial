# ML job interview tutorial
This tutorial is for those who have no idea how to prepare for machine learning job interview. This repository contains general interview questions and answers. Please contribute with more questions and answer corrections.

### Contents
1. [General Questions](#general-questions)

### Reference
1. [Data Science and Machine Learning Interview Questions](https://towardsdatascience.com/data-science-and-machine-learning-interview-questions-3f6207cf040b)
2. [Mahchine Learning Interview Questions and Answers](https://www.youtube.com/watch?v=hB1CTizqGFk)

## General Questions
#### 1. What is gradient descent?
Gradient Descent is an iterative optimization algorithm for finding the minimum of a function. To find the local minimum of a function, one takes steps proportional to the negative of the gradient of the function. GD repeats this process util convergence.
#### 2. What's the trade-off between bias and variance?
Bias is the difference between the average prediction and the correct value. Model with high bias pays little attention to the training data and leads to high error on training and test data. <br>
Variance is the variability of model prediction for a given data point. Model with high variance pays a lot of attention to training data and does not generalize which leads to high error rates on test data. <br>
If my model is simple and has very few parameters then it may have high bias and low variance. However if our model has large number of parameters then it's going to have high variance and low bias. So we need to find the right balance without overfitting and underfitting.
#### 3. Explain over and under fitting and how to combat them?
#### 4. How do you combat the curse of dimentionality?
#### 5. What is regularization and why do we need it? What are some common methods?
#### 6. Explain Principal Compponent Analysis(PCA)?
#### 7. Why is ReLU better and more often used than Sigmoid in Neural Networks?
#### 8. What is data normalization and why do we need it?
Data normalization is used to rescale values to fit in a specific range to assure better convergence during backpropagation. In general you subtract the mean of each data point to center the dataset to 0 and devide by its standard deviation. This is to make all the features have similar magnitude and have bigger learning rates to converge faster.
#### 9. Explain dimentionality reduction, where it's used and its benefits?
Dimentionality reduction is the process to reduce the number of features variables under consideration by obtaining a set of principal variables(important features). The importance of a feature depends on how much it contributes to the information representation of the data. There are linear and non linear techniques. Benefits are (1) more storage space (2) speed up computation (3) remove redundant features (4) easy plotting (5) reduce overfitting.
#### 10. How to handle corrupted or missing data?
You could drop the column/row or replace with a placeholder value. Pandas library provides you with isnull() to find null values and dropna() to drop those values. If you want to replace with a placeholder value you can use fillna() function.
#### 11. How would you go about doing an Exploratory Data Analysis?
#### 12. How do you know which machine learning modle you should use?
#### 13. Why do we use Convolutional Layer for images rather than just Fully Connected Layers?
#### 14. What makes CNNs translation invariant?
#### 15. Why do we have max-pooling in classification CNNs?
#### 16. Why do segmentation CNNs typically have and encoder-decoder style structure?
#### 17. What is the significnace of Residual Networks?
#### 18. What is batch normalization and how does it work?
#### 19. How would you handle an imbalanced dataset?
#### 20. Why would you use many small convolutional kernels such as 3x3 rather than a few large ones?
#### 21. Do you have any other projects