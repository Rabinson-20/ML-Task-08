# Phishing Website Detection Using Machine Learning

## 📌 Project Overview

This project uses Machine Learning to classify website records as phishing or legitimate based on URL and website-related features. A Linear Support Vector Machine (SVM) classifier is trained and evaluated using the PhiUSIIL Phishing URL Dataset.

## 🎯 Objectives

- Analyze URL and website-related features.
- Preprocess the dataset for machine learning.
- Train a Linear SVM classification model.
- Evaluate model performance using standard classification metrics.
- Visualize predictions using a confusion matrix and ROC curve.

## 📂 Dataset

**Dataset:** PhiUSIIL Phishing URL Dataset

The dataset contains features such as:
- URL and domain characteristics
- URL length and special characters
- HTTPS status
- Website title and domain matching
- Redirects and website resources
- Forms and other website properties

**Target column:** `label`

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook / Google Colab

## ⚙️ Project Workflow

1. Load the dataset using Pandas.
2. Inspect dataset dimensions, missing values, and class distribution.
3. Remove records with missing target labels.
4. Select numerical features and handle missing or infinite values.
5. Split the dataset into 80% training and 20% testing data.
6. Standardize features using `StandardScaler`.
7. Train a Linear SVM classifier.
8. Generate predictions for test data.
9. Evaluate the model and visualize the results.

## 🤖 Machine Learning Algorithm

**Linear Support Vector Machine (Linear SVM)**

The notebook uses `LinearSVC` with the following settings:

- Regularization parameter: `C=1.0`
- Class weighting: `balanced`
- Maximum iterations: `5000`
- Random state: `42`

## 📊 Model Evaluation

The project evaluates the classifier using:

| Metric | Purpose |
|---|---|
| Confusion Matrix | Shows correct and incorrect classifications |
| Precision | Measures the accuracy of positive predictions |
| Recall | Measures how many actual positive cases are identified |
| F1-score | Balances precision and recall |
| ROC-AUC | Measures class discrimination using decision scores |
| Classification Report | Summarizes performance for each class |
| ROC Curve | Visualizes the true-positive and false-positive rate trade-off |

The actual metric values are generated when the notebook runs.

## 🚀 How to Run the Project

### Using Google Colab

1. Upload `ml task 08.ipynb` to Google Colab.
2. Upload `PhiUSIIL_Phishing_URL_Dataset.csv`.
3. Ensure the CSV path in the notebook is correct.
4. Run all notebook cells in order.
5. Review the evaluation metrics and visualizations.

### Install Required Libraries

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## 📁 Project Structure

```text
Phishing-Website-Detection/
├── ml task 08.ipynb
├── PhiUSIIL_Phishing_URL_Dataset.csv
└── README.md
```

## 🔮 Future Enhancements

- Compare multiple machine learning algorithms.
- Improve preprocessing and feature selection.
- Tune model hyperparameters.
- Test performance on unseen website data.
- Verify the original dataset label definitions.

## 👨‍💻 Project Type

Machine Learning | Binary Classification | Cybersecurity
