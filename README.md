# Heart Disease Classification Project

A machine learning project comparing Logistic Regression and Support Vector Machine (SVM) models for predicting heart disease using patient health data.

## 📋 Project Overview

This project implements and compares two supervised learning algorithms to classify patients as having or not having heart disease based on various medical indicators. The analysis includes data preprocessing, model training, evaluation, and performance comparison.

## 🎯 Objective

- Predict the presence of heart disease (AHD - Angiographic Heart Disease)
- Compare the performance of Logistic Regression vs SVM classifiers
- Identify the most effective model for heart disease prediction

## 📊 Dataset

**Source:** Heart.csv

**Features:**
- Categorical variables: ChestPain, Thal, AHD (target)
- Numerical variables: Age, Sex, RestBP, Chol, Fbs, RestECG, MaxHR, ExAng, Oldpeak, Slope, Ca

**Target Variable:** AHD (Angiographic Heart Disease)
- 0: No heart disease
- 1: Presence of heart disease

## 🔧 Technologies Used

- **Python 3.x**
- **Libraries:**
  - `pandas` - Data manipulation and analysis
  - `scikit-learn` - Machine learning models and metrics
  - `matplotlib` - Data visualization
  - `seaborn` - Statistical data visualization

## 🚀 Installation

```bash
# Install required packages
pip install pandas scikit-learn matplotlib seaborn
```

## 📁 Project Structure

```
├── Heart.csv                           # Dataset
├── régression_logistique_svm.py       # Main script
└── README.md                          # Project documentation
```

## 🔄 Workflow

### 1. Data Preparation
- Load dataset from CSV file
- Remove unnecessary columns (Unnamed: 0)
- Convert categorical variables to numerical codes
- Handle missing values
- Feature scaling using StandardScaler

### 2. Data Splitting
- Training set: 80%
- Testing set: 20%
- Random state: 17 (for reproducibility)

### 3. Model Implementation

#### Logistic Regression
- Algorithm: Binary classification using logistic function
- Parameters: `random_state=0`

#### Support Vector Machine (SVM)
- Kernel: Linear
- Parameters: `random_state=17`

### 4. Model Evaluation

**Metrics Used:**
- Accuracy (Training & Testing)
- Precision
- Recall
- F1-Score
- Confusion Matrix
- Classification Report

## 📈 Results

The project generates:
- Class distribution visualization
- Confusion matrices for both models
- Comparative bar chart of model metrics
- Detailed classification reports

## 🎯 Key Features

✅ Comprehensive data preprocessing pipeline  
✅ Handling of categorical variables  
✅ Feature standardization  
✅ Class balance analysis  
✅ Side-by-side model comparison  
✅ Visual performance metrics  

## 💡 Usage

```python
# Run in Google Colab or Jupyter Notebook
# Upload your Heart.csv file when prompted
# Execute all cells sequentially

# The script will output:
# - Training and testing accuracy
# - Precision, Recall, F1-Score
# - Confusion matrices
# - Comparative visualizations
```

## 📊 Model Comparison

The final comparison includes:
- Accuracy scores for both models
- Precision-Recall trade-offs
- F1-Score comparison
- Visual bar chart highlighting performance differences

## 🔍 Insights

- Both models are evaluated on the same test set for fair comparison
- Standardization improves model performance
- Confusion matrices reveal model strengths and weaknesses
- Metrics are weighted to account for class imbalance


## 📝 License

This project is open-source and available for educational purposes.

## 👤 Author

Samia BAYLOUL - Data Science Project - Heart Disease Classification

## 📧 Contact

For questions or suggestions, please open an issue in the repository.

---

**Note:** This project uses Google Colab for execution. Make sure to upload the Heart.csv dataset when prompted.