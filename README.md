# YOLOv5-Powered Self-Driving Cars: Autorickshaw Detection

## Project Overview
This project implements a real-time object detection system using YOLOv5 for the perception module of self-driving cars. The model is trained to detect Autorickshaws, which are common vehicles in Indian traffic environments.

## Objectives Completed
- Used pre-trained YOLOv5s model for object detection on static images, videos, and live webcam feed.
- Created a custom dataset for Autorickshaw detection using Roboflow.
- Trained YOLOv5s model on the custom dataset.
- Tested the trained model on images and real-time webcam.

## Dataset
- Source: Roboflow
- Class: Autorickshaw
- Format: YOLOv5 PyTorch

## Model
- Base Model: YOLOv5s
- Trained for 50 epochs
- Best weights saved as best.pt

## How to Run Detection

### On Webcam:
python detect.py --weights best.pt --source 0 --conf 0.4

### On Images:
python detect.py --weights best.pt --source path/to/images --conf 0.4

### On Video:
python detect.py --weights best.pt --source path/to/video.mp4 --conf 0.4

## Project Structure
YOLOv5_Autorickshaw_Detection/
├── best.pt
├── data.yaml
├── results.png
├── README.md
├── detect_commands.txt
└── detection_results/

## Tools & Technologies
- Python
- YOLOv5 (Ultralytics)
- OpenCV
- Roboflow
- Google Colab (for training)