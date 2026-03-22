# 🎯 Real-Time Motion Detection & Visualization System

A Python-based real-time motion detection system that captures video from a webcam, detects movement, logs activity timestamps, and visualizes motion using an interactive timeline.

---

## 🚀 Features

- 📹 Real-time motion detection using webcam  
- 🧠 Frame differencing and contour detection  
- 🟩 Bounding boxes around moving objects  
- ⏱️ Logs motion start and end timestamps  
- 📊 Stores motion data in CSV format  
- 📈 Interactive visualization using Bokeh  
- 🖱️ Hover tooltips for detailed time intervals  

---

## 🛠️ Tech Stack

- Python  
- OpenCV (cv2)  
- Pandas  
- Bokeh  
- Datetime  

---

## 📂 Project Structure


.
├── motion_detector.py # Motion detection and data logging
├── plotting.py # Visualization using Bokeh
├── Times.csv # Generated output (motion logs)
├── Graph1.html # Generated visualization


---

## ⚙️ How It Works

### 1. Motion Detection
- Captures live video feed using webcam  
- Converts frames to grayscale and applies Gaussian blur  
- Compares current frame with the initial frame  
- Detects motion using contour detection  
- Draws bounding boxes around moving objects  
- Records timestamps when motion starts and ends  

### 2. Data Logging
- Stores motion intervals in a Pandas DataFrame  
- Saves data to `Times.csv`  

### 3. Visualization
- Reads motion data from DataFrame  
- Formats timestamps  
- Creates an interactive timeline using Bokeh  
- Displays motion duration as horizontal bars  

---

## ▶️ How to Run

### Step 1: Install Dependencies

```bash
pip install opencv-python pandas bokeh
Step 2: Run Motion Detection
python motion_detector.py
Press q to stop recording
Generates Times.csv
Step 3: Run Visualization
python plotting.py
Opens Graph1.html in your browser
📊 Output
Times.csv → Contains motion start and end timestamps
Graph1.html → Interactive visualization of motion activity
💡 Future Improvements
Email alerts on motion detection
Cloud storage integration (AWS S3, Azure Blob)
AI-based object detection (person vs object)
Mobile notifications
Multi-camera support
📌 Use Cases
Home security monitoring
Office surveillance
Smart automation systems
Activity tracking
