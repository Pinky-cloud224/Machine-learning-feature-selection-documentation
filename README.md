# Documentation on different feature selection methods for machine learning

## Feature selection
Feature selection is highly impactful because ------

   - Higher number of feature can lead to model overfitting.
   - Effective for extracting non-relevent feature.
   - Reduce time and memory uses.

The dataset used has been collected from dataset colloected from https://www.kaggle.com/mathchi/diabetes-data-set. The dataset contains 768 samples and 9 features. It is a binary classification dataset.

## 1. Filter method
### 1.1 Univariate selection method

- Univariate selection method is based on the univariate statistical tests such as ANOVA, F-test.

- This method assume linear relationship between feature and target.

- The following feature selection method is based on Gaussian distribution.

** SelectKBest and SelectPercentile is the two most popular methods for univariate selection method.

### 1.1.1 SelectKBest
This method select the features according to the best scores of K.

***chi2 is effective for the classification tasks not for the regression tasks and sparse data.

### 1.1.2 SelectPercentile
This method select the features according to the best Percentile scores.

### 1.1.3 Information gain method
In this feature selection method features are selected according to the collected information from the feature.

### 1.2. ANOVA-f test
- Calculate ANOVA-f value for the selected samples.
- Effective for numerical input and categorical output data.

### 1.3. Coorelation matrix with heatmap
- Find the linear relationship between two or more variable

- Variables need to be coorrelated with the targets but uncorrelated with each other.

The feature correlation coefficient(r) has a range of -1 to 1.

- r= -1, high negative coorelation
- r= 0, no correlation
- r= 1, high positive correlation

### 1.4 Basic method
##### 1.4.1 Recursive Feature Elimination
--- Removing constant feature
- Constant feature show the same value, single value for all observation in the dataset.

- The constant features provide no information that is effective for a machine learning model to discriminate or predict a target.

## 2. Wrapper Methods

- Wrapper method is based on specific Machine learning algorithm, that are implemented on the given dataset.
- The followings are the common wrapper method-
  - Forward selection
  - Backward Elimination
  - Exhaustive feature selection
  - Recursive feature elimination
  - Recursive feature elimination with cross-validation

## 3. Embedded method
- Two most popular Embedded mothod are
  - LASSO Regression
  - Random Forest

### 3.1. LASSO Regularization

- LASSO regularization perform L2-regularization.

- Lasso regularisation helps to remove non-important features from the dataset.

- Effective for categorical input and numerical output data.
### 3.2 Random Forest
- Random forest is highly effective for providing in a good predictive performance, low overfitting and easy interpretability.