VISIONTRACKAI
Intelligent CCTV-Based Employee and Customer Activity Monitoring System

AI-powered surveillance system for detecting, tracking, and analyzing human activities in CCTV footage.

Project Overview

VISIONTRACKAI is a smart surveillance system designed to monitor environments such as retail stores or offices using artificial intelligence and computer vision.

The system detects people in CCTV footage, classifies them as employees or customers, tracks their movements, and records their activities in real time.

By analyzing video streams, the system provides automated insights that can help improve security monitoring, employee productivity analysis, and customer behavior understanding.

Key Features

Real-time person detection

Employee and customer classification

Multi-person tracking using unique IDs

Basic activity recognition (walking, standing, browsing, working)

Automatic activity logging

CCTV video processing

Technologies Used
Programming Language

Python

Computer Vision

OpenCV

Ultralytics YOLO

Data Processing

NumPy

Pandas

Utilities

argparse

tqdm

Libraries Used
Library	Purpose
OpenCV	Capture and process CCTV frames
Ultralytics YOLO	Detect people in images
NumPy	Calculate movement and perform numerical operations
Pandas	Store activity logs and data
argparse	Handle command-line arguments
tqdm	Display progress bars
System Architecture
CCTV Camera
     ↓
Frame Capture (OpenCV)
     ↓
Person Detection (YOLO)
     ↓
Employee / Customer Classification
     ↓
Person Tracking
     ↓
Activity Recognition
     ↓
Activity Logging

Project Structure

VISIONTRACKAI
│
├── dataset
│   ├── train
│   └── test
│
├── models
│   └── yolov8_model.pt
│
├── src
│   ├── detection.py
│   ├── tracking.py
│   ├── activity_detection.py
│   ├── activity_logger.py
│   └── main.py
│
├── logs
│   └── activity_log.csv
│
├── requirements.txt
└── README.md

Team Member Roles
Member 1 — Data Collection and Interface Developer

Responsibilities:

Collect training images and videos

Prepare dataset structure

Label images for employee and customer classes

Build display interface for system results

Manage dataset organization

Tools Used:

Python

OpenCV

Dataset annotation tools

Member 2 — Activity Analysis and Data Logging Developer

Responsibilities:

Implement person tracking

Analyze movement to detect activities

Generate activity records

Save logs in CSV or database format

Activities detected:

Walking

Standing

Browsing

Working

Tools Used:

NumPy

Pandas

OpenCV

Member 3 — AI and Computer Vision Developer

Responsibilities:

Develop detection model

Train employee vs customer classification model

Integrate YOLO detection with tracking

Optimize system performance

Tools Used:

Python

Ultralytics YOLO

OpenCV

Installation

Clone the repository:

git clone https://github.com/yourusername/VISIONTRACKAI.git

Go to project directory:

cd VISIONTRACKAI

Install dependencies:

pip install -r requirements.txt
Running the Project

Run the main file:

python src/main.py

The system will start detecting people from the CCTV feed.

Example Activity Log
Person ID	Type	Activity	Time
1	Employee	Working	10:02
2	Customer	Walking	10:03
3	Customer	Browsing	10:04
Future Improvements

Face recognition for employee identification

Suspicious activity detection

Customer behavior analytics

Dashboard visualization for managers

Cloud-based monitoring system

Conclusion

VISIONTRACKAI demonstrates how artificial intelligence and computer vision can be applied to CCTV systems for automated monitoring and activity analysis. The system provides insights into employee and customer behavior, improving operational efficiency and security management.
