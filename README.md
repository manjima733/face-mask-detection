# face-mask-detection

This project classifies face mask usage into 6 categories using a YOLOv8 classifier. It detects and crops faces using OpenCV, processes the dataset, splits it into train/val/test sets, and trains a model using Ultralytics YOLOv8.

 ## Classes
We classify faces into the following 6 categories:
- mask_chin
- mask_mouth_chin
- mask_nose_mouth
- no_mask_chin
- no_mask_mouth_chin
- no_mask_nose_mouth

## Tools Used
- Python
- OpenCV (for face detection and cropping)
- Ultralytics YOLOv8 (for image classification)
- Scikit-learn (for dataset splitting)
- Matplotlib (for visualization)


##  Steps

 1. Preprocess the Dataset
- Detect faces using OpenCV
- Crop and resize to 224x224
- Relabel into 6 classes

2. Split the Dataset
- Train: 70%
- Validation: 20%
- Test: 10%

 3. Train the Classifier
- Model used: yolov8n-cls.pt
- Trained for 30 epochs with early stopping

 4. Evaluate the Model
- Test set accuracy is calculated
- prediction visualization included


