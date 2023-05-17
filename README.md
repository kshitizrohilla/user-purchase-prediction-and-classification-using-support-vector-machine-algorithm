# User Purchase Classification Prediction using SVM
This project implements the Support Vector Machine (SVM) algorithm for predicting user purchase classification. It utilizes the user-data.csv dataset, which contains information about users and their purchase behavior. The goal is to train an SVM classifier to predict whether a user will purchase a particular product or not.

## Data Pre-processing Step
The first step in the project is data pre-processing. The user_data.csv file is imported using the Pandas library, and the independent variables (features) and the dependent variable (target) are extracted from the dataset. The dataset is then split into training and test sets using the train_test_split function from the sklearn.model_selection module. Feature scaling is performed using the StandardScaler class from the sklearn.preprocessing module.

## SVM Algorithm
The SVM algorithm is implemented using the SVC (Support Vector Classifier) class from the sklearn.svm library. In this project, a linear kernel is used to create the SVM classifier for linearly separable data. The classifier is trained on the training set using the fit method.

## Predicting the Test Set Result
The trained SVM classifier is used to predict the output for the test set. The predict method is used to obtain the predicted values, which are stored in the y_pred vector. The predicted values can be compared with the actual values (y_test) to evaluate the performance of the classifier.

## Confusion Matrix
The performance of the SVM classifier is evaluated by creating a confusion matrix. The confusion_matrix function from the sklearn.metrics module is used to generate the confusion matrix. It takes the actual values (y_test) and the predicted values (y_pred) as parameters.

## Visualizing the Training Set Result
The training set result is visualized using the contourf and scatter functions from the matplotlib.pyplot module. The contourf function is used to create a filled contour plot, representing the decision boundary of the SVM classifier. The scatter function is used to plot the data points, with different colors representing different classes. The plot is labeled with appropriate titles, axis labels, and legends.

## Visualizing the Test Set Result
The test set result is visualized in a similar manner as the training set result. The contourf and scatter functions are used to create the filled contour plot and plot the data points, respectively. The plot is labeled with appropriate titles, axis labels, and legends.

## Conclusion
The SVM classifier successfully predicts user purchase classification based on the provided dataset. The project demonstrates the use of SVM algorithm for binary classification tasks and provides visualizations of the decision boundary and class separation.

## Dependencies
The following Python libraries are used in this project:

* numpy
* matplotlib.pyplot
* pandas
* sklearn.model_selection
* sklearn.preprocessing
* sklearn.svm
* sklearn.metrics