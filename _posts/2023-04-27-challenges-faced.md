### Challenges Faced

Throughout this project, my goal was to train and evaluate models for detecting fraudulent credit card transactions. I judged the suitability of each model by analyzing the accuracy score as well as other performance metrics after making adjustments. To start, I began by undersampling to account for the datasets' imbalance. In the original dataset, genuine cases accounted for nearly 99.8% of all transactions. Prior to undersampling, the accuracies for each of the four classifiers were high, above 0.9, but the other performance metrics did not show that the models performed well. After undersampling, all values, including the performance metrics, were over 0.9.

Another challenge I faced was choosing an appropriate test size that would yield accurate results. I chose a 20-30% range since a smaller test size may result in unreliable estimates of model performance. I tried 20% and 30%, but I found that 20% yielded better, more accurate results (above 0.9).

The last challenge I faced was scaling the dataset. I chose two scaling methods: StandardScaler and MinMaxScaler. After experimenting with both, I did not find a significant change in results for the logistic regression and decision tree classifiers, so I did not use the scaled dataset with those two. On the contrary, the StandardScaler data was instrumental in improving the performance of the other two classifiers: perceptron and SVM.

Overall, this project allowed me to experiment with different methods to obtain better and more accurate results in order to choose the best models with the most appropriate dataset alterations.
