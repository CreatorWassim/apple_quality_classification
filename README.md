
# **Apple Quality Classification using Support Vector Machines (SVM)**

**Introduction:**

This project aims to develop a robust machine learning model for classifying the quality of apples based on various features such as size, weight, sweetness, crunchiness, juiciness, ripeness, and acidity. Support Vector Machines (SVM) are employed as the primary classifier due to their effectiveness in handling high-dimensional data and their capability to handle non-linear decision boundaries.

You can run the original code on Kaggle:
https://www.kaggle.com/code/wassimouledmohamed/apple-quality-classification-using-svm

**Dataset:**

https://www.kaggle.com/datasets/nelgiriyewithana/apple-quality

The dataset used in this project consists of 4000 samples of apple data, with features including size, weight, sweetness, crunchiness, juiciness, ripeness, acidity, and the quality label (good or bad). The dataset was preprocessed by dropping missing values and irrelevant columns, resulting in a balanced dataset with 2004 samples labeled as 'good' and 1996 samples labeled as 'bad'.

**Data Preprocessing:**

After loading the dataset, missing values were dropped, and irrelevant columns were removed. The 'Quality' column was encoded to numerical values (1 for 'good' and 0 for 'bad'). Correlation analysis revealed no significant correlation between the features and the target variable.

**Machine Learning Model:**

The dataset was split into training and testing sets using an 80-20 split. Initially, a Linear SVM model was trained, achieving an inadequate accuracy of around 75%. Hyperparameter tuning was performed to improve the model's performance, resulting in a marginal increase in accuracy.

**Model Performance:**

Two other SVM classifiers were explored: Polynomial Kernel SVM and RBF Kernel SVM. Polynomial Kernel SVM, despite achieving high accuracy, showed signs of overfitting. RBF Kernel SVM, on the other hand, demonstrated a balance between accuracy and generalization.

**Conclusion:**

In conclusion, the RBF Kernel SVM with hyperparameters C=100 and gamma=0.1 emerged as the most effective classifier for apple quality classification, achieving a test accuracy of 93%. This model can be deployed for practical applications in fruit quality assessment, contributing to improved quality control processes in the agricultural industry. 
