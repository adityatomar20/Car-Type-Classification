### Project Overview
In this project, we aim to predict the class of cars using the Car Evaluation Dataset, which consists of six categorical attributes: buying, maintenance, doors, persons, lug_boot, and safety. The goal is to implement and evaluate various classification algorithms to determine the best-performing model for predicting car classes.

### Dataset Description

#### Attributes:

1. buying: v-high, high, med, low
2. maint: v-high, high, med, low
3. doors: 2, 3, 4, 5-more
4. persons: 2, 4, more
5. lug_zoot: small, med, big
6. safety: low, med, high

#### Class Distribution:

1. unacc: 70.02%
2. acc: 22.22%
3. good: 3.99%
4. v-good: 3.76%

### Implementation Steps
#### 1. Data Loading and Preprocessing
We start by loading the Car Evaluation Dataset into a Pandas DataFrame. We then split the data into training and testing sets, using 80% for training and 20% for testing. Additionally, we create one-hot encoded and ordinal encoded versions of the dataset to handle categorical attributes.

#### 2. Model Benchmarking
We establish a benchmark model by predicting everything as the majority class. This simple model serves as a baseline for evaluating the performance of more complex models.

#### 3. Model Evaluation
We implement and evaluate the performance of several classification algorithms, including K-Nearest Neighbors (KNN), Decision Tree, Naive Bayes, Logistic Regression, and Support Vector Classifier (SVC). We conduct hyperparameter tuning using cross-validation and record the Matthews Correlation Coefficient (MCC) as our evaluation metric.

#### 4. Model Selection
We compare the MCC scores of different models and select the one with the highest performance as our final model.

#### 5. Final Model Evaluation
The chosen model, a Support Vector Classifier (SVC), is fitted to the training data and evaluated on the entire dataset, including the test set. We assess metrics such as accuracy, confusion matrix, F-scores, Kappa coefficient, and MCC.

### Results and Conclusion
The final Support Vector Classifier (SVC) demonstrates exceptional performance with an accuracy of 99.65%, high precision, recall, and F-scores for all classes. The MCC of 0.99 indicates that the model significantly outperforms random chance. The confusion matrix provides insights into the classification results for each car class.

### This project showcases the application of machine learning algorithms for car classification, providing a robust and accurate model for predicting car classes based on given attributes.





