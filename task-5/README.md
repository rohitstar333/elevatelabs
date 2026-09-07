# Task 5 - Decision Trees and Random Forests

## Objective

Build classification models using Decision Tree and Random Forest algorithms and compare their performance.

## Dataset

The **Heart Disease Dataset** (`heart.csv`) was used for this task.

- Problem type: Binary Classification
- Target column: `target`
- Dataset: Heart Disease Dataset

## Tools and Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Kaggle Notebook

## Steps Performed

### 1. Data Loading and Exploration

The Heart Disease dataset was loaded using Pandas. The dataset was inspected for:

- Dataset dimensions
- Column names
- Data types
- Missing values
- Target class distribution

### 2. Train-Test Split

The dataset was divided into:

- 80% training data
- 20% testing data

Stratified splitting was used to maintain the class distribution.

### 3. Decision Tree Classifier

A Decision Tree Classifier was trained on the training data.

The model was evaluated using test accuracy and a classification report.

### 4. Decision Tree Visualization

The trained decision tree was visualized using `plot_tree()` to understand how the model makes classification decisions.

The visualization was limited to a depth of 3 for better readability.

### 5. Tree Depth and Overfitting

Different values of `max_depth` were tested to study the effect of tree complexity on training and testing accuracy.

As tree depth increases, the model becomes more complex. Very deep trees can learn the training data too closely and may lead to overfitting.

### 6. Random Forest Classifier

A Random Forest Classifier with 100 decision trees was trained.

Random Forest combines predictions from multiple decision trees to produce a final classification.

### 7. Model Comparison

The Decision Tree and Random Forest models were compared using:

- Test Accuracy
- Mean Cross-Validation Accuracy

### 8. Feature Importance

Feature importance was calculated using the Random Forest model.

The most important features were identified and visualized using a bar chart.

### 9. Cross-Validation

5-fold cross-validation was performed for both:

- Decision Tree
- Random Forest

The individual cross-validation scores and their mean accuracy were calculated.

## Results

The final model comparison was performed using test accuracy and mean 5-fold cross-validation accuracy.

The exact values are available in the Kaggle notebook output.

| Model | Test Accuracy | Mean CV Accuracy |
|---|---:|---:|
| Decision Tree | See notebook | See notebook |
| Random Forest | See notebook | See notebook |

## Conclusion

Decision Tree and Random Forest classifiers were successfully implemented for binary classification using the Heart Disease Dataset.

The Decision Tree visualization helped understand the decision-making process of a tree-based classifier. Different tree depths were tested to analyze model complexity and possible overfitting.

Random Forest was then used as an ensemble learning approach by combining multiple decision trees. Feature importance was also analyzed to identify the features that contributed most to the model's predictions.

Finally, 5-fold cross-validation was performed to obtain a more reliable estimate of model performance.

## Files

- `README.md` - Project documentation
- `task5_decision_tree_random_forest.ipynb` - Complete implementation
- `heart.csv` - Dataset used for the task
