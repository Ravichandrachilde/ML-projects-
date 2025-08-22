Cancer Cell Classification using Scikit-learn

This project demonstrates how Machine Learning can be applied to solve real-world problems in the medical field.
We use the Breast Cancer Wisconsin (Diagnostic) dataset to classify cancer cells as Malignant (cancerous) or Benign (non-cancerous) using Naive Bayes.

Dataset

Source: Scikit-learn’s built-in dataset (load breast cancer)

Instances: 569 tumor samples

Features: 30 (e.g., radius, texture, perimeter, area)

Target labels:

0 → Malignant (cancerous)

1 → Benign (non-cancerous)


Project workflow

Data Import & Exploration:

   	Loaded dataset from sklearn.datasets

   	Explored using pandas (df.info(), df.describe())

	Visualized class distribution with a pie chart

Data Preprocessing:

	Split dataset into training (67%) and testing (33%) using train_test_split

Model Building:

	Used Gaussian Naive Bayes (GaussianNB) for classification

	Trained model on the training dataset

Model Evaluation:

	Predicted labels on the test set

	Evaluated performance with accuracy_score

Achieved ~94.15% accuracy

Tech Stack

Language: Python

Libraries:

scikit-learn → dataset, model, evaluation

pandas → data exploration

matplotlib → visualization


Results

Accuracy: ~94.15%

The Naive Bayes model successfully classified tumor samples with high precision.

Project highlights how ML can assist in early cancer detection and medical diagnostics.