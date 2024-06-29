# Classifying Stages of Dementia

This project aims to classify different stages of dementia using a dataset of brain MRI images. The dataset is sourced from Kaggle and contains images categorized into four classes.
## Requirements
- Python 3.x 
- Tensorflow   ```pip install tensorflow```
- Keras        ```pip install keras```
- Seaborn      ```pip install seaborn```
- Scikit-learn ```pip install scikit-learn```
- Scikit-image ```pip install scikit-image```
  

## Dataset [here](https://www.kaggle.com/datasets/tourist55/alzheimers-dataset-4-class-of-images)
### About Dataset
Alzheimer MRI Preprocessed Dataset 
-The Dataset has four classes of images.
- The Dataset is consists of total 5000 MRI images.
  1. Class - 1: Mild Demented 
  2. Class - 2: Moderate Demented 
  3. Class - 3: Non Demented 
  4. Class - 4: Very Mild Demented


![image](https://github.com/ChaimaaeMsaad/Data-Science/assets/171491301/62c451c5-ed9d-4499-b19d-dab109464de4)
 



## Code
The code in this repository includes data preprocessing, image augmentation, model creation, and evaluation using various machine learning techniques. The models implemented include:

  * Convolutional Neural Networks (CNN) using the Keras API in TensorFlow:
        The CNN architecture consists of multiple convolutional layers with ReLU activation, max pooling layers, and dense layers. It uses a sequential model, starting with rescaling, followed by three sets of convolutional and max pooling layers, then flattening, and finally two dense layers. This setup is designed to classify stages of dementia effectively.

  *  Naive Bayes models with and without PCA for probabilistic classification.

  *  K-Nearest Neighbors (KNN) using PCA for dimensionality reduction.

  *  Random Forest classifiers with PCA for ensemble learning.

## Results
Keras Model Results:

The Keras model was trained and evaluated on the Alzheimer's Dataset (4 class of images) from Kaggle.

    Training Results (last epoch):
        Loss: 0.0163
        Accuracy: 99.61%

    Test Results:
        Loss: 2.2621
        Accuracy: 62.71%

These results indicate potential overfitting, as the model performed well on the training data but showed a drop in accuracy on the test data.
Naive Bayes Model Results (Without PCA):

The Naive Bayes model (Multinomial Naive Bayes) was evaluated without PCA.

    Best Parameters:
        Alpha: 0.1
        Model: Multinomial Naive Bayes
        Filter: Vertical

    Results:
        Binary Classification: 72.19% accuracy
        Multi-Class Classification: 67.34% accuracy

Random Forest Model Results:
Binary Classification (2 classes)

    Training Data:
        Accuracy: 93.75%

    Test Data:
        Accuracy: 90.00%
        Classification Report:
            Class 0: Precision 0.88, Recall 0.99, F1-Score 0.93
            Class 1: Precision 0.92, Recall 0.86, F1-Score 0.89
            Class 2: Precision 1.00, Recall 0.75, F1-Score 0.86
            Class 3: Precision 1.00, Recall 0.33, F1-Score 0.50

Multi-Class Classification (4 classes)

    Training Data:
        Accuracy: 90.31%

    Test Data:
        Overall Accuracy: 90.00%
        Macro Avg: Precision 0.95, Recall 0.73, F1-Score 0.79
        Weighted Avg: Precision 0.91, Recall 0.90, F1-Score 0.90

K-Nearest Neighbors (KNN) Model Results:
Binary Classification

    Parameters:
        PCA Components: 50
        Neighbors: 3
        Accuracy: 95.62% on test data

Multi-Class Classification

    Parameters:
        PCA Components: 50
        Neighbors: 3
        Accuracy: 93.44% on test data


## Conclusion
This repository provides a comprehensive framework for the development and evaluation of machine learning models for Alzheimer's disease detection using CNNs. The code and resources in this repository can be used as a starting point for further research and development in this area.
