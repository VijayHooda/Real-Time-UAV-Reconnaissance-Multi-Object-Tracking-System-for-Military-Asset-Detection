
## README.md


# Real-Time-UAV-Reconnaissance & Multi-Object-Tracking-System-for-Military-Asset-Detection

## Overview

Built an end-to-end UAV perception pipeline for real-time military asset detection and tracking under dense aerial surveillance conditions.

It combines:
- YOLOv8 for object detection
- DeepSORT for multi-object tracking
- Real-time inference pipeline
- FPS + latency benchmarking
- Detection visualization and output logging

---

## System Architecture

Drone Feed → Detection → Tracking → Visualization → Output

---

## Dataset

- Source: Drone-based military asset imagery
- Classes:
  - Tank
  - Military Truck
  - Armored Vehicle
  - Other tactical assets

Model trained using YOLOv8-compatible dataset structure.

---

## Model Used

- Detector: YOLOv8
- Tracker: DeepSORT
- Framework: PyTorch + OpenCV

---

## What Worked

- Real-time object detection from UAV video
- Persistent multi-object tracking using track IDs
- FPS monitoring and metrics logging
- Strong performance in medium-altitude footage

---

## What Didn’t

- Small distant objects remain difficult
- Heavy occlusion reduces tracking stability
- Low-light scenes reduce confidence

## Challenges:
- Small object detection at altitude
- Motion blur from UAV movement
- Occlusion in dense scenes
- Scale variation
  
---

## Results

- Real-time inference achieved
- FPS measured dynamically
- Latency logged automatically
- Validation mAP added after model evaluation

---

## How to Run

### Install dependencies

```bash
pip install -r requirements.txt
````

### Run system

```bash
python run.py
```

### Exit

Press ESC to close video inference.



Built a real-time drone-based reconnaissance pipeline for detecting and tracking military assets using YOLOv8 and DeepSORT, optimized for dense scenes and mission-critical aerial surveillance.

```
```
