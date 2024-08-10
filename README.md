# Music Genre Classification

### 1. Dataset Preparation
With streaming services becoming the main way people listen to music, categorizing tracks for personalized recommendations has become essential. We'll start by loading metadata and track metrics from The Echo Nest.

### 2. Identifying Correlated Features
To avoid feature redundancy, we’ll check for strong correlations between variables using Pandas' `.corr()` function.

### 3. Feature Normalization
Since there are no strong correlations, we’ll reduce the number of features using Principal Component Analysis (PCA). First, we normalize the data using Scikit-learn’s `StandardScaler`.

### 4. Applying PCA
With our scaled data, PCA will help us reduce dimensionality. We’ll use scree plots and cumulative explained variance plots to determine the optimal number of components.

### 5. Visualizing PCA
We'll examine the cumulative explained variance plot to decide how many components are needed to capture about 85% of the variance.

### 6. Genre Classification with Decision Trees
Using the lower-dimensional PCA data, we’ll classify songs into genres with a decision tree algorithm.

### 7. Comparing Models: Decision Tree vs. Logistic Regression
We'll compare the decision tree with logistic regression to see if a simpler model performs better.

### 8. Model Evaluation with Cross-Validation
To assess our models' performance, we’ll use cross-validation (CV).
