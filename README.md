# 🌌 Cosmic Classifier: Planet Classification Model

## 🚀 Project Overview
A machine learning model to classify planets into 10 different categories based on their physical and atmospheric characteristics. This project was developed for the IIT Roorkee Techfest ML Model Event.

**Author:** Sanskar Khandelwal  
**Cogni ID:** cogni2048376

## 📊 Dataset Overview

### Input Features (10 attributes)
1. **Atmospheric Density** (kg/m³)
2. **Surface Temperature** (Kelvin)
3. **Gravity** (m/s²)
4. **Water Content** (0-100%)
5. **Mineral Abundance** (0-1)
6. **Orbital Period** (Earth days)
7. **Proximity to Star** (AU)
8. **Magnetic Field Strength** (Tesla)
9. **Radiation Levels** (Sieverts/year)
10. **Atmospheric Composition Index** (0-1)

### Output Classes (10 German Categories)
1. Bewohnbar
2. Terraformierbar
3. Rohstoffreich
4. Wissenschaftlich
5. Gasriese
6. Wüstenplanet
7. Eiswelt
8. Toxischetmosäre
9. Hohestrahlung
10. Toterahswelt

## 🛠️ Technical Approach

### 1. Data Preprocessing
- Handled missing values using KNN imputation
- Converted categorical variables (Magnetic Field Strength, Radiation Levels) to numeric values
- Normalized features using StandardScaler
- Removed rows with missing target values

### 2. Exploratory Data Analysis (EDA)
- Analyzed feature distributions
- Created correlation heatmaps
- Visualized class imbalance
- Studied feature relationships

### 3. Model Development
Implemented and compared multiple models:
- Support Vector Machine (SVM)
- K-Nearest Neighbors (KNN)
- XGBoost
- Random Forest
- Logistic Regression

### 4. Model Optimization
- Used GridSearchCV for hyperparameter tuning
- Implemented SMOTE for handling class imbalance
- Performed cross-validation
- Optimized for accuracy and F1-score

### 5. Final Model Selection
Selected SVM as the best performing model with:
- Best parameters: {'C': 10, 'gamma': 'scale', 'kernel': 'rbf'}
- Validation Accuracy: 0.9042
- F1 Score: 0.9043
- Precision: 0.9046
- Recall: 0.9042

## 🎯 Key Achievements
- Achieved 90.42% accuracy on validation set
- Successfully handled class imbalance
- Robust handling of missing values
- Efficient feature engineering

## 🧪 Challenges Faced
1. **Data Quality Issues**
   - Missing values in multiple features
   - Class imbalance in target variable
   - Noise in the dataset

2. **Feature Engineering**
   - Converting categorical variables to meaningful numeric values
   - Handling different scales of features

3. **Model Selection**
   - Choosing between multiple algorithms
   - Optimizing hyperparameters
   - Balancing accuracy and computational efficiency

## 💡 Why This Approach?
1. **Data Preprocessing**
   - KNN imputation preserves relationships between features
   - StandardScaler ensures fair comparison of features

2. **Model Selection**
   - SVM chosen for its ability to handle non-linear relationships
   - RBF kernel captures complex patterns in the data
   - GridSearchCV ensures optimal parameter selection

3. **Class Imbalance Handling**
   - SMOTE creates synthetic samples for minority classes
   - Helps prevent model bias towards majority classes

## 📈 Results
The final model achieved impressive results across all metrics:
- High accuracy across all classes
- Balanced precision and recall
- Consistent performance on validation set

## 🔍 Future Improvements
1. Feature engineering based on domain knowledge
2. Ensemble methods combining multiple models
3. Advanced techniques for handling outliers
4. Further optimization of hyperparameters

## 🛠️ Technologies Used
- Python 3.x
- scikit-learn
- pandas
- numpy
- matplotlib
- seaborn
- XGBoost
- imbalanced-learn

## 📝 Code Structure
The implementation is organized in the following steps:
1. Data loading and initial exploration
2. Preprocessing and feature engineering
3. Model development and comparison
4. Hyperparameter tuning
5. Final model selection and evaluation
6. Prediction generation

## 🎉 Conclusion
The developed model successfully classifies planets into their respective categories with high accuracy, demonstrating the effectiveness of the chosen approach in handling complex astronomical data with various challenges.

---
*This project was developed as part of the IIT Roorkee Techfest ML Model Event.* 
