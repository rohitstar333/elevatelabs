# Task 4 - Classification with Logistic Regression

## Objective

Build a binary classification model using Logistic Regression and evaluate its performance using different classification metrics.

## Dataset

The **Breast Cancer Wisconsin Dataset** available through Scikit-learn was used for this task.

- Number of samples: 569
- Number of features: 30
- Problem type: Binary Classification
- Missing values: 0

## Tools and Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Kaggle Notebook

## Steps Performed

### 1. Data Loading and Exploration

The Breast Cancer Wisconsin dataset was loaded using Scikit-learn. The dataset was inspected for its shape, target distribution, and missing values.

### 2. Train-Test Split

The dataset was divided into:

- 80% training data
- 20% testing data

Stratified splitting was used to maintain the class distribution.

### 3. Feature Standardization

The input features were standardized using `StandardScaler`.

The scaler was fitted only on the training data and then applied to the test data.

### 4. Logistic Regression

A Logistic Regression classifier was trained using the standardized training data.

### 5. Model Evaluation

The model was evaluated using:

- Confusion Matrix
- Precision
- Recall
- ROC-AUC
- ROC Curve

The obtained results were:

| Metric | Score |
|---|---:|
| Precision | 0.9861 |
| Recall | 0.9861 |
| ROC-AUC | 0.9954 |

### 6. Sigmoid Function

The sigmoid function used in Logistic Regression was studied and visualized.

The sigmoid function is:

$$
\sigma(z) = \frac{1}{1 + e^{-z}}
$$

It converts the model's output into a value between 0 and 1, which can be interpreted as a probability.

### 7. Threshold Tuning

Different classification thresholds were tested:

- 0.3
- 0.4
- 0.5
- 0.6
- 0.7

Changing the threshold changes how predicted probabilities are converted into class labels and affects precision and recall.

## Conclusion

A binary classification model was successfully developed using Logistic Regression.

The model achieved a precision of **98.61%**, recall of **98.61%**, and ROC-AUC of **99.54%** on the test data.

The task demonstrated binary classification, feature standardization, Logistic Regression, confusion matrix, precision, recall, ROC-AUC, ROC curves, the sigmoid function, and classification threshold tuning.

## Files

- `README.md` - Project documentation
- `task4_logistic_regression.ipynb` - Complete implementation
