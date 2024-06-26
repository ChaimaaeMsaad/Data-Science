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

  * Convolutional Neural Networks (CNN) using the Keras API in TensorFlow.

  *  Naive Bayes models with and without PCA for probabilistic classification.

  *  K-Nearest Neighbors (KNN) using PCA for dimensionality reduction.

  *  Random Forest classifiers with PCA for ensemble learning.

## Results
*Keras Model Results:

* The Keras model was trained and evaluated on the Alzheimer's Dataset (4 class of images) from Kaggle.

    Training Results :
        Loss: 0.0163 |
        Accuracy: 99.61%

    Test Results:
        Loss: 2.2621 |
        Accuracy: 62.71%


```diff
- These results indicate potential overfitting, as the model performed well on the training data but showed a drop in accuracy on the test data.
```



*Naive Bayes Model Results (Without PCA) : 

* Binary Classification

    Training Accuracy: 75.94%  |
    Test Accuracy: 72.19%

* Multi-Class Classification

    Training Accuracy: 68.13%  |
    Test Accuracy: 67.34%


```diff
- These results suggest a slight drop in accuracy from training to test data, indicating some level of overfitting
```


*Naive Bayes Model Results (With PCA) :
  
* Binary Classification

    Training Accuracy: 65.39% |
    Test Accuracy: 67.19%

* Multi-Class Classification

    Training Accuracy: 56.56% |
    Test Accuracy: 54.84%

```diff
- It performs worst than without PCA ! 
```




*Random Forest Model Results (With PCA):

* Binary Classification :

    Training Accuracy: 93.75%
    Test Accuracy: 90.00%

* Multi-Class Classification : 

    Training Accuracy: 90.31%
    Test Accuracy: 90.00%


```diff
- These findings showcase the Random Forest model's strong performance when PCA is utilized, achieving high accuracy across both binary and multi-class classification tasks on the test dataset
```



*K-Nearest Neighbors (KNN) Model Results (With PCA) :

* Binary Classification

    Training Accuracy: 95.23%
    Test Accuracy: 95.63%

* Multi-Class Classification

    Training Accuracy: 94.06%
    Test Accuracy: 93.44%

* Test Data Overview

    Accuracy (binary class): 95.63%
    Accuracy (multi class): 93.44%



## Conclusion 

```diff
- KNN performs really well (fast and accurate), especially with PCA transformation because of dimension reduction. 
```

  



