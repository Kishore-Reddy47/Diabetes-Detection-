# Diabetes-Detection-
 A machine learning project to predict diabetes using a dataset of health metrics. The data is cleaned by handling missing values, removing outliers, and duplicates. Features are standardized, and an SVM model with a linear kernel is trained. The model achieves high accuracy and can predict diabetes for new inputs.


This project involves developing a predictive model to detect diabetes using machine learning techniques. The dataset used for training and evaluation contains various health-related attributes. The project follows a structured approach:

1)Data Preprocessing:

Loaded a dataset (diabetes.csv) using pandas.
Handled missing values and removed outliers using the IQR (Interquartile Range) method.
Removed duplicate entries to clean the dataset.
Standardized the data using StandardScaler to normalize features.

2)Model Development:

Split the data into training and testing sets using train_test_split from sklearn.
Built a Support Vector Machine (SVM) model with a linear kernel.
Trained the SVM model on the training set and evaluated its performance using accuracy scores on both training and test data.

3)Model Evaluation:

Achieved accuracy scores for training and testing datasets, indicating the model’s performance.
Used the trained model to make predictions on new input data, determining whether a person is diabetic based on specific health metrics.

4)Predictive System:

Developed a system to input new health data, standardize it, and predict the likelihood of diabetes.
