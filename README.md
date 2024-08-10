# Music Genre Classification Project

This project focuses on classifying music tracks into genres using machine learning techniques.

### 1. Dataset Preparation
We begin by loading the metadata and track metrics provided by The Echo Nest. This data forms the foundation for our analysis and model training.

### 2. Identifying Correlated Features
To ensure our model isn't using redundant features, we check for strong correlations between variables using Pandas' correlation function (`.corr()`). Removing highly correlated features helps in reducing feature redundancy.

### 3. Feature Normalization
Next, we normalize the features using Scikit-learn’s `StandardScaler`. Normalization is a crucial step before applying dimensionality reduction techniques like Principal Component Analysis (PCA), as it ensures all features contribute equally to the analysis.

### 4. Applying PCA
With the normalized data, we apply PCA to reduce the dimensionality of our dataset. We analyze scree plots and cumulative explained variance plots to determine the optimal number of components that capture the most variance in the data.

### 5. Visualizing PCA
We further analyze the cumulative explained variance plot to decide on the number of components required to explain approximately 85% of the variance. This step is vital for understanding how much of the data’s information we are retaining.

### 6. Genre Classification with Decision Trees
Using the reduced-dimensionality data from PCA, we classify the music tracks into genres using a decision tree algorithm. Decision trees are a simple yet powerful method for classification tasks.

### 7. Comparing Models: Decision Tree vs. Logistic Regression
We compare the performance of the decision tree with logistic regression, a simpler classification model. This comparison helps us understand whether a more complex model is necessary or if a simpler approach suffices.

### 8. Model Evaluation with Cross-Validation
To validate the performance of our models, we apply cross-validation (CV). Cross-validation gives us a better estimate of how well our model is likely to perform on unseen data.
