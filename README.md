# Person Detection with YOLOv8

## Table of Contents
- [About The Project](#about-the-project)
- [Built With](#built-with)
- [Getting Started](#getting-started)
- [Installation](#installation)
- [Dependencies](#dependencies)
- [Project Structure](#project-structure)
- [Usage](#usage)
- [Features](#features)
- [Google Colab Setup](#google-colab-setup)
- [Contributing](#contributing)
- [License](#license)

## About The Project
This project implements person detection using YOLOv8, a state-of-the-art object detection algorithm. The project demonstrates how to:
- Download a custom dataset using Roboflow
- Train a YOLOv8 model on a custom person detection dataset
- Perform inference on images and videos
- Save and visualize detection results

## Built With
- [Ultralytics YOLOv8](https://github.com/ultralytics/ultralytics)
- [Roboflow](https://roboflow.com/)
- [OpenCV](https://opencv.org/)
- [Google Colab](https://colab.research.google.com/)

## Getting Started
To get started with this project, you'll need:
- A Google Colab account
- Roboflow API key
- Custom person detection dataset

## Installation
1. Open a new Google Colab notebook
2. Install required libraries:
```python
!pip install ultralytics roboflow
```

## Dependencies
- ultralytics
- roboflow
- opencv-python
- google-colab

## Project Structure
```
project_root/
│
├── images/
│   ├── inp.jpg        # Input image for detection
│   └── out.jpg        # Output image with detections
│
├── videos/
│   ├── testrel.mp4    # Input video
│   └── test_video_out.mp4  # Output video with detections
│
└── runs/              # Training results and model weights
```

## Usage
### Training the Model
1. Mount Google Drive
2. Initialize Roboflow and download dataset
3. Train YOLOv8 model for a specified number of epochs

### Image Detection
1. Load the trained model
2. Set detection threshold
3. Run inference on an input image
4. Save output image with bounding boxes

### Video Detection
1. Load the trained model
2. Process video frame by frame
3. Apply object detection
4. Save output video with bounding boxes

## Features
- Custom dataset training
- Person detection in images
- Person detection in videos
- Configurable detection threshold
- Visualization of detection results

## Google Colab Setup
1. Connect to Google Colab
2. Enable GPU runtime
3. Mount Google Drive
4. Install dependencies
5. Run training and inference scripts

## Contributing
Contributions are welcome! Please:
- Fork the repository
- Create a new branch
- Submit a pull request

## Authors
Shubam Sarawagi

## Acknowledgements
- Ultralytics for YOLOv8
- Roboflow for dataset management
- Google Colab for computational resources
```
