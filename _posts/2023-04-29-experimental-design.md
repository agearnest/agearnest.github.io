### Experimental Design

To begin with, I obtained the dataset from Kaggle and conducted a thorough analysis of the provided information. Afterwards, I checked for missing values and discovered zero, hence no need to alter the dataset in that sense. I then assigned the dataset to different variables, with a value of 0 for genuine transactions and 1 for fraudulent transactions. 

![Screenshot 2023-05-03 233302](https://user-images.githubusercontent.com/132291092/236113103-18512a61-3f66-4a2b-9037-e9e6b31d0216.jpg)

I also noted the severe imbalance in the dataset and performed undersampling to ensure a more even distribution, resulting in 492 cases for each class. With undersampling, I eliminated the bias of the majority class, in this case genuine transactions, and created a 50/50 split in the data which will yield better results.

![Screenshot 2023-05-03 233355](https://user-images.githubusercontent.com/132291092/236113169-ad77f984-f871-49e0-a34c-24e6cec5b6bc.jpg)

Following the undersampling, I split and scaled the data, using a 20% test set. Although I experimented with a 30% test set, a 20% test set provided more accurate results. I also tested two different scaling methods, StandardScalar and MinMaxScalar, but did not observe a significant difference in results for two of my classifiers. Hence, I only used the StandardScalar data with perceptron and SVM classifier.

![Screenshot 2023-05-03 233522](https://user-images.githubusercontent.com/132291092/236113426-234d17ea-b10a-4883-801f-d4e2e7cc4c8b.jpg)

Furthermore, I selected four classifiers to see which one would be the best fit. Furthermore, if my results were not satisfactory, I would alter which dataset was utilized to make each classifer well-fit models for my problem and dataset. Logistic regression yeilded accurate results and it is suitable for predicting binary outcomes. As the problem at hand was to detect fraud, i.e., genuine or fraudulent, I needed to predict a binary outcome. In addition, the SVM was also an excellent classifier for the problem and dataset as seen in the table below:

![Screenshot 2023-05-03 233928](https://user-images.githubusercontent.com/132291092/236113810-d33468f6-5de7-4198-b39c-4609d01d9e7e.jpg)

I evaluated the performance of each classifier on the testing set using appropriate performance metrics such as accuracy, precision, recall, and F1 score. After accounting for undersampling, a 20% test size, and occasional scaling, each performance metric utilized resulted in excellent scores above 90%.

In conclusion, based on my analysis of the dataset, including importing data, evaluating missing values, performing undersampling, and splitting and scaling the data, I determined that logistic regression and SVM classifier with undersampling and 20% test set produced the most accurate results and was therefore the best models for detecting fraudulent credit card transactions.
