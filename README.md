# Traffic Detection using YOLOv8

## About the Project
This project utilizes the YOLOv8 object detection model to identify and count vehicles in a video feed. The model processes each frame of the video, detects vehicles, and displays the count in real time.

## Features
- Uses Ultralytics' YOLOv8 for object detection
- Detects and counts vehicles in a given video
- Highlights detected vehicles with bounding boxes
- Displays real-time vehicle count

## Requirements
Ensure you have the following dependencies installed before running the script:

```sh
pip install ultralytics torch opencv-python
```

## Usage
1. Clone the repository and navigate to the project directory.
2. Ensure you have a video file named `traffic.mp4` in the same directory.
3. Run the script using:

```sh
python traffic_detection.py
```

4. The script will process the video, detect vehicles, and display the annotated frames in a window.
5. Press 'q' to exit the video stream.

## How It Works
- Loads the YOLOv8 model and moves it to the available device (CPU/GPU).
- Reads frames from `traffic.mp4` and resizes them.
- Passes each frame through the YOLO model for detection.
- Draws bounding boxes around detected vehicles.
- Counts and displays the number of vehicles per frame.

## Customization
- To change the input video, replace `traffic.mp4` with your desired video file.
- Adjust `frame_width` and `frame_height` to modify the video resolution.
- Modify the YOLO model file (`yolov8n.pt`) to use different versions (e.g., `yolov8s.pt`).


## Acknowledgments
- [Ultralytics YOLO](https://github.com/ultralytics/ultralytics)
- [PyTorch](https://pytorch.org/)
- [OpenCV](https://opencv.org/)

## Credits
-Made by Shashank Singh.
