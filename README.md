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
To overcome underfitting we have to increase the degree d of the polynomial predictive function. The training error will tend to decrease. Also the cross validation error will tend to decrease forming a convex curve.<br>
To overcome overfitting we can use regularization techniques. There are three types L1, L2 regularization and Elastic Net. L1 adds absolute value of magnitude to the cost function. L2 adds squared magnitude to the cost function. Elastic Net implements both Lasso and Ridge together. 
#### 4. How do you combat the curse of dimentionality?
When the dimensionality increases the volume of the space increases exponentially. To support the complex model the more data you need. To solve this problem I would change the algorithm (use RNNs) or reduce the dimentionality of my data. It is explained in question number 9.
#### 5. What is regularization and why do we need it? What are some common methods?
We need them to overcome over and underfitting explained in question number 3.
#### 6. Explain Principal Component Analysis(PCA)?
PCA is a technique used to emphasize variation and bring out strong patterns in a dataset and also easy to visualize. We find principal components by finding the most fitting axis using SVM. Then calculate the sum of squared distances for all the data point for each principal component and find the variance and reliability of the dataset.
#### 7. Why is ReLU better and more often used than Sigmoid in Neural Networks?
There are two major benefits of ReLUs. It has sparsity and reduced likelihood of vanishing gradient. When relu's input value is bigger than 0 gradient of relu is a constant value. In contrast gradient of sigmoid becomes increasingly small as the absolute value of the input increases. Also sparsity arises when input is same or smaller than 0 which is beneficial than dense representation.
#### 8. What is data normalization and why do we need it?
Data normalization is used to rescale values to fit in a specific range to assure better convergence during backpropagation. In general you subtract the mean of each data point to center the dataset to 0 and devide by its standard deviation. This is to make all the features have similar magnitude and have bigger learning rates to converge faster.
#### 9. Explain dimentionality reduction, where it's used and its benefits?
Dimentionality reduction is the process to reduce the number of features variables under consideration by obtaining a set of principal variables(important features). The importance of a feature depends on how much it contributes to the information representation of the data. Benefits are (1) more storage space (2) speed up computation (3) remove redundant features (4) easy plotting (5) reduce overfitting. <br>
Types of dimentionality reduction techniques
1. Singular Value Decomposition (Usually this would work)
2. Feature Selection Algorithms
3. Non-Linear Dimentionality reduction methods ISOMAP, Laplacian, Eigenmaps, MDS
4. Feature Hahsing / Random Projections
5. Clustering via K-Means and keep the distance to k centroids for k dimensions.
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