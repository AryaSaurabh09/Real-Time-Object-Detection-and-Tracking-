# Real-time Object Detection and Tracking using TinyML

Welcome to the repository for Real-time Object Detection and Tracking using TinyML. This project leverages advanced computer vision techniques to detect and track objects in real-time.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Structure](#structure)
- [Technologies Used](#technologies-used)
- [Contact](#contact)

## Introduction

This project aims to develop a real-time object detection and tracking system utilizing Wireless Camera Networks (WCN). The system can identify and follow objects in a video feed, which is essential for various applications like surveillance, autonomous vehicles, and smart environments.

## Features

- **Real-time Object Detection**: Leverages deep learning models to identify objects in video frames instantly.
- **Object Tracking**: Employs advanced tracking algorithms to maintain consistent identification of moving objects.
- **Wireless Communication Integration**: Utilizes WCN for seamless data transmission and system scalability.
- **User-Friendly Interface**: Provides an easy-to-use interface for real-time monitoring and analysis.
- **Scalability**: Designed to handle multiple objects and extensive environments efficiently.

## Installation

To install and run the project, follow these steps:

1. **Clone the repository**:
   ```sh
   git clone https://github.com/AryaSaurabh09/Real-Time-Object-Detection-and-Tracking-.git
   cd Real-Time-Object-Detection-and-Tracking-
   ```

2. **Install the necessary dependencies**:
   ```sh
   pip install -r requirements.txt
   ```

## Usage

You can run the model for different sources using the following commands:

### For Video File
```sh
python yolo\v8\detect\detect_and_trk.py model=yolov8m.pt source="test.mp4" show=True
```

### For Image File
```sh
python yolo\v8\detect\detect_and_trk.py model=yolov8m.pt source="path_to_image"
```

### For Webcam
```sh
python yolo\v8\detect\detect_and_trk.py model=yolov8m.pt source=0 show=True
```

### For External Camera
```sh
python yolo\v8\detect\detect_and_trk.py model=yolov8m.pt source=1 show=True
```

## Structure

```plaintext
├── README.md
├── requirements.txt
├── main.py
├── yolo/
│   ├── v8/
│   │   ├── detect/
│   │   │   ├── detect_and_trk.py
│   │   │   └── ...
│   │   └── ...
│   └── ...
└── models/
    └── pre-trained-models/
```

- **main.py**: The entry point for the project.
- **yolo/v8/detect/**: Contains the script for detection and tracking.
- **models/**: Directory for storing pre-trained models.

## Technologies Used

- **Base Libraries:**
  - Matplotlib (plotting library)
  - NumPy (numerical computing)
  - OpenCV (computer vision library)
  - Pillow (Python Imaging Library)
  - Torch (deep learning framework)
  - Torchvision (computer vision library for PyTorch)
  - Ultralytics (deep learning research tools)

- **Tracking:**
  - FilterPy (Kalman filtering and optimal estimation library)
  - scikit-image (image processing library)

- **Programming Languages**: Python
- **Frameworks**: TensorFlow, PyTorch, TensorFlow Lite


## Contact
```
For any queries, feel free to reach out to me at saurabharya2421@gmail.com
```
