# Brain Tumor Segmentation using U-Net (BraTS 2020 Dataset)

## Project Overview
This project focuses on brain tumor segmentation using deep learning techniques. The model is built using the U-Net architecture and trained on the BraTS 2020 dataset to automatically segment brain tumors from MRI images.
The goal is to assist in medical image analysis by accurately identifying tumor regions, which can support early diagnosis and treatment planning.

## Dataset
The dataset used in this project is the BraTS 2020 (Brain Tumor Segmentation Challenge) dataset.
- Source: https://www.kaggle.com/datasets/awsaf49/brats2020-training-data
- It contains multimodal MRI scans (T1, T1ce, T2, FLAIR)
- Includes expert-labeled segmentation masks for brain tumors
Note: Due to size restrictions, the dataset is not included in this repository.

## Methodology
 1. Data Preprocessing
- Loading MRI images and masks
- Normalization of pixel values
- Resizing images for uniform input shape
- Conversion of One hot encoded to single channel
- Splitting dataset into training, validation and testing sets(80:10:10)

 2. Model Architecture
- Started with CNN Model
- U-Net deep learning model used for image segmentation
- Encoder-decoder structure with skip connections
- Designed for biomedical image segmentation tasks

 3. Model Training
- Loss Function: Dice Loss + Weighted cross entropy
- Optimizer: Adam
- Evaluation based on segmentation performance

 4. Evaluation Metrics
- Dice Coefficient
- Intersection over Union (IoU)
- Precision
- Recall
- Specificity

## Technologies Used
- Python
- Pytorch
- NumPy
- OpenCV
- Matplotlib
- Scikit-learn

## Results
- The model successfully segments brain tumor regions from MRI scans
- Achieves good performance using U-Net architecture
- Visual comparison of predicted vs ground truth masks shows effective segmentation
