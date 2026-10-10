# AI-Powered Driver Drowsiness Prediction System

## Overview

A real-time driver drowsiness detection system using **Python, OpenCV, and MediaPipe**. It monitors eye closure and yawning through facial landmarks and provides an audio alert when drowsiness is detected.

## Key Features

* Real-time webcam monitoring
* Facial landmark detection using MediaPipe
* Eye Aspect Ratio (EAR) for eye closure detection
* Mouth Aspect Ratio (MAR) for yawning detection
* Automatic EAR calibration
* Drowsiness detection based on prolonged eye closure and yawning
* Audio alert using `winsound`

## Technologies

* Python
* OpenCV
* MediaPipe
* Computer Vision
* Facial Landmark Detection
* EAR and MAR

## Workflow

```text
Webcam
   ↓
OpenCV
   ↓
MediaPipe Face Landmarks
   ↓
EAR + MAR Calculation
   ↓
Eye Closure / Yawning Detection
   ↓
Drowsiness Alert
```

## Requirements

```bash
pip install mediapipe opencv-python
```

The project also requires the `face_landmarker.task` model file.

## Usage

1. Install the required libraries.
2. Place `face_landmarker.task` in the project directory.
3. Run the Python script or Jupyter Notebook.
4. Allow webcam access.
5. Keep your eyes open during the initial calibration.
6. The system will monitor eye closure and yawning in real time.
7. Press `a` to exit.

## Detection Parameters

| Parameter            |     Value |
| -------------------- | --------: |
| Calibration Frames   |        30 |
| Eye Closure Duration | 2 seconds |
| MAR Threshold        |       0.5 |
| MAR Frames           |         8 |

## Applications

* Driver monitoring
* Fatigue detection
* Vehicle safety systems
* Real-time AI and computer vision applications

## Limitations

The system can be affected by lighting, camera quality, head movement, and facial visibility.
