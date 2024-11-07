# Predictive-Classification-of-Exoplanetary-Orbital-Periods

This project focuses on the predictive classification of exoplanetary orbital periods. By analyzing data collected from the Kepler Telescope, the model aims to classify exoplanets based on their orbital periods into distinct categories—short, medium, or long periods. Orbital period classification is essential for understanding the unique dynamics of exoplanetary systems and can offer insights into their formation, stability, and potential habitability.

## Table of contents
* Libraries used
* Dataset
* Data exploration
* Data cleaning
* Data transformation
* Data modeling
* Model assessment

### Libraries used
1. **pandas**: For data manipulation and analysis, especially handling large datasets and creating dataframes.
2. **matplotlib.pyplot** and **seaborn**: For visualizing data distributions, relationships, and trends within the dataset.
3. **numpy**: For numerical operations and array manipulations essential for scientific computations.
4. **statsmodels.stats.outliers_influence**: To calculate the Variance Inflation Factor (VIF), assessing multicollinearity among features.
5. **sklearn.preprocessing.StandardScaler**: For standardizing features to have a mean of 0 and a standard deviation of 1, which is crucial for many machine learning algorithms.
6. **sklearn.model_selection.train_test_split**: For splitting data into training and testing sets to evaluate model performance.
7. **scipy.stats.mstats.winsorize**: For handling outliers by limiting extreme values.
8. **sklearn.preprocessing.PowerTransformer**: For transforming features to improve normality, particularly useful for skewed data.
9. **statsmodels.api**: Provides a variety of statistical models, including logistic regression, used for inferential statistics.
10. **sklearn.linear_model.LogisticRegression**: The main classification algorithm for predicting the categories of exoplanetary orbital periods.
11. **sklearn.metrics (confusion_matrix, accuracy_score, classification_report)**: For evaluating model performance, providing insights into accuracy, precision, recall, and F1 scores.

### Dataset
The dataset used in this project is the [Kepler Telescope Exoplanet Discoveries](https://www.kaggle.com/datasets/melissamonfared/kepler-confirmed-planets) which was posted by _Melissa Monfared_ in Kaggle. Please read the full dataset description on the link embedded which will redirect to Melissa's data card. In summary, this dataset contains detailed information on approximately 3,373 confirmed exoplanets discovered by the Kepler Telescope, including those from the extended K2 mission. The Kepler Mission is designed to survey a large sample of stars, aiming to uncover the structure and diversity of planetary systems. The data includes various planetary and stellar parameters essential for understanding exoplanet characteristics and is invaluable in supporting the mission’s scientific objectives.

For this project, only five columns are used from the dataset:
* semi-major axis
* eccentricity
* stellar mass
* stellar temperature
* orbital period (target variable)
  
These features provide a foundational understanding of each exoplanet's orbit and stellar characteristics, supporting the classification of orbital periods.

