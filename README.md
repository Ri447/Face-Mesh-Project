# Face Mesh – Facial Landmark Detection with OpenCV & MediaPipe

A real-time facial landmark detection project built using **Python, OpenCV, and MediaPipe Face Mesh**. The project detects facial landmarks through a webcam and extracts specific facial regions to perform basic facial geometry analysis.

## Overview

This project uses MediaPipe Face Mesh to detect and track facial landmarks in real time. It processes webcam frames, identifies facial feature coordinates, and calculates geometric measurements such as Eye Aspect Ratio (EAR) and Mouth Aspect Ratio (MAR).

The goal is to understand facial landmark detection and explore how facial geometry can be used for interactive computer vision applications.

## Features

- **Real-Time Face Mesh Detection:** Detects facial landmarks through a webcam using MediaPipe.
- **Facial Landmark Extraction:** Extracts landmark IDs and their corresponding X, Y, and Z coordinates.
- **Facial Feature Identification:** Retrieves landmarks belonging to specific facial regions:
  - Left eye
  - Right eye
  - Lips
  - Nose
- **Forehead Landmark Extraction:** Identifies selected forehead landmarks for future face-filter and object-placement applications.
- **Eye Aspect Ratio (EAR):** Calculates the ratio between vertical and horizontal eye dimensions to analyse eye openness.
- **Mouth Aspect Ratio (MAR):** Calculates the ratio between vertical and horizontal mouth dimensions to analyse mouth openness.
- **Facial Distance Calculation:** Uses Euclidean distance to calculate distances between facial landmarks.

## Technologies Used

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| OpenCV | Webcam access and image processing |
| MediaPipe | Facial landmark detection |
| NumPy / Math | Mathematical and geometric operations |

## Concepts Explored

### 1. Face Mesh

MediaPipe Face Mesh detects 468 facial landmarks per face. These landmarks represent key points across the face, allowing facial features to be identified and tracked.

### 2. Facial Landmark Coordinates

Each landmark contains normalized X, Y, and Z coordinates. The normalized coordinates are converted into pixel coordinates using the dimensions of the webcam frame.

### 3. Eye Aspect Ratio (EAR)

EAR measures eye openness using the distances between selected eye landmarks.

It can be used as a foundation for blink detection.

### 4. Mouth Aspect Ratio (MAR)

MAR measures mouth openness by comparing the vertical distance between the upper and lower lips against the horizontal distance between the mouth corners.

It can be used to identify whether the mouth is open or closed.

## Project Structure

```text
Face-Mesh/
│
├── FaceMeshModule.py
├── FaceMesh.py
└── README.md
```

## Learning Outcomes

Through this project, I explored:

- Real-time computer vision using OpenCV.
- Facial landmark detection using MediaPipe.
- Extracting and working with specific facial regions.
- Coordinate mapping between normalized landmarks and image pixels.
- Applying Euclidean distance to facial geometry.
- Using EAR and MAR for facial feature analysis.

---

**Current Focus:** Exploring facial landmark geometry and building the foundation for real-time interactive face filters.
