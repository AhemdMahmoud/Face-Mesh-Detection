# Face Mesh Detection Project

This project implements real-time face mesh detection using OpenCV and MediaPipe libraries. It captures video from your computer's camera and overlays a face mesh on any detected faces in real-time.

## Screenshot

![Face Mesh Detection Screenshot](https://github.com/AhemdMahmoud/Face-Mesh-Detection/blob/main/face%20mish.png)

## Features

- Real-time face detection
- Face mesh overlay with tesselation and contours
- Easy-to-use interface

## Prerequisites

Before you begin, ensure you have met the following requirements:

- Python 3.7 or higher
- pip (Python package manager)

## Installation

1. Clone this repository:
   ```
   git clone https://github.com/AhemdMahmoud/Face-Mesh-Detection.gith
   cd face-mesh-detection
   ```

2. Install the required packages:
   ```
   pip install opencv-python mediapipe
   ```

## Usage

1. Run the script:
   ```
   python face_mesh_detection.py
   ```

2. A window will open showing the video feed from your camera with the face mesh overlay.

3. Press 'q' to quit the application.

## How it works

The application uses the following process:

1. Capture video frames from the camera
2. Convert each frame to RGB color space
3. Process the frame with MediaPipe's face mesh model
4. Draw the face mesh tesselation and contours on the frame
5. Display the processed frame

## Customization

You can customize the appearance of the face mesh by modifying the `DrawingSpec` parameters in the code. For example:

```python
drawing_spec = mp_drawing.DrawingSpec(thickness=1, circle_radius=1, color=(0,255,0))
```

Adjust the `thickness`, `circle_radius`, and `color` values to change the appearance of the mesh.



## Acknowledgments

- OpenCV team for their computer vision library
- Google's MediaPipe team for their face mesh solution
