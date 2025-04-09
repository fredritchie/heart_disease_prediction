# Heart Disease Prediction Project

This project focuses on predicting heart disease using machine learning techniques. The analysis is based on data obtained from Kaggle. [cite: 5]

## Data Preprocessing

The dataset was preprocessed to handle categorical variables and prepare it for modeling. The following transformations were applied:

* Gender was mapped to numerical values (Female: 0, Male: 1). [cite: 7]
* Smoking status was converted to numerical categories (Heavy: 3, Current: 0, Former: 1, Never: 2). [cite: 7]
* Alcohol intake was categorized (Heavy: 0, Moderate: 1, None: 2). [cite: 7]
* Family History, Diabetes, Obesity, and Exercise Induced Angina were converted to binary (Yes: 1, No: 0). [cite: 7]
* Chest Pain Type was mapped to numerical values (Atypical Angina: 0, Typical Angina: 1, Non-anginal Pain: 2, Asymptomatic: 3). [cite: 7]

## Correlation Analysis

A correlation matrix was generated to visualize the relationships between different features in the dataset. [cite: 9] The analysis revealed no significant correlation between Exercise Induced Angina and Smoking with Heart Disease. [cite: 9]

## Model Training and Evaluation

### Ensemble Learning with XGBoost

* The project initially explored using XGBoost, a gradient boosting framework, for ensemble learning. [cite: 15, 16, 17, 18, 19, 20]
* However, the XGBoost model's results were deemed unreliable. [cite: 25]

### Scikit-learn Random Forest

* Due to the issues with XGBoost, the project shifted to using the Random Forest algorithm from the Scikit-learn library. [cite: 25]
* It was found that both the best parameters and default parameters for Random Forest led to overfitting. [cite: 26]

### K-Nearest Neighbors (KNN)

* The K-Nearest Neighbors (KNN) algorithm was then employed for classification. [cite: 27, 28, 29, 30, 31, 32, 33]
* Different K values were tested, and the optimal K value was determined to be 61. [cite: 34, 35]
* The KNN model with the optimal K value yielded reasonable results. [cite: 36]
* K-Fold cross-validation was performed, and the score was satisfactory. [cite: 37]

## Conclusion

The project explored various machine learning models for heart disease prediction. The KNN algorithm, with an optimized K value, provided the most reliable results.