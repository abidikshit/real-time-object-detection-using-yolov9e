# Real-Time Object Detection with YOLOv9 and Supervision

[![Watch the video](/output_video/objectdetection.png)](Real-Time-Object-Detection-Using-YOLOv9-e/output_video/LiveFeed_Detect_Log.mp4)

<a href="/output_video/LiveFeed_Detect_Log.mp4" target="_blank">
  <img src="/output_video/objectdetection.png" alt="Watch the video" width="500" height="300">
</a>

## Overview

This project showcases real-time object detection using YOLOv9, coupled with Supervision for annotating detected objects on security camera feeds. The system generates real-time logs in nested JSON format, detailing object counts with respective timestamps, and implements a priority system to flag objects based on predefined criteria.

## Features

- **Real-Time Object Detection**: Utilizes YOLOv9 for real-time object detection on security camera feeds.
- **Annotation and Visualization**: Uses Supervision for annotating detected objects on frames with labels.
- **Data Logging**: Generates nested JSON logs with object counts and timestamps for each frame.
- **Priority System**: Implements a priority system to give real-time alerts based on object presence and duration.
- **Configurability**: Supports configuration through a JSON file, allowing easy customization of camera URLs and other parameters.

## Requirements

- Python 3.x
- OpenCV (`cv2`)
- Supervision
- Ultralytics YOLO

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/abidikshit/real-time-object-detection-using-yolov9e.git
    ```

2. Navigate to the project directory:
    ```bash
    cd real-time-object-detection-using-yolov9e
    ```

3. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. Update the `config.json` file with your camera details and other configurations.
2. Run the main script:
    ```bash
    python main.py --config config.json
    ```

## File Structure
├── main.py # Main script for real-time object detection
├── supervision.py # Annotator and other utilities using Supervision
├── yolov9e.pt # Pre-trained YOLOv9 model
├── config.json # Configuration file
├── requirements.txt # Required Python packages
├── output.json # JSON logs with object counts and timestamps
├── class_counts.csv # CSV file with class counts
└── README.md # Project documentation


## License

This project is licensed under the MIT License. See [LICENSE](https://github.com/abidikshit/Real-Time-Object-Detection-Using-YOLOv9-e/blob/main/LICENSE) for more details.

