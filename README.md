# K-NN Classifier for Pima Indian Diabetes Dataset

This project implements a **K-Nearest Neighbors (K-NN)** classifier using Python to predict diabetes in the Pima Indian dataset. The goal is to experiment with different values of K (the number of neighbors) to find the best model that accurately predicts diabetes.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Methodology](#methodology)
- [Results](#results)
- [Conclusion](#conclusion)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

In this project, we implement the K-NN algorithm to classify individuals in the **Pima Indian Diabetes dataset** as either diabetic or non-diabetic. We test different K values to find the best fit for the model and evaluate the performance using metrics such as **Accuracy**, **Precision**, **Recall**, and **F1 Score**.

## Dataset

The dataset used for this project is the **Pima Indian Diabetes dataset**, which is publicly available on Kaggle:
- [Download the dataset](https://www.kaggle.com/kumargh/pimaindiansdiabetescsv)

The dataset consists of several features such as glucose levels, blood pressure, BMI, and age, which are used to predict whether a person has diabetes or not.

## Methodology

1. **K-NN Classifier**: 
   - The K-NN classifier is implemented using the `KNeighborsClassifier` from `sklearn`.
   - We iterate over different values of K (from 1 to 50) to find the optimal number of neighbors.

2. **Performance Metrics**:
   - **Accuracy**: Measures how often the model is correct.
   - **Precision**: When the model predicts someone has diabetes, how often is it correct?
   - **Recall**: Out of the people who actually have diabetes, how many does the model correctly identify?
   - **F1 Score**: The balance between precision and recall.

3. **ROC Curve and AUC**:
   - The **Receiver Operating Characteristic (ROC)** curve is plotted to show the model's ability to distinguish between classes.
   - The **Area Under the Curve (AUC)** indicates how well the classifier performs, with values closer to 1 indicating better performance.

## Results

After testing different K values, the following results were obtained:

- **K = 8** had the best **Accuracy** (0.779) and **F1 Score** (0.613).
- **K = 6** had the best **Precision** (0.684).
- **K = 1** had the highest **Recall** (0.583).

Based on these results, **K = 8** was selected as the optimal K value for this classification task, as it balanced precision and recall with the highest F1 score.

### Example Plots:
- Accuracy and F1 score across K values.
- ROC curve across different K values.

## Conclusion

We concluded that the most optimal K value for the Pima Indian Diabetes dataset is **K = 8**, as it provides the best balance between precision and recall (as indicated by the F1 Score) and has high accuracy overall. This K value is the most appropriate for identifying individuals with diabetes in the dataset.

