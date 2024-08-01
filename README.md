# YOLOv8 Object Detection and Segmentation Project

This repository contains code for object detection and segmentation using the YOLOv8 model. The project leverages Google Colab for training and inference tasks, with datasets managed via Roboflow.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Input and Output](#input-and-output)
- [Algorithms Used](#algorithms-used)

## Installation

To get started, clone the repository and install the necessary dependencies:

```python
# Mount Google Drive
from google.colab import drive
drive.mount('/content/gdrive')

# Set up the project directory
ROOT_DIR = '..path to your project directory..'
%cd {ROOT_DIR}

# Clone the Ultralytics repository
!git clone https://github.com/ultralytics/ultralytics.git

# Navigate to the cloned repository
%cd ultralytics

# Install the ultralytics package
!pip install ultralytics

# Install Ipython for displaying images
!pip install Ipython
```

# Object Detection and Segmentation


# Input and Output

## Input:

Images: JPG or PNG format images for object detection and segmentation. In this repository please refer to the input/dogs_n_cars.jpg file.
Videos: MP4 format videos for object detection and segmentation. In this repository please refer to the input/test_vid.mp4
Datasets: Custom datasets for training, managed via Roboflow. In this repository please refer to the 

## Output:

Predicted Images: Saved in the runs/detect/predict directory for object detection.
Predicted Videos: Saved in the runs/segment/predict directory for object segmentation.
Training Results: Saved in the runs/detect/train directory, including the model weights and logs.

# Algorithms Used

**YOLOv8 Model**: The YOLO (You Only Look Once) v8 model is used for both object detection and segmentation.
**Image Preprocessing**: Images are preprocessed to fit the input size requirements of the YOLOv8 model.
**Inference**: The YOLOv8 model performs inference to detect objects and segment images/videos.
**Post-processing**: Results are post-processed to display bounding boxes and segmentation masks.