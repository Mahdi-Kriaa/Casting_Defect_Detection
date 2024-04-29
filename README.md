# Casting_Defect_Detection

## Objective
Casting is a manufacturing process where a liquid material is typically poured into a mold containing a hollow cavity of the desired shape. The material then solidifies. 
A casting defect refers to an undesired irregularity in the metal casting process. These defects can take various forms, including blow holes, pinholes, burr, shrinkage defects, mold material defects, pouring metal defects, and metallurgical defects.
In the casting industry, defects are undesirable occurrences. To mitigate defective products, companies establish quality inspection departments. However, manual inspection processes are inherently fallible due to the potential controller errors. This lack of precision can lead to the rejection of entire orders, resulting in significant losses for the company
Thus, The objective of this project is to detect any casting defect. so that we can reducing significantly the error risk.

## Data Description
The data contain grayscale images with the size of 512x512 including 519 images for good pieces (labeled "ok_front") and 781 images for defecticve ones (labeled "def_front").
This data come from the kaggle platform which is originally collected from PILOT TECHNOCAST company.
Link to dataset: https://www.kaggle.com/datasets/ravirajsinh45/real-life-industrial-dataset-of-casting-product

<p align = "center"> 
  <img src = "https://github.com/Mahdi-Kriaa/Casting_Defect_Detection/blob/main/images/ok+def.png">
</p>

## Methodology
The data will be preprocessed using data augmentation techiques, then We will explore two convolutional neural networks to detect casting defects. Model performance will be evaluated based on the accuracy score as validating a defective piece or rejecting a good one are a crucial errors


## Machine Learning 

### Machine Learning Models

Models used in this project are the following :

    - Simple CNN Model
    - Fine Tuned MobileNetV2 Model

### Models Evaluation & Results

The following are the accuracy scores for each model on the validation dataset:

    - Simple CNN model: 0.92
    - Fine Tuned MobileNetV2 model: 0.98

<p align = "center"> 
  <img src = "https://github.com/Mahdi-Kriaa/Casting_Defect_Detection/blob/main/images/confusion_matrix.png">
</p>

This is the confusion matrix for the fine Tuned MobileNetV2 model on the validation dataset
## Recommendations
- The fine tuned MobileNetV2 model can detect the majority of defective pieces but it still not perfect, so it is not reliable to trust only on it.
- Images must represent the frontal piece view and must be taken in a good brigthness level.

## Limitations & Next Steps

The model is not reliable for detecting all the casting defects so other image preprocessing techniques or models can be tried to improve the model performance.


 
