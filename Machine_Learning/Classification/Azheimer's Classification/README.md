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
The code in this repository includes data preprocessing, image augmentation, model creation and evaluation using CNNs, and transfer learning techniques. The CNN models are implemented using the Keras API in Tensorflow. Transfer learning is performed using pre-trained CNN models such as VGG and ResNet.

## Results
The results of the experiments conducted using CNN models are presented in the form of accuracy and loss as shown below:<br></br>
- **Validation loss:** 0.0687 or **6.87%**
- **Validation accuracy:** 0.9805 or **98.05%**
- **Number of misclassified images:** 25 of 1280
## Conclusion
This repository provides a comprehensive framework for the development and evaluation of machine learning models for Alzheimer's disease detection using CNNs. The code and resources in this repository can be used as a starting point for further research and development in this area.
