Credit Card Fraud Detection ML Project:

Project Overview
Credit card fraud is a significant issue that impacts both consumers and financial institutions, leading to financial losses and damage to trust. 
Detecting fraudulent transactions efficiently is crucial, and machine learning has proven to be an effective approach for this. In this project, 
I used logistic regression to build a model that classifies transactions as either legitimate or fraudulent based on their features.

Dataset Details
The dataset used for this project is in CSV format and contains 284,807 transaction records across 31 columns. 
The target variable, labeled "Class," indicates whether a transaction is legitimate (Class = 0 denotes legitimate) or fraudulent 
(Class = 1 denotes fraud).This dataset provides a robust foundation for training and evaluating the fraud detection model.

Preprocessing
To get started, we first need to clean and prepare the data. We separate the legitimate transactions from the fraudulent ones. 
The dataset is highly imbalanced, with a lot more legitimate transactions compared to fraudulent ones, so we need to balance it out. 
To do this, we perform undersampling, which means reducing the number of legitimate transactions to make the classes more balanced.
After this, we split the data into training and testing sets using the train_test_split() function from scikit-learn.

Model
For this project, we chose logistic regression to classify transactions as legitimate or fraudulent based on their features. 
Logistic regression is a popular and simple classification algorithm that works by estimating the probability of an event happening based on input features. 
We train the model using the LogisticRegression() function from scikit-learn on our training data. 
Once trained, the model is used to predict whether the transactions in the testing set are legitimate or fraudulent.

Evaluation
To check how well our model is performing, we use the accuracy metric, which tells us the percentage of transactions that were classified correctly.
We calculate the accuracy for both the training and testing data using the accuracy_score() function from scikit-learn.

Conclusion
In this project, we used logistic regression to detect fraudulent credit card transactions. 
We achieved a high accuracy on both the training and testing data, indicating that the model is effective at detecting fraudulent transactions. 
The Streamlit application provides an easy-to-use interface for detecting fraudulent transactions in real-time.
