# Counterfeit Currency Classification Using KNN

## Project Overview

This project uses Python and machine learning to classify banknotes as genuine or counterfeit based on their physical measurements.

A K-Nearest Neighbors (KNN) classification model was developed using the banknote dataset. The project demonstrates data preprocessing, feature scaling, supervised machine learning, and model evaluation.

## Technologies and Libraries

- Python
- Pandas
- NumPy
- Scikit-learn
- Jupyter Notebook

## Dataset

The dataset contains 1,500 banknote observations and six physical measurement features:

- Diagonal
- Left height
- Right height
- Lower margin
- Upper margin
- Length

The target variable indicates whether a banknote is genuine or counterfeit.

## Methodology

1. **Data Loading:** Imported the dataset using Pandas.
2. **Data Inspection:** Examined the dataset and identified missing values.
3. **Missing Value Treatment:** Replaced missing values in `margin_low` with the column median.
4. **Label Encoding:** Converted the genuine/counterfeit target variable into numerical values.
5. **Train/Test Split:** Divided the data into 80% training and 20% testing sets.
6. **Feature Scaling:** Applied StandardScaler to standardize the features.
7. **Model Training:** Trained a K-Nearest Neighbors classifier using five neighbors.
8. **Model Evaluation:** Evaluated predictions using accuracy, a confusion matrix, precision, recall, and F1-score.

## Results

The KNN classifier achieved **98.33% accuracy** on the held-out test dataset.

### Confusion Matrix

| | Predicted Counterfeit | Predicted Genuine |
|---|---:|---:|
| Actual Counterfeit | 105 | 5 |
| Actual Genuine | 0 | 190 |

### Classification Performance

| Metric | Counterfeit | Genuine |
|---|---:|---:|
| Precision | 1.00 | 0.97 |
| Recall | 0.95 | 1.00 |
| F1-score | 0.98 | 0.99 |

## Key Takeaways

- Practiced handling missing data and preparing a dataset for machine learning.
- Applied feature scaling to improve distance-based classification.
- Developed a supervised classification model using scikit-learn.
- Evaluated model performance using multiple classification metrics.
- Explored the application of machine learning to counterfeit currency detection.

## Project Files

- `project4JT.ipynb` — Jupyter Notebook containing the original analysis and model development.

## Future Improvements

Potential extensions include comparing different classification algorithms, experimenting with different values of K, and evaluating model performance using cross-validation.
