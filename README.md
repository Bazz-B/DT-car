# Predict safety of car using Decision Tree
Using Decision Tree on Classification

Based on the data set we want to predict the safety of the car
1. Import Library
   
2. Load Data
   
3. Find Feature Selection. Since we want to predict the safety of the car
   
   X = The feature 

   Y = Target variable which are 'class'
   
5. Split X and Y into training and testing sets
   
   We are using 80% dataset as training and 20% dataset as testing
   
   X_train, X_test, y_train, y_test = train_test_split(X, y, test_size = 0.2, random_state = 42)

7. Build Decision Tree Model

   5.1 criterion='gini'
   
   5.2 train Decision Tree Classifer
   
   5.3 predict the response for test dataset

9. Evaluate model by checking the accuracy score

   print('Model accuracy score with criterion gini index: {0:0.4f}'. format(accuracy_score(y_test, y_pred_gini)))

7. Visualize the model using graphviz

8. Optimize decision tree performance with criterion = 'entropy'

   8.1 criterion='entropy'
   
   8.2 train Decision Tree Classifer
   
   8.3 predict the response for test dataset

10. Visualize the 'Pruned' decision tree.

# Result and Conclusion

1.   I constructed a Random Forest Classifier to forecast the safety level of the car. Two models were developed, one employing the 'gini' criterion and the other utilizing the 'entropy' criterion.
2.   The accuracy of the model using the 'gini' criterion is 0.8025, while the accuracy using the 'entropy' criterion is also 0.8025. This indicates that even after pruning, the accuracy remains consistent across both models.
3.   Consequently, we conducted a confusion matrix and classification report to visualize the model's performance. The model achieved an accuracy of 0.82.
