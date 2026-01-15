# 🚦 Smart Control of Traffic Light Using Artificial Intelligence

An AI-driven traffic management system that dynamically controls traffic lights based on real-time traffic density. This project combines **computer vision (YOLO)** with a **traffic simulation engine (Pygame)** to demonstrate intelligent and adaptive traffic signal control.

---

## 📌 Problem Statement

Traditional traffic signal systems rely on:

* Manual traffic control (high manpower)
* Fixed-time signals (inefficient for varying traffic)
* Sensor-based systems (high deployment cost)

These approaches fail to adapt efficiently to real-time traffic density.

---

## 💡 Proposed Solution

This project uses **traffic cameras and AI-based vehicle detection** to:

* Detect and count vehicles in each lane using **YOLO (You Only Look Once)**
* Estimate traffic density dynamically
* Adjust traffic signal timing automatically

The system supports:

* **Simulated traffic control** using Pygame
* **Real-world traffic video analysis** using YOLO

---

##  Key Features

*  Real-time vehicle detection & counting
*  Adaptive green/red signal timing
*  Traffic simulation using Pygame
*  YOLO-based video processing
*  User-friendly GUI using Tkinter

---

##  Technologies Used

* **Python 3**
* **YOLOv3 (OpenCV DNN)**
* **Pygame** – Traffic simulation
* **Tkinter** – GUI
* **OpenCV** – Video processing
* **NumPy, SciPy** – Computation

---

##  Project Structure

```
├── Main.py                     # Main GUI application
├── traffic_simulation.py       # Pygame traffic simulation logic
├── yolo_traffic.py             # YOLO vehicle detection & counting
├── run.bat                     # One-click project launcher
├── requirements_instructions.txt
├── output.mp4                  # YOLO processed output video
├── images/                     # Simulation assets (signals, vehicles)
├── yolo-coco/                  # YOLO config, weights, class names
└── Smart_traffic_SCREENS.docx  # Screenshots & documentation
```

---

##  Installation & Setup

### 1️ Prerequisites

* Python 3.x
* Windows OS (recommended)

### 2️ Install Dependencies

```bash
pip install pygame==2.0.0
pip install keras==2.3.1
pip install tensorflow==1.14.0
pip install opencv-python imutils numpy scipy
```

> **Note:** YOLO runs slowly on systems without GPU support.

---

##  How to Run the Project

### Option 1: Using Batch File (Recommended)

```bash
Double-click run.bat
```

### Option 2: Manual Execution

```bash
python Main.py
```

---

##  Modules Explanation

###  Run Traffic Simulation

* Launches a Pygame-based traffic intersection
* Vehicles are generated randomly
* Signal timings adjust automatically based on density

###  Run YOLO Traffic Detection & Counting

* Upload a traffic video (e.g., `traffic2.mp4`)
* YOLO detects & counts vehicles frame-by-frame
* Output saved as `output.mp4`

---

##  Screenshots & Demo

Screenshots and execution flow are available in:

```
Smart_traffic_SCREENS.docx
```

---

##  Output

* Live traffic simulation window
* Processed video with:

  * Bounding boxes
  * Vehicle IDs
  * Total vehicle count overlay

---

##  Future Enhancements

* GPU acceleration (CUDA)
* Lane-wise signal optimization
* Emergency vehicle prioritization
* IoT-based live camera integration
* Cloud-based traffic analytics dashboard

---
