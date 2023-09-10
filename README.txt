# California Housing Price Predictor

This project is an exploration and prediction of housing prices in California using various regression models. The data source is the `housing.csv`, which contains different features related to housing prices in California.

## 🚀 Features

1. **Exploratory Data Analysis (EDA)**:
    - Understanding the dataset with `.info()`.
    - Visualization of `ocean_proximity` values.
    - Distribution visualizations with histograms.
    - Visualization of `median_income` stratification.

2. **Feature Engineering**:
    - Addition of `inc_cat` for income categories.
    - Geographical scatter plot showing population and median house values.

3. **Transformers & Pipelines**:
    - Custom transformer: `ClusterSimilarity` calculates the RBF kernel similarity between instances and cluster centroids.
    - Pipelines for different preprocessing tasks, such as:
        - Calculating ratio-based features.
        - Log-transformations.
        - Geographical clustering.
        - One-hot encoding of categorical variables.
        - Standard scaling.

4. **Modeling**:
    - Linear Regression
    - Decision Tree Regressor
    - Random Forest Regressor
    - Support Vector Machines (with Grid and Randomized Search for hyperparameter tuning)

5. **Evaluation**:
    - Use of RMSE for model evaluation.
    - Cross-validation scores to get insights on model's performance variance.

6. **Feature Selection**:
    - Use of `SelectFromModel` for feature importance.
    
7. **Custom Transformer**:
    - `FeatureFromRegression`: A transformer that uses predictions from a given estimator as a new feature.

## 📌 Requirements

- pandas
- numpy
- matplotlib
- scikit-learn

## 🔧 Getting Started

1. Clone this repository.
2. Make sure you have all the required libraries installed.
3. Run the code using a Python environment or Jupyter notebook.

## 📊 Analysis Results

- The histogram analysis shows that many features are right-skewed.
- `median_income` and `median_house_value` data have been capped.
- `ClusterSimilarity` transformer was used to create features based on geographical data, using clustering techniques.
- Hyperparameter tuning for SVR using both GridSearch and RandomizedSearch gave insights into best parameters for optimal performance.

## 📝 Conclusion

This project showcases a detailed exploration, preprocessing, modeling, and evaluation process to predict housing prices in California. Different models and techniques were utilized to get a holistic understanding of the data and improve prediction capabilities.
