![alt text](https://github.com/shashanksharad/AccordiLytics/blob/master/Icon.png)
# AccordiLytics 
A simple windows based software to perform exploratory data analysis, dimensionality reduction and predictive modeling. This software enables users to generate &amp; visualize feature statistics, class distributions, feature cross-plots, correlations, principal components and confusion matirx.
It uses Accord.NET framework for performing machine learning & statistics operations and derives its name from same.

# Installing
To install AccordiLytics simply download and run the Setup.msi file and follow the instructions. .NET 4.6+ is required.

# Sample Project

Let's follow the step by step guide to create a machine learning supervised classification model in AccordiLytics. The data used here is the famous breast cancer diagonistic dataset available at this [UCI ML Repository](http://archive.ics.uci.edu/ml/datasets/breast+cancer+wisconsin+%28diagnostic%29). 
The same data is already available as train and test sets in this repository.

# User Interface
The input data is required to be imported in csv format for each of the training and the test sets. Each feature column should have corresponding header and class data should be the last column. The classes should be numeric and mandatorily starting from 0 and subsequently increasing by 1. The import buttons followed by Load Data button create the essential data structures to be used for further operations.

![alt text](https://github.com/shashanksharad/AccordiLytics/blob/master/UI.PNG)

# Descriptive Statistics
Once the training and test data are loaded, user can generate the descriptive statistics comprising of the sample count, mean, standard deviations, minimum and maximum for each of the features. Additionally the class distribution is also generated to evaluate the cases of class imbalance prior to modeling.
![alt text](https://github.com/shashanksharad/AccordiLytics/blob/master/DescStats.PNG)

# Feature Crossplots
In order to evaluate the presence a good or bad correlation between the input features, it automatically transforms the feature data to their Standard scores and hence have zero mean and unit variance. The features are then cross-plotted taken two at a time. The crossplot points are also colored based on their class. It also gives the histogram distribution of individual features plotted along the diagonal.
![alt text](https://github.com/shashanksharad/AccordiLytics/blob/master/Xplots.PNG)

# Feature Correlations Heatmap
To further quantify the level of correlations between the features, it creates heatmap of their Pearson correlation coefficients.
![alt text](https://github.com/shashanksharad/AccordiLytics/blob/master/Correlations.PNG)

# Principal Component Analysis: Compute and Visualize
AccordiLytics lets you compute the principal components of the feature data in order to utilize transformed input feature data in variance maximized domain. The principal components are dumped in a sheet format with additional useful informations such as their proportions, cumulative proportions, singular values, eigenvalues and eigen-vectors. It also provides users with excellent component visualization in the form of pie chart(pie chart) and cumilative function( cumulative proportion).
![alt text](https://github.com/shashanksharad/AccordiLytics/blob/master/PCA.PNG)

# Machine Learning Model Training and Estimation
Once the user has performed necessary exploratory data analysis and dimensionality reduction operations, he/she can start building the supervised classification model. AccordiLytics lets user select either all the feature data or a number of principal components to be used for machine learning training stage. User can also define the fold of cross validation scheme used to test the model at each training iteration. 

![alt text](https://github.com/shashanksharad/AccordiLytics/blob/master/Model_Before.PNG)

Currently only Random Forest classification algorithm has been included in the algorithms list and Deep Neural Networks will be implemented in the next release. User can select the Random Forest parameters and click the Run model button. This step in background builds a classification model using random forest algorithm following the specified fold cross-validation scheme. The same model is then used to predict target class of the test data.

# Model Evaluation-Confusion Matrices
Once the software has learned the feature-class relationship in the training data, it automatically applies it to both the training and  test data to predict the target classes. To evaluate the accuracy and generalization of the learnt classification model the predicted classes are compared with the true classes in the form of a Confusion Matrix. It shows the proportion of samples correctly classified as well as proportion of samples wrongly classified. The Precision, Recall and F-Scores of each of the classes are also populated to represent the single number model evaluation metric.
![alt text](https://github.com/shashanksharad/AccordiLytics/blob/master/Model_After.PNG)

# Export Predictions
Once the training and estimation process is complete, users can also export the test data prediction in csv format

# Contributing
Users interested in contributing to this project can request the source code at shashank.sharad@gmail.com.
