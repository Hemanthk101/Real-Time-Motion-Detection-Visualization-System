# 🎯 Real-Time Motion Detection & Visualization System

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.x-blue?logo=python">
  <img src="https://img.shields.io/badge/OpenCV-Computer%20Vision-green?logo=opencv">
  <img src="https://img.shields.io/badge/Bokeh-Visualization-orange">
  <img src="https://img.shields.io/badge/Status-Active-success">
  <img src="https://img.shields.io/badge/License-MIT-lightgrey">
</p>

---

## 📌 Overview

A **real-time motion detection system** built using **Python and OpenCV** that captures video from a webcam, detects movement, logs activity timestamps, and visualizes motion patterns using an interactive timeline.

This project demonstrates:
- Computer Vision (OpenCV)
- Real-time video processing
- Data logging & analytics
- Interactive visualization (Bokeh)

---

## 🚀 Features

- 📹 Real-time motion detection using webcam  
- 🧠 Frame differencing & contour detection  
- 🟩 Bounding boxes for detected motion  
- ⏱️ Logs motion start & end timestamps  
- 📊 Saves structured data in CSV format  
- 📈 Interactive timeline visualization  
- 🖱️ Hover tooltips for detailed insights  

---

## 🛠️ Tech Stack

| Category            | Technology Used        |
|--------------------|----------------------|
| Programming        | Python               |
| Computer Vision    | OpenCV (cv2)         |
| Data Processing    | Pandas               |
| Visualization      | Bokeh                |
| Time Handling      | Datetime             |

---

## 📂 Project Structure
- motion_detector.py
- plotting.py
- Times.csv
- Graph1.html
- 
---

## ⚙️ How It Works

### 🔹 Step 1: Motion Detection
- Captures live video from webcam  
- Converts frames to grayscale and applies Gaussian blur  
- Compares frames to detect differences  
- Uses contour detection to identify motion  
- Draws bounding boxes around moving objects  

### 🔹 Step 2: Data Logging
- Tracks motion start and end times  
- Stores timestamps in a Pandas DataFrame  
- Exports results to `Times.csv`  

### 🔹 Step 3: Visualization
- Reads timestamp data  
- Converts it into readable format  
- Generates an interactive graph using Bokeh  
- Displays motion intervals visually  

---

## ▶️ Getting Started

### 🔧 Prerequisites

- Python 3.x installed

### 📦 Install Dependencies

```bash
pip install opencv-python pandas bokeh
▶️ Run the Application
1. Start Motion Detection
python motion_detector.py
Press q to stop recording
This will generate Times.csv
2. Generate Visualization
python plotting.py
Opens Graph1.html in your browser
📊 Output
File	Description
Times.csv	Motion start and end timestamps
Graph1.html	Interactive motion timeline graph
📸 Demo (Optional)

Add screenshots or GIFs here for better presentation

![Demo Screenshot](your-image-link-here)
💡 Future Enhancements
🔔 Email alerts on motion detection
☁️ Cloud storage (AWS S3 / Azure Blob)
🤖 AI-based object detection (YOLO / TensorFlow)
📱 Mobile notifications
🎥 Multi-camera support
📌 Use Cases
🏠 Home security systems
🏢 Office monitoring
🤖 Smart surveillance applications
📊 Activity tracking & analytics
🧠 Learning Outcomes
Real-time video processing
Computer vision fundamentals
Event-based logging systems
Data visualization techniques
End-to-end Python project design
