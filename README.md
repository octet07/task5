# Heart Disease Prediction - Decision Tree and Random Forest Analysis

This project involves analyzing a heart disease dataset to build and evaluate classification models. The primary objective was to apply machine learning algorithms like Decision Trees and Random Forests to predict the presence of heart disease, and to interpret the performance and behavior of these models using visualization and evaluation techniques.

## 1. Train a Decision Tree Classifier and Visualize the Tree

The dataset was first loaded and preprocessed to define features and the target variable. A Decision Tree Classifier was trained on the data using the training set. The resulting decision tree structure was visualized to understand the splits made by the model based on feature thresholds. This step provided insights into how the model makes predictions and which features are considered most important in early splits.

## 2. Analyze Overfitting and Control Tree Depth

To study the problem of overfitting, decision trees were trained with different values of `max_depth`. The training and testing accuracies were recorded and plotted against the tree depth. This allowed the identification of the point at which the model starts to overfit the training data — where training accuracy remains high while testing accuracy begins to drop. An optimal depth was selected to balance bias and variance.

## 3. Train a Random Forest and Compare Accuracy

A Random Forest Classifier was trained using the same training data. Accuracy scores were calculated for both the training and testing sets and compared with those of the Decision Tree. The Random Forest model demonstrated improved generalization and better test accuracy, due to its ensemble nature and ability to reduce overfitting by aggregating multiple decision trees.

## 4. Interpret Feature Importances

The feature importances from the trained Random Forest model were extracted and visualized. This helped determine which input features had the most influence on the model’s predictions. A ranked bar chart was plotted to show the relative importance of each feature, highlighting the top contributors to heart disease prediction.

## 5. Evaluate Using Cross-Validation

To ensure robust evaluation, 5-fold cross-validation was performed on both the Decision Tree and Random Forest classifiers. The mean accuracy and standard deviation across the folds were reported. Cross-validation helped assess the models’ performance across multiple train-test splits and provided a better estimate of their generalization capability.

---

**Conclusion:**  
This workflow demonstrated the complete process of training, evaluating, and interpreting decision tree-based models for classification. The Random Forest classifier proved to be more stable and accurate than the standalone Decision Tree, especially when evaluated through cross-validation and feature importance analysis.
