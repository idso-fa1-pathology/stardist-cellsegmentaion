# Cell Detection in Microscopy Images with StarDist

## Overview
This project demonstrates the application of the StarDist model for cell detection in microscopy images, specifically tailored to a custom multiplex immunofluorescence (mIF) dataset. Our approach leverages deep learning and image processing techniques to identify and classify cell types within microscopy images, aiding in the analysis and understanding of cellular structures and behaviors.

## Dataset
The dataset consists of microscopy images and corresponding masks that delineate individual cells. Additionally, class dictionaries are provided to classify cells based on specific criteria. This setup aims to facilitate the training and evaluation of the StarDist model for precise cell detection and classification.

## Methodology
The project utilizes the StarDist 2D model, configured for our specific use case. Key steps in the workflow include:

- Preprocessing of images and masks to fit the model requirements.
- Normalization and augmentation to enhance model training.
- Training the StarDist model with custom configurations.
- Evaluation of model performance with various metrics.

### Preprocessing
Images and masks are loaded, normalized, and prepared for training. Class dictionaries are applied to categorize cells into predefined classes, essential for the model's classification tasks.

### Model Configuration and Training
We configured the StarDist 2D model with parameters suited to our dataset's characteristics. Training involves data augmentation techniques such as random flipping, rotation, and intensity changes to improve model robustness.

### Evaluation
The model's performance is evaluated using precision, recall, accuracy, F1 score, and other relevant metrics at different Intersection over Union (IoU) thresholds. Visualization of predictions alongside ground truth annotations provides intuitive insights into the model's effectiveness.

## Requirements
- Python 3.6+
- [StarDist](https://github.com/stardist/stardist)
- TensorFlow 2.0+
- NumPy
- Matplotlib
- scikit-image
- tqdm

## Installation
Clone this repository and install the required dependencies:
```bash
git clone <repository-url>
cd <repository-directory>
pip install -r requirements.txt
