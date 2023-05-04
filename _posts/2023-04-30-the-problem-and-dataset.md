### The Problem and Dataset

The dataset I am working with for my Capstone Project is from Kaggle and contains transactions made by credit cards in September 2013 by European cardholders. In total, there were 284,807 transactions, out of which 492 were fraudulent. This makes the dataset highly unbalanced, with fraudulent occurrences accounting for roughly 0.2% of all transactions.

The dataset is composed of only numerical input variables resulting from a PCA transformation. Unfortunately, due to confidentiality issues, they could not provide the original features or any more background information about the data. In the dataset, features V1, V2, … V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'. Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset. The feature 'Amount' is the transaction Amount, this feature can be used for example-dependant cost-sensitive learning.

![Screenshot 2023-05-03 232414](https://user-images.githubusercontent.com/132291092/236112277-56f675b1-7162-46d1-bb51-071f135194c8.jpg)

The response variable in this dataset is 'Class,' which takes on a value of 1 in case of fraud and 0 for genuine transactions. This variable is what I am trying to predict using an appropriate model(s). Working with an unbalanced dataset presents unique challenges, and I must utilize techniques that are specifically designed to handle such scenarios. The dataset presents a unique challenge that requires me to employ special techniques to handle the imbalance accurately in order to predict genuine or fraudulent transactions. My goal is to select an appropriate model that can accurately detect fraudulent credit card transactions based on the given data. 

