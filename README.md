# Pose Estimation with Kalman Filtering

This project implements real-time pose estimation and tracking using MediaPipe, OpenCV, and Kalman filters for enhanced stability. It processes video frames to detect keypoints and applies Kalman filtering to reduce noise, ensuring smooth and accurate pose estimation.

---

## Sample Input Results


## Introduction

This project uses computer vision to detect human poses in video frames with real-time processing. By integrating Kalman filters, it improves the stability of detected keypoints, minimizing jitter and inaccuracies.

Key objectives:
- Detect human poses using MediaPipe's pose estimation model.
- Enhance the accuracy and consistency of pose tracking with Kalman filtering.
- Visualize keypoints directly on video frames.

---

## Features

1. **Real-Time Pose Detection**:
   - Uses MediaPipe to identify 33 keypoints on the human body.

2. **Noise Reduction**:
   - Applies Gaussian filters for preprocessing.
   - Uses Kalman filters to stabilize detected keypoints.

3. **Frame-by-Frame Processing**:
   - Handles video input and processes each frame independently.

4. **Keypoint Visualization**:
   - Draws detected keypoints on frames for visualization.

---

## Dependencies

Ensure you have the following libraries installed:

- `mediapipe`
- `opencv-python-headless`
- `numpy`
- `scipy`
- `pykalman`

Install them with:

```bash
pip install mediapipe opencv-python-headless numpy scipy pykalman
```

---

## Installation and Setup

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/your-repo/pose-estimation.git
   cd pose-estimation
   ```

2. **Install Required Libraries**:

   ```bash
   pip install -r requirements.txt
   ```

3. **Provide Video Input**:

   Replace the `video_path` in the script with your video file's path.

4. **Run the Script**:

   ```bash
   python untitled2.py
   ```

---

## Usage

Load your video file in the specified path. The script processes the video frame by frame:

1. Detects pose keypoints.
2. Filters noise using Kalman filters.
3. Displays the video with overlaid keypoints.


---


### Results:
1. **Visual Output**:
   - The processed video displays keypoints overlaid on the body parts in real time.
   - Smoothed trajectories of keypoints due to Kalman filtering.

2. **Performance Metrics**:
   - Reduced jitter in detected keypoints.
   - Stable and consistent pose estimation across frames.

3. **Example Visualization**:
   - Keypoints such as shoulders, elbows, and knees are distinctly highlighted, enabling clear tracking of movements.

---

## How It Works

1. **Input Video**:
   - Reads the input video frame by frame.

2. **Preprocessing**:
   - Converts frames to grayscale.
   - Applies Gaussian filtering to reduce noise.

3. **Pose Detection**:
   - Uses MediaPipe to detect keypoints on the human body.

4. **Kalman Filtering**:
   - Stabilizes the detected keypoints by reducing noise and smoothing the trajectory.

5. **Visualization**:
   - Draws keypoints on the processed frames and displays the output in real-time.

---

## Future Enhancements

1. **Support for Live Webcam Input**:
   - Extend functionality to process webcam streams.

2. **Gesture Recognition**:
   - Integrate gesture-based controls using the detected keypoints.

3. **Performance Optimization**:
   - Optimize Kalman filtering and pose detection for faster processing.

4. **Cross-Platform Compatibility**:
   - Develop a mobile version for Android and iOS.

---



