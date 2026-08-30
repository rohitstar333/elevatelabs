# AI & ML Internship - Task 2: Exploratory Data Analysis (EDA)

## Objective

The objective of this task is to perform Exploratory Data Analysis (EDA) on the Titanic dataset to understand the data using descriptive statistics and visualizations.

The analysis focuses on identifying distributions, relationships, patterns, trends, and potential anomalies in the dataset.

## Dataset

The **Titanic Dataset** was used for this task.

The dataset contains information about passengers, including:

- Passenger ID
- Survival status
- Passenger class
- Name
- Gender
- Age
- Number of siblings/spouses
- Number of parents/children
- Ticket
- Fare
- Cabin
- Port of Embarkation

## Tools and Libraries Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Plotly
- Kaggle Notebook

## Exploratory Data Analysis Performed

### 1. Dataset Exploration

The dataset was loaded and inspected using:

- `head()`
- `shape`
- `info()`
- `describe()`
- `isnull().sum()`

The original Titanic dataset contains **891 rows and 12 columns**.

### 2. Missing Value Analysis

Missing values were identified in the following columns:

- `Age` - 177 missing values
- `Cabin` - 687 missing values
- `Embarked` - 2 missing values

For this EDA task, the original dataset was retained so that the missing values could be observed and analyzed rather than modified.

### 3. Summary Statistics

Descriptive statistics were generated for numerical features such as:

- Age
- Fare
- SibSp
- Parch
- Pclass
- Survived

Measures such as mean, standard deviation, minimum, maximum, and median were analyzed.

### 4. Histograms

Histograms were created for numerical features to understand their distributions.

The following features were analyzed:

- Age
- Fare
- SibSp
- Parch

The histograms helped identify the shape of distributions, concentration of observations, skewness, and unusual values.

### 5. Boxplots

Boxplots were created for numerical features to identify potential outliers.

The analysis focused on:

- Age
- Fare
- SibSp
- Parch

The Fare feature showed noticeable high-value observations and potential outliers.

### 6. Correlation Analysis

A correlation matrix and heatmap were created to understand relationships between numerical features.

The following features were included:

- Survived
- Pclass
- Age
- SibSp
- Parch
- Fare

### 7. Scatterplot Analysis

Scatterplots were used to visually investigate relationships between numerical features.

The following relationships were analyzed:

- Age vs Fare
- Fare vs Pclass

Survival status was also included in the visual analysis.

### 8. Survival Analysis

Survival was analyzed using visualizations based on:

- Overall survival
- Gender
- Passenger class

Survival rates were also calculated by gender and passenger class.

## Basic Feature-Level Inferences

### Age

- Passengers belong to different age groups, with many passengers concentrated in young and middle-aged ranges.
- The boxplot indicates some potential unusual age values.

### Fare

- Fare is right-skewed.
- Most passengers paid relatively lower fares.
- A smaller number of passengers paid considerably higher fares.
- The boxplot indicates several potential high-fare outliers.

### SibSp

- Most passengers had zero or a small number of siblings or spouses aboard.
- Higher values occurred less frequently.

### Parch

- Most passengers had zero parents or children aboard.
- Higher Parch values were less common.

### Passenger Class

- The dataset contains passengers from first, second, and third class.
- Third-class passengers form a large portion of the dataset.

### Gender and Survival

- Survival rates differ noticeably between male and female passengers.
- Female passengers generally had a higher survival rate than male passengers.

### Passenger Class and Survival

- Survival rates differ across passenger classes.
- First-class passengers generally had higher survival rates than second- and third-class passengers.

## Patterns, Trends and Anomalies

### Patterns and Trends

- Gender is an important feature when analyzing passenger survival.
- Passenger class is associated with survival outcomes.
- Fare varies considerably between passengers.
- Most passengers had relatively low values of SibSp and Parch.

### Anomalies

- Boxplots indicate potential outliers, particularly in the Fare feature.
- Some passengers paid substantially higher fares than most other passengers.
- Missing values are present in Age, Cabin, and Embarked.

## Key Insights

1. The Titanic dataset contains both numerical and categorical features.
2. Age contains missing values and has a varied distribution.
3. Fare is strongly right-skewed and contains potential outliers.
4. Most passengers had few or no siblings, spouses, parents, or children aboard.
5. Survival differs noticeably by gender.
6. Survival also differs across passenger classes.
7. Histograms, boxplots, heatmaps, and scatterplots help identify distributions, relationships, patterns, and anomalies.

## Conclusion

Exploratory Data Analysis was successfully performed on the Titanic dataset using summary statistics and data visualizations.

Histograms were used to understand numerical feature distributions, while boxplots helped identify potential outliers. Correlation analysis and scatterplots were used to investigate relationships between numerical features.

Survival analysis revealed noticeable differences based on gender and passenger class. The EDA process provided useful insights into the structure, distributions, relationships, patterns, and anomalies present in the Titanic dataset.

The analysis provides a foundation for further data preprocessing and machine learning model development.

## Repository Structure

```text
Task-2-EDA/
│
├── README.md
├── task-2.ipynb
└── Titanic-Dataset.csv
