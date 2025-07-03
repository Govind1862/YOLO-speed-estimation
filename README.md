# YOLO-speed-estimation
Real-time vehicle detection and speed estimation using YOLOv8 and OpenCV. Tracks vehicles via centroid tracking and calculates their speed based on frame-to-frame displacement. Ideal for smart traffic monitoring and surveillance systems.


# Real-Time Vehicle Detection & Speed Estimation using YOLOv8

A real-time computer vision project using **YOLOv8** and **OpenCV** that detects vehicles in a video stream, tracks them, and estimates their speed based on their movement across frames.


## Features

- ✅ Real-time object detection using YOLOv8
- ✅ Vehicle tracking with unique object IDs
- ✅ Speed estimation in km/h based on centroid tracking
- ✅ Live video feed with bounding boxes, labels, and speeds
- ✅ Easily configurable for webcam or video file input

---

## How It Works

1. YOLOv8 detects all objects in each frame.
2. Vehicles (cars, bikes, trucks, buses) are filtered out using COCO class labels.
3. Each vehicle's position is tracked across frames using centroid comparison.
4. Speed is estimated using the formula:  
   \[
   \text{Speed} = \frac{\text{Pixel Distance}}{\text{Time Difference}}
   \]
5. Vehicle ID and speed are displayed in the video feed.

> **Note:** The current speed is in pseudo km/h using pixel-based estimation. For real-world accuracy, camera calibration is needed.

---
