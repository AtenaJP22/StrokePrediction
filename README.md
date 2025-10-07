# StrokePrediction
Stroke Prediction with Multiple Linear Regression based on the kaggle competition [Stroke Prediction Dataset Assignment](https://www.kaggle.com/competitions/stroke-prediction-dataset-assignment/data?select=submission.csv)

# Stroke Prediction Analysis

A comprehensive machine learning project for predicting stroke risk based on patient health metrics and demographic information.

## 📋 Project Overview

This project analyzes and predicts the likelihood of stroke occurrence using various machine learning models. The implementation includes extensive data preprocessing, exploratory data analysis, feature engineering, and model evaluation to identify key risk factors for stroke.

## 🎯 Objectives

- Perform comprehensive exploratory data analysis on stroke prediction dataset
- Implement multiple machine learning algorithms for stroke prediction
- Handle class imbalance using SMOTE technique
- Evaluate and compare model performance
- Identify key features contributing to stroke risk

## 📊 Dataset

The dataset contains 11 clinical and demographic features:

### Features
- **Demographic**: `id`, `gender`, `age`
- **Health Metrics**: `hypertension`, `heart_disease`, `avg_glucose_level`, `bmi`
- **Lifestyle**: `ever_married`, `work_type`, `Residence_type`
- **Target**: `stroke` (0 = No, 1 = Yes)

### Data Characteristics
- **Total samples**: 5,110
- **Stroke cases**: 249 (4.87%)
- **Missing values**: BMI (201 missing values)

## 🛠️ Installation & Requirements

```bash
pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn
```

## 📁 Project Structure

```
├── AIN2002_Stroke_Predictions.ipynb  # Main Jupyter notebook
├── README.md                         # Project documentation
└── (Dataset file - not included in repo)
```

## 🚀 Implementation

### Data Preprocessing
- Handling missing values in BMI column
- Encoding categorical variables
- Feature scaling and normalization
- Train-test split (80-20)

### Models Implemented
1. **Logistic Regression**
2. **K-Nearest Neighbors (KNN)**
3. **Support Vector Machine (SVM)**
4. **Decision Tree**
5. **Random Forest**
6. **Gradient Boosting**

### Handling Class Imbalance
- **SMOTE (Synthetic Minority Over-sampling Technique)**
- Improves model performance on minority class (stroke cases)

## 📈 Results

### Performance Metrics
Models are evaluated using:
- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC Score

### Key Findings
- Random Forest and Gradient Boosting showed superior performance
- Age, average glucose level, and hypertension are top predictors
- SMOTE significantly improved recall for stroke detection

## 💡 Key Insights

1. **Top Risk Factors**: Age, hypertension, and glucose levels are strongly correlated with stroke risk
2. **Data Imbalance**: Original dataset is highly imbalanced (95% non-stroke vs 5% stroke)
3. **Model Selection**: Ensemble methods outperform single classifiers
4. **Feature Importance**: Clinical features outweigh demographic factors in prediction

## 🎮 Usage

1. Clone the repository
2. Install required dependencies
3. Run the Jupyter notebook sequentially
4. Modify parameters for experimentation
5. View results and visualizations

## 🔧 Customization

- Adjust SMOTE parameters for different sampling strategies
- Modify hyperparameters for each model
- Add new features or preprocessing steps
- Extend with additional machine learning models

## 📝 Future Improvements

- Implement neural networks for comparison
- Add feature selection techniques
- Incorporate cross-validation
- Develop a web application for predictions
- Add explainable AI techniques (SHAP, LIME)

## 👥 Contributors

- [AtenaJP22](https://github.com/AtenaJP22)

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🤝 Contributing

Contributions, issues, and feature requests are welcome. Feel free to check [issues page](https://github.com/AtenaJP22/StrokePrediction/issues) if you want to contribute.

---

**Note**: This project is for educational and research purposes. Always consult healthcare professionals for medical advice.
