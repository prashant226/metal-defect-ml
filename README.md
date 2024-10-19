 # Metal Defect Detection using Machine Learning and Keras
This project utilizes a Convolutional Neural Network (CNN) built with TensorFlow and Keras to detect defects on metal surfaces. It automates quality control by identifying various types of defects, improving the efficiency of inspection processes.

Table of Contents
Introduction
Project Structure
Features
Technologies Used
Data Preparation
Model Architecture
Installation
Usage
Results
Contributing
License
Contact
Introduction
Metal defects can significantly impact the quality and performance of products in the manufacturing industry. This project aims to automatically detect these defects using a machine learning model, reducing manual inspection efforts and minimizing errors.

Project Structure
The project is organized into the following directories:

NEU/train: Contains training data organized into six sub-folders, each representing a specific type of defect.
NEU/test: A test dataset generated from the training data.
NEU/valid: Validation data created from the test dataset to fine-tune the model's performance.
Defect Categories:
Crazing
Inclusion
Patches
Pitted
Rolled
Scratches
Features
Automated defect detection using CNNs.
Data augmentation to improve model robustness.
Early stopping mechanism to prevent overfitting.
Real-time predictions on new images.
Technologies Used
Python: For data handling and model implementation.
TensorFlow & Keras: To create and train the deep learning model.
OpenCV: For image processing and augmentation.
NumPy & Pandas: For data manipulation.
Matplotlib: To visualize training and validation results.
Data Preparation
The data is split into training, validation, and test sets using a predefined ratio:

Training Data: Contains 92% of the original images.
Test Data: Consists of 8% of the training data.
Validation Data: Formed by splitting 50% of the test data.
Image data is augmented using techniques like rescaling, shearing, zooming, and horizontal flipping to increase model generalization.

Model Architecture
The CNN architecture includes:

Convolutional Layers: To extract features from images.
Max Pooling Layers: For down-sampling to reduce dimensionality.
Dense Layers: For classification.
Dropout Layer: To prevent overfitting.
Output Layer: Uses softmax activation for multi-class classification.

