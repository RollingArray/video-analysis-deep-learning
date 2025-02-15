# Video Analysis with Deep Learning

## Overview
This project performs advanced video analysis using deep learning and computer vision techniques. The analysis includes:
- **Low-Level Features**: Color analysis, shape detection, motion detection.
- **Mid-Level Features**: Shot boundary detection, keyframe extraction, object detection.
- **High-Level Features**: Semantic concepts, emotional features, contextual features.
- **Motion Tracking**: Optical flow-based motion detection and visualization.

## Features Implemented
### 1. Video Properties Extraction
- Extracts **FPS, frame count, width, and height** of the video.
- Provides an overview of the video structure.

### 2. Low-Level Feature Extraction
- **Color Features**: Extracts and visualizes average color changes over time.
- **Shape Detection**: Uses edge detection (Canny) to detect objects' outlines.
- **Motion Detection**: Computes frame difference to track motion intensity.
- **Visualization**: Motion intensity plotted over time, color changes represented in a heatmap.

### 3. Object Detection
- Utilizes **TensorFlow Hub’s SSD MobileNet V2** for real-time object detection.
- **Bounding boxes** are drawn on detected objects with their labels.
- Captures **random frames** with detected objects and displays them.

### 4. High-Level Features Extraction
- **Semantic Concepts**: Identifies objects and their relevance to the video.
- **Emotional Features**: Analyzes scene brightness, color tone, and movement intensity.
- **Contextual Features**: Determines scene type (e.g., urban, nature) based on object detection.
- **Visualization**: Displays sentiment scores over time in a graph.

### 5. Motion Tracking
- Uses **Optical Flow (Farneback Algorithm)** to track motion in the video.
- Generates a **motion intensity graph** to visualize motion trends.
- Captures **random frames** of tracked motion and displays them.

## Dependencies
Ensure you have the following dependencies installed before running the code:
```bash
pip install tensorflow opencv-python numpy matplotlib
```

## How to Run
1. Place your video file in the working directory.
2. Update the `video_path` variable in the script.
3. Run the Python script to analyze the video.
4. View the generated graphs and visualizations.

## Sample Output
- **Motion intensity graph**: Shows how motion varies across the video.
- **Random object detection frames**: Displays detected objects with bounding boxes.
- **Sentiment analysis graph**: Visualizes emotional intensity in the video.
- **Motion tracking visualization**: Displays tracked motion with optical flow.

## Future Enhancements
- Implement **face detection** for enhanced emotional analysis.
- Use **transformer models** for better contextual understanding.
- Integrate **audio analysis** for multi-modal video understanding.

## Author
- Ranjoy Sen

