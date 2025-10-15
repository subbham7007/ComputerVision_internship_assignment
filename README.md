# Vehicle Classification with Pretrained Architectures  
FILE
This repository contains the code and results for a project comparing pretrained architectures (e.g., ResNet50, EfficientNetB0) for vehicle classification using Focal Loss and Categorical Crossentropy. 

1st Download the original dataset from the link:


## **1. Dataset**  
The dataset used is the Vehicle Dataset split into training and validation sets .

- **Training Directory:** `/path/to/train`  
- **Validation Directory:** `/path/to/val`  

## **2. Prerequisites**  Install these libraries or make a Virtual environment and then install these libraries 
- python   
- matplotlib  
- scikit-learn  
- pandas  
- torch
-  torchvision 
- tensorflow
- cleanvision  
- seaborn 
- onnx
-  onnxruntime 
-  scikit-learn
- optuna
- tqdm 
- tf2onnx


Install dependencies with:  
```bash
pip install tensorflow matplotlib scikit-learn pandas ....

Clean the dataset using the cleanvision library 

now take the cleaned dataset and then test various Pre-trained model architectures like ...
Select the best model among these and then do some hyperparameter Fine Tuning of the parameters using "optuna".

Finally save the best model as onnx and again load the saved model to check if everything is working fine as given in the file.

## **To reproduce the results run the  "Deliverables\i2v-systems-imageclassification.ipynb" it has model training 
Fistly, Check all the models then training which ever performed best in our case there are two which are almost equally good 
still the one with focal_loss() is my recommendations as it is good for data sets with "IMBALANCE: as in our case.
The file also has some hyperparameter fine tuning code
and atlast it saves the model as .onnx file 
