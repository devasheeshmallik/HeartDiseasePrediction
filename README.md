# HeartDiseasePrediction

**OBJECTIVES:**
   Is to analyse the sample data set of various people containing attributes such as resting heart rate, age, gender, cholesterol levels, etc. and classify people using these attributed to find whether a person has heart disease or not.

In this notebook, we have prepared two machine learning models: LGBM and MLP classifiers to create prediction algorithms and test their accuracy.


**LGBM Introduction**

Light Gradient Boosting Machine is an open-source gradient boosting framework that uses tree based learning algorithms and is developed by Microsoft. LGBM structure tends to grow with most promising branches and leaves(nodes with the most delta loss), holding the number of the decision leaves constant. (If this doesn’t make sense to you, don’t sweat. This won’t prevent you from effectively using LGBM).

**Advantages of LGBM over other decision tree framework:**
    • Faster training speed with higher accuracy, 
    • Lower memory usage,
    • Better accuracy than any other boosting algorithm specially handles the overfitting very well when working with a small dataset, 
    • Compatibility with large datasets, and
    • Parallel learning support. 
Light GBM is sensitive to overfitting and can easily over-fit small data. 

In this heart diseases classification problem, we have seperated the dataset in ratio 70:30 (i.e., 70% data is in training and 30% data in test the model), implemented a decision tree classifier from scikit learn module with k- fold cross validation. After implementing the decision tree we have enhanced accuracy using the LGBMClassifier. 


**MLPClassifier Introduction**
Multi layer perceptron is a feed forward artificial neural network that generates a set of outputs from a set of inputs. An MLP can be characterized by a series of layers connected as directed graphs between the inputs and the output layers of each other. MLPClassifier is used in different types of classification problems. Since heart disease is a binary classification problem, we have used this classifier to understand the result of the neural network model in this dataset.

We have used the MLPClassifier model from scikit learn and make 2 different models with different learning rate, iterations and hidden layers. 
