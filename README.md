# High-Recall Type 2 Diabetes Prediction

Type 2 Diabetes Mellitus is a major metabolic disorder that often progresses silently, making early detection critical. This project provides an end-to-end deep learning framework for diabetes screening using 100,000 clinical records. False negatives in medical diagnostics carry severe consequences; this model strictly prioritizes **Recall (sensitivity)** over raw accuracy. 

## Dataset
Diabetes prediction dataset (https://www.kaggle.com/datasets/iammustafatz/diabetes-prediction-dataset), which contains 100,000 clinical records featuring key demographic and biomarker data.

## The Approach
Instead of using spatial models like CNNs, this project utilizes an **Attention-Enhanced Multi-Layer Perceptron (Attention-MLP)** tailored for independent tabular clinical data. 
* **Feature Attention:** Dynamically prioritizes critical clinical biomarkers, such as HbA1c and blood glucose levels.
* **Class Imbalance:** Addresses the severe 8.5% diabetic minority class using SMOTE (Synthetic Minority Over-sampling Technique) and Focal Loss optimization.

## Results
Evaluated on an isolated testing set, the Attention-MLP successfully identified at-risk individuals, outperforming baseline models:
* **Attention-MLP Recall:** 92.0%
* **1D-CNN Recall:** 89.0%
* **Baseline MLP Recall:** 86.0%

#### Collaboration
This project was collaborated on by Jingying Ng, Jiayu Ong, Xinya Siow and JunXun Too.
