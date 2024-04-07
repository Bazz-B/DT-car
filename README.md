# DT-car

# Using Decision Tree on Classification

Based on the data set we want to predict the cafety of the car
1. Import Library
   
2. Load Data
   
3. Find Feature Selection. Since we want to predict the safety of the car
   
   X = The feature 
   Y = Target variable which are 'class'
   
4. Split X and Y into training and testing sets
   
   We are using 80% dataset as training and 20% dataset as testing
   X_train, X_test, y_train, y_test = train_test_split(X, y, test_size = 0.2, random_state = 42)

5. Build Decision Tree Model

   5.1 criterion='gini'
   5.2 train Decision Tree Classifer
   5.3 predict the response for test dataset

6. Evaluate model by checking the accuracy score

  print('Model accuracy score with criterion gini index: {0:0.4f}'. format(accuracy_score(y_test, y_pred_gini)))

7. Visualize the model using graphviz

8. Optimize decision tree performance with criterion = 'entropy'

   8.1 criterion='entropy'
   8.2 train Decision Tree Classifer
   8.3 predict the response for test dataset

9. Visualize the 'Pruned' decision tree.

# Result and Conclusion

1. I build a Random Forest Classifier to predict the safety of the car. I build two models, one with criterion = 'gini' and criterion = 'entropy'.
2. The model accuracy for gini impurity is 0.8024602026 while entropy impurity is 0.8024602026. This shows, even after pruned the accuracy is same.
3. Thus we preform a confusion matrix and classification report to visualize the model performance. The model accuracy is 0.82
