# Final Project: Diabetes Prediction and Analysis

## Overview
This project explores and applies machine-learning techniques to predict diabetes outcomes based on patient health data. The dataset is processed, visualized, and modeled using regression, classification, and clustering techniques. The project output includes model predictions, visualizations, and accuracy/error metrics for each model.

## Data Preprocessing
- **Outlier Removal**: Outliers were managed using the Interquartile Range (IQR) method.
- **Scaling**: StandardScaler was applied to normalize PCA and model input features.
- **Principal Component Analysis (PCA)**: PCA was performed for dimensionality reduction, retaining 2 components.

## Models and Equations

### 1. **Linear Regression**
   - **Equation**: $` y = wX + b `$
   - **Metrics**: Mean Squared Error (MSE) on the test set.
   - **Performance**: MSE is evaluated to assess accuracy.

### 2. **Logistic Regression**
   - **Equation**: $` P(Y=1|X) = \frac{1}{1 + e^{-(wX + b)}} `$
   - **Metrics**: MSE, ROC AUC Score, Classification Report, Confusion Matrix.
   - **Performance**: Provides accuracy on diabetes classification.

### 3. **Decision Tree Regressor**
   - **Equation**: Recursive partitioning divides data points based on feature thresholds.
   - **Metrics**: MSE for regression tasks.
   - **Performance**: Outputs prediction error in regression.

### 4. **K-Nearest Neighbors (KNN)**
   - **Equation**: Distance-based prediction based on k-nearest data points.
   - **Metrics**: ROC AUC Score, Classification Report, Confusion Matrix.
   - **Performance**: Measures accuracy in classifying diabetes.

### 5. **Artificial Neural Network (ANN)**
   - **Architecture**: 3-layer network (128, 64, 1 nodes) with ReLU and Sigmoid activation.
   - **Loss Function**: Binary Crossentropy.
   - **Metrics**: Accuracy on test data.
   - **Performance**: Evaluates model accuracy over 10 epochs.

### 6. **Support Vector Machine (SVM)**
   - **Equation**: Maximizes the margin between classes.
   - **Metrics**: MSE, ROC AUC Score, Classification Report, Confusion Matrix.
   - **Performance**: SVM model accuracy in diabetes classification.

### 7. **K-Means Clustering**
   - **Equation**: $` \text{minimize} \sum_{i=1}^k \sum_{x \in C_i} \|x - \mu_i\|^2 `$
   - **Metrics**: Silhouette Score for clustering quality.
   - **Performance**: Optimal clusters analyzed; scores achieved around 0.499.

## Output and Evaluation
Each model's predictions are saved as `.csv` files and performance metrics are calculated for each, focusing on either MSE for regression tasks or classification metrics (e.g., ROC AUC, accuracy) for classification tasks.
