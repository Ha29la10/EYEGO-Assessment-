# Real-Time Object Tracking using OpenCV

## Overview
This project implements a real-time object tracking system using Python and OpenCV. 
The system allows a user to select an object in the first frame from a live webcam feed 
using a bounding box. After selection, the tracker follows the object in real time 
while displaying the tracking results in the video stream.

A demo video showing the tracking performance is included.

---

## Features
- Manual object selection using a bounding box
- Real-time tracking from webcam feed
- Visual bounding box around the tracked object
- FPS display for performance monitoring
- Recorded demo video of the tracking process

---

## Implementation Details

The system is implemented using Python and the OpenCV library.

### Tracking Algorithm
The project uses the **CSRT (Discriminative Correlation Filter with Channel and Spatial Reliability)** tracker available in OpenCV.

CSRT was chosen because it provides:
- Higher accuracy than simpler trackers
- Better handling of scale variation
- Improved robustness when the object appearance changes

### Workflow

1. Start webcam capture.
2. Capture the first frame.
3. Allow the user to select an object using a bounding box.
4. Initialize the tracker with the selected region.
5. Continuously update the tracker on new frames.
6. Draw the bounding box on the tracked object.
7. Display FPS and tracking status in real time.



