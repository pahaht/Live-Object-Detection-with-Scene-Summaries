![alt text]( https://github.com/pahaht/Live-Object-Detection-with-Scene-Summaries/blob/main/bicycle-car.JPG)

## Live-Object-Detection-with-Scene-Summaries

This repository contains a Python script that uses YOLOv11 for real-time object detection in video streams. Instead of displaying labels on individual objects, the script draws bounding boxes around detected objects and overlays a dynamic textual summary at the top of the frame, which lists the types and counts of objects detected. 

## Features

- **Real-time Object Detection:** Uses YOLOv11 (Nano model) for fast inference.
- **Clean Visualization:** Draws only bounding boxes on detected objects (no individual labels).
- **Dynamic Summary:** Generates and displays a textual summary of all detected objects at the top of the video frame.
- **Flexible Input:** Works with an image, webcam or a video file.

## Requirements

- Python 3.11
- [Ultralytics YOLO](https://github.com/ultralytics/ultralytics)
- [OpenCV-Python](https://pypi.org/project/opencv-python/)
- [NumPy](https://pypi.org/project/numpy/)

## Installation
1. **Clone the repository:**

2. **Install the required dependencies:**
pip install ultralytics opencv-python numpy

## Code Overview
The main script (yolo_summary.py) performs the following tasks:

1.Model Loading:
Loads the lightweight YOLOv8 model (yolov8n.pt) for object detection.

2.Video Capture:
Opens a video stream from a webcam (or video file).

3.Object Detection & Summary Generation:

Processes each video frame to detect objects.
Counts the number of objects per label.
Constructs a textual summary (e.g., "This video displays a person, 2 cars.").

4.Visualization:

Draws bounding boxes around detected objects (labels are not shown on the boxes).
Overlays the summary text at the top of the frame.
Displays the processed video stream in real time.

   

  
