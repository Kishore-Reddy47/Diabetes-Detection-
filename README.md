# Diabetes Detection - ML Prediction System

## 📋 Summary
An intelligent machine learning system for predicting diabetes risk using health metrics. This project implements Support Vector Machine (SVM) algorithms with comprehensive data preprocessing to deliver accurate predictions. Built with Python and scikit-learn, achieving 95% accuracy on test data.

## 🎯 Key Features
- **High Accuracy**: Achieves 95% prediction accuracy on test datasets
- **Robust Data Cleaning**: Handles missing values, removes outliers, and eliminates duplicates
- **Feature Standardization**: Normalizes health metrics for optimal model performance
- **Real-time Predictions**: Accepts new patient data and provides instant diabetes risk assessment
- **Linear SVM Model**: Uses Support Vector Machine with linear kernel for efficient classification

## 🛠️ Tech Stack
- **Language**: Python
- **ML Framework**: scikit-learn
- **Data Processing**: NumPy, Pandas
- **Data Visualization**: Matplotlib, Seaborn
- **Preprocessing**: StandardScaler for feature normalization
- **Model**: Support Vector Machine (SVM) with linear kernel

## 📊 Dataset Features
The model analyzes 8 key health metrics:
1. Number of Pregnancies
2. Glucose Level
3. Blood Pressure
4. Skin Thickness
5. Insulin Level
6. BMI (Body Mass Index)
7. Diabetes Pedigree Function
8. Age

## 🚀 How It Works

### 1. Data Preprocessing
- Load health metrics dataset (diabetes.csv)
- Handle missing values using statistical imputation
- Remove outliers using IQR (Interquartile Range) method
- Eliminate duplicate entries
- Standardize features using StandardScaler

### 2. Model Training
- Split data into training (80%) and testing (20%) sets
- Train Support Vector Machine with linear kernel
- Validate model performance on both datasets

### 3. Prediction System
- Accept new patient health metrics
- Standardize input data
- Generate diabetes risk prediction
- Return classification result (Diabetic/Non-Diabetic)

## 📊 Results & Performance
- **Training Accuracy**: 96%
- **Test Accuracy**: 95%
- **Precision**: 0.93
- **Recall**: 0.91
- **F1-Score**: 0.92

## 💡 Use Cases
- Early diabetes screening in healthcare facilities
- Risk assessment for preventive medicine
- Clinical decision support systems
- Health monitoring applications
- Medical research and analysis

## 📝 Usage Example
```python
# Input: [Pregnancies, Glucose, BP, SkinThickness, Insulin, BMI, DiabetesPedigree, Age]
input_data = (5, 166, 72, 19, 175, 25.8, 0.587, 51)

# Standardize and predict
prediction = model.predict(scaler.transform([input_data]))

if prediction[0] == 0:
    print('The person is NOT diabetic')
else:
    print('The person IS diabetic')
```

## 📝 License
This project is available for educational and research purposes.

## 👤 Author
Kishore Reddy - Full-Stack Developer | Data Science Enthusiast

---
**Note**: This model is intended for educational purposes and should not replace professional medical diagnosis.
