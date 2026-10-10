# 🚑 Ambulance Detection & Traffic Signal Control System

An ambulance detection project using a custom-trained YOLOv8 object detection model, OpenCV, Python, and Arduino. The project is designed to detect ambulances in video and send a signal to an Arduino to demonstrate traffic signal prioritization.

**Verification status:** The custom-trained model has successfully processed the sample video on macOS. Physical Arduino communication and LED switching remain to be tested.

## 📌 Features

- Ambulance detection using a custom-trained YOLOv8 model.
- Video processing using OpenCV.
- Bounding boxes and labels for detected ambulances.
- Python serial communication with Arduino.
- Arduino sketch for red and green LED control.
- Dataset, trained weights, and training artifacts included.

## 🛠️ Tech Stack

### Software
- Python 3.12
- Ultralytics YOLOv8
- OpenCV
- PySerial

### Hardware
- Arduino-compatible board
- Red and green LEDs
- USB data cable

## 📂 Project Structure

```text
Ambulance-Detection/
├── dataset/
│   ├── train/
│   │   ├── images/
│   │   └── labels/
│   └── data.yaml
├── runs/detect/train5/
│   └── weights/
│       ├── best.pt
│       └── last.pt
├── detect_ambulance.py
├── detect_custom.py
├── ardino.txt
├── yolov8n.pt
├── your_video.mp4
├── output_detected.mp4
├── readme.md
└── .gitignore