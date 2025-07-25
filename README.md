# Pancreatic Cancer Tumor vs Non-Tumor Classification

This project aims to classify pancreatic tissue samples as tumor or non-tumor using gene expression data. The classification model was built using machine learning techniques such as Random Forest, Logistic Regression, and Support Vector Machine (SVM). The project utilizes the GSE28735 dataset, which contains gene expression data for pancreatic cancer.

## Overview

Pancreatic cancer is one of the most lethal cancers, and early detection is crucial for improving patient outcomes. This project focuses on leveraging gene expression data to classify pancreatic tissue samples as either tumor or non-tumor using computational models. The project is intended to explore how machine learning can be applied in cancer diagnostics.

### Project Goals:
- Build a model to classify pancreatic cancer tissue samples as tumor vs. non-tumor.
- Utilize gene expression data from the GSE28735 dataset.
- Evaluate multiple classification algorithms and compare their performance.
- Provide insights into the gene expression features that best distinguish tumor from non-tumor samples.

## Dataset

The dataset used in this project is from the **GSE28735** series. It contains gene expression data from pancreatic cancer samples. The dataset includes **90 samples** and **28,869 genes**.

- **Tumor vs. Non-Tumor**: The dataset includes paired samples of tumor and adjacent non-tumor tissue from pancreatic cancer patients. Each sample has a corresponding gene expression profile.

### Data Columns:
- **Gene Expression Matrix**: Rows represent genes, and columns represent individual tissue samples. The values represent the expression levels of genes in the tissue samples.
- **Sample Labels**: Each sample is labeled as tumor (1) or non-tumor (0).

## Requirements

To run this project, the following dependencies need to be installed:

- Python 3.x
- pandas
- scikit-learn
- matplotlib
- seaborn
- numpy
- XGBoost (Optional for enhanced performance)

- ## How to Run

1. **Clone the repository to your local machine**:

    ```bash
    git clone https://github.com/your-username/pancreatic-cancer-classification.git
    ```

2. **Navigate to the project directory**:

    ```bash
    cd pancreatic-cancer-classification
    ```

3. **Install the necessary Python packages**:

    ```bash
    pip install -r requirements.txt
    ```

4. **Download the GSE28735 dataset and extract it into the project directory**.

5. **Run the classification model**:

    ```bash
    python classify_pancreatic_cancer.py
    ```

    This script will:
    - Load and preprocess the gene expression data.
    - Train multiple machine learning models (Random Forest, SVM, etc.).
    - Evaluate and compare model performance.
    - Output the final accuracy, precision, recall, and F1-score for each model.

## Results

- **Accuracy**: 83% (on test set).
- The **Random Forest** model outperformed other models with high accuracy and balanced precision/recall scores.

<img width="1189" height="790" alt="image" src="https://github.com/user-attachments/assets/124b4624-4a2b-4f96-9aa7-8d44533e3cee" />


### Evaluation Metrics:
- **Accuracy**: The proportion of correct predictions (both tumor and non-tumor) out of all predictions.
- **Precision**: The proportion of true positives (tumor samples correctly classified) out of all predicted positives.
- **Recall**: The proportion of true positives out of all actual positives (tumor samples).
- **F1-Score**: The harmonic mean of precision and recall, which gives a balanced measure of performance.
