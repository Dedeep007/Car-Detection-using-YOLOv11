# Car-Detection-using-YOLOv11

## Overview
This project demonstrates how to use YOLOv11 for car detection in images and videos. YOLOv11 is the latest version of the YOLO (You Only Look Once) series developed by Ultralytics, offering state-of-the-art accuracy, speed, and efficiency for real-time object detection.

## Requirements
- Python 3.7 or higher
- TensorFlow 2.4 or higher
- OpenCV
- Ultralytics YOLOv11 package

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repository-url.git
   cd Car-Detection-using-YOLOv11
   pip install tensorflow opencv-python ultralytics

## Inference
1. Using the Trained Model
  a. Real-time Webcam Inference:

   from ultralytics import YOLO

   model = YOLO('Cardet_@_260ep.pt')

   results = model.predict(source=0, show=True, conf=0.5, save=True)

   b. File (Image/Video) Inference:

   from ultralytics import YOLO

model = YOLO('Cardet_@_260ep.pt')

results = model.predict('path_of_your_file', imgsz=640, conf=0.3, save=True, show=True)


