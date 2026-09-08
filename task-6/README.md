# Task 6 - K-Nearest Neighbors (KNN) Classification

## Objective

Understand and implement K-Nearest Neighbors (KNN) for classification problems.

## Dataset

The **Iris Dataset** was used for this task.

- Problem Type: Multi-class Classification
- Number of Samples: 150
- Number of Features: 4
- Classes: Iris-setosa, Iris-versicolor, Iris-virginica

## Tools and Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Kaggle Notebook

## Steps Performed

### 1. Data Loading and Exploration

The Iris dataset was loaded and inspected for its features, target classes, and missing values.

### 2. Feature Normalization

The four numerical features were normalized using `StandardScaler`.

This is important for KNN because the algorithm uses distances between data points.

### 3. Train-Test Split

The dataset was divided into:

- 80% training data
- 20% testing data

Stratified splitting was used to maintain the class distribution.

### 4. KNN Classification

A `KNeighborsClassifier` was trained using different values of K:

- 1
- 3
- 5
- 7
- 9
- 11
- 13
- 15

### 5. K Selection

The highest test accuracy was **96.67%**.

Multiple K values achieved this accuracy:

- K = 1
- K = 7
- K = 9
- K = 11
- K = 13
- K = 15

K = 1 was selected because it was the first K value achieving the maximum accuracy.

### 6. Model Evaluation

The final KNN model was evaluated using:

- Accuracy
- Confusion Matrix

The final test accuracy was:

**96.67%**

### 7. Decision Boundary Visualization

Decision boundaries were visualized using:

- Petal Length
- Petal Width

The visualization demonstrates how KNN separates the three Iris classes in a two-dimensional feature space.

## Results

| Metric | Result |
|---|---:|
| Selected K | 1 |
| Test Accuracy | 96.67% |

Several other K values also achieved 96.67% accuracy.

## Conclusion

K-Nearest Neighbors was successfully implemented for classification using the Iris dataset.

The experiment demonstrated feature normalization, distance-based classification, selection of K, accuracy evaluation, confusion matrix analysis, and decision-boundary visualization.

The model achieved a test accuracy of **96.67%**.
    
## Files

- `README.md` - Project documentation
- `task6_knn_classification.ipynb` - Complete Kaggle notebook
- `Iris.csv` - Dataset used for the task
