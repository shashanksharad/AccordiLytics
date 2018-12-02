![alt text](https://github.com/shashanksharad/AccordiLytics/blob/master/Icon.png)
# AccordiLytics 
A simple windows based software to perform exploratory data analysis, dimensionality reduction and predictive modeling. This software enables users to generate &amp; visualize feature statistics, class distributions, feature cross-plots, correlations, principal components and confusion matirx.
It uses Accord.NET framework for performing machine learning & statistics operations.

# Installing
To install AccordiLytics simply run the attached setup.exe file and follow the instructions.

# Sample Project

Let's follow the step by step guide to create a machine learning supervised classification model in AccordiLytics. The data used here is the famous breast cancer diagonistic dataset available at this [UCI ML Repository](http://archive.ics.uci.edu/ml/datasets/breast+cancer+wisconsin+%28diagnostic%29). 

# User Interface
The input data is required to be imported in csv format for each of the training and the test sets. Each feature column should have corresponding header and class data should be the last column. The classes should be numeric and mandatorily starting from 0 and subsequently increasing by 1. The import buttons followed by Load Data button create the essential data structures to be used for further operations.

![alt text](https://github.com/shashanksharad/AccordiLytics/blob/master/UI.PNG)

# Descriptive Statistics
Once the training and test data are loaded, user can generate the descriptive statistics comprising of the sample count, mean, standard deviations, minimum and maximum for each of the features. Additionally the class distribution is also generated to evaluate the cases of class imbalance prior to modeling. The 
![alt text](https://github.com/shashanksharad/AccordiLytics/blob/master/DescStats.PNG)

# Feature Crossplots
In order to evaluate the presence a good or bad correlation between the input features, it automatically transforms the feature data to their Standard scores and hence have zero mean and unit variance. The features are then cross-plotted taken two at a time. The crossplot points are also colored based on their class. It also gives the histogram distribution of individual features plotted along the diagonal.
![alt text](https://github.com/shashanksharad/AccordiLytics/blob/master/Xplots.PNG)

![alt text](https://github.com/shashanksharad/AccordiLytics/blob/master/Correlations.PNG)

![alt text](https://github.com/shashanksharad/AccordiLytics/blob/master/PCA.PNG)

![alt text](https://github.com/shashanksharad/AccordiLytics/blob/master/Model_Before.PNG)

![alt text](https://github.com/shashanksharad/AccordiLytics/blob/master/Model_After.PNG)
