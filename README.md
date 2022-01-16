# Prediction-of-Heart-Failure-Using-a-Combination-of-Machine-Learning-AutoML
The correct prediction of heart disease can prevent life threats, and incorrect prediction can prove to be fatal at the same time. In this paper different machine learning algorithms and H20 AutoML are applied to compare the results and analysis of the Machine Learning Heart Disease dataset.

## Patients Heart Data Pair Graph
![alt text](https://github.com/dnyanshwalwadkar/Prediction-of-Heart-Failure-Using-a-Combination-of-Machine-Learning-AutoML/blob/main/Model_Results_Images/output.png)

# KNN :
K Nearest Neighbor algorithm falls under the Supervised Learning category and is used for classification (most commonly) and regression. It is a versatile algorithm also used for imputing missing values and resampling datasets. As the name (K Nearest Neighbor) suggests it considers K Nearest Neighbors (Data points) to predict the class or continuous value for the new Datapoint.

## The algorithm’s learning is:

1. Instance-based learning: Here we do not learn weights from training data to predict output (as in model-based algorithms) but use entire training instances to predict output for unseen data.

2. Lazy Learning: Model is not learned using training data prior and the learning process is postponed to a time when prediction is requested on the new instance.

3. Non -Parametric: In KNN, there is no predefined form of the mapping function.

## correlation matrix of Patient Features

A correlation matrix is a table showing correlation coefficients between variables. Each cell in the table shows the correlation between two variables. A correlation matrix is used to summarize data, as an input into a more advanced analysis, and as a diagnostic for advanced analyses.

![alt text](https://github.com/dnyanshwalwadkar/Prediction-of-Heart-Failure-Using-a-Combination-of-Machine-Learning-AutoML/blob/main/Model_Results_Images/Correlation_HeatMap.PNG)


## How to choose the value for K?
K is a crucial parameter in the KNN algorithm. Some suggestions for choosing K Value are:

1. Using error curves: The figure below shows error curves for different values of K for training and test data.
2.  Also, domain knowledge is very useful in choosing the K value.

3. K value should be odd while considering binary(two-class) classification.

![alt text](https://github.com/dnyanshwalwadkar/Prediction-of-Heart-Failure-Using-a-Combination-of-Machine-Learning-AutoML/blob/main/Model_Results_Images/KNN_Optimization.PNG)

# AutoML: Automatic Machine Learning

### What is Auto ML?
Automated Machine Learning (AutoML) is the process of automating tasks in the machine learning pipeline such as data preprocessing, hyperparameter tuning, model selection and evaluation. In this article we will examine how to utilize open source automated machine learning package from H2O to accelerate a Data Scientist’s model development process.


## Introduction
H2O is a fully open-source, distributed in-memory machine learning platform with linear scalability. H2O supports the most widely used statistical & machine learning algorithms, including gradient boosted machines, generalized linear models, deep learning, and many more. AutoML is a function in H2O that automates the process of building a large number of models, with the goal of finding the “best” model without any prior knowledge or effort by the Data Scientist.

The current version of H2O AutoML trains and cross-validates a default Random Forest, an Extremely-Randomized Forest, a random grid of Gradient Boosting Machines (GBMs), a random grid of Deep Neural Nets, a fixed grid of GLMs, and then trains two Stacked Ensemble models at the end. One ensemble contains all the models (optimized for model performance), and the second ensemble contains just the best performing model from each algorithm class/family (optimized for production use).

Automated Machine Learning (AutoML) is the process of automating the end-to-end process of applying machine learning to real-world problems. In a typical machine learning application, the typical stages (and sub-stages) of work are the following:

* Data preparation
* data pre-processing
* feature engineering
* feature extraction
* feature selection
* Model selection
* Hyperparameter optimization (to maximize the performance of the final model)

![alt text](https://github.com/dnyanshwalwadkar/Prediction-of-Heart-Failure-Using-a-Combination-of-Machine-Learning-AutoML/blob/main/Model_Results_Images/H20_Results.PNG)

## Report

![alt text](https://github.com/dnyanshwalwadkar/Prediction-of-Heart-Failure-Using-a-Combination-of-Machine-Learning-AutoML/blob/main/Model_Results_Images/AutoML_Report.PNG)





