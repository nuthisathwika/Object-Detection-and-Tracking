# Object-Detection-and-Tracking
This project uses the MobileNet-SSD model for real-time object detection and tracking on video files and live webcam streams. It identifies objects with accuracy and speed, displaying bounding boxes and labels. A Tkinter-based GUI enables easy video upload, webcam access, and real-time visualization for users.

## Features

- *Real-time Object Detection:* Employs the efficient MobileNet-SSD model for fast and accurate detection.
- *Multiple Video Sources:* Supports processing both local video files and live webcam feeds.
- *Multi-Class Identification:* Capable of detecting 20 common object classes.
- *Simple GUI:* A straightforward interface built with Tkinter allows users to easily select their video source.

## How It Works

The application loads a pre-trained MobileNet-SSD Caffe model. When a user selects a video source (a file or webcam), the script reads the video frame by frame. Each frame is pre-processed into a blob and passed through the neural network. The model returns the detected objects, their locations, and a confidence score. Bounding boxes and class labels are then drawn on the frames for objects detected with a confidence score above a set threshold, and the resulting video is displayed in real-time.

## Setup and Installation

### Prerequisites

- Python 3.x
- OpenCV

The necessary model files are included in the repository:
- MobileNetSSD_deploy.prototxt.txt
- MobileNetSSD_deploy.caffemodel

### Instructions

1.  *Clone the repository:*
    bash
    git clone https://github.com/jagruthi42/Object-Detection-and-Tracking.git
    cd Object-Detection-and-Tracking
    

2.  *Create and activate a virtual environment (recommended):*
    bash
  
    # Create the environment
    python -m venv venv

   On Windows:

       .\venv\Scripts\activate


   On macOS/Linux:

        source venv/bin/activate
    

3.  *Install the required dependencies:*
    bash
    pip install -r requirements.txt
    

## Usage

To run the application, execute the app.py script from your terminal:

bash
python app.py


- In the application window, click *"Browse System Videos"* to select a video file from your computer.
- Click *"Start Webcam Video Tracking"* to use your live webcam feed as the source.
- While the video is playing, press the q key to stop the stream and close the video window.

## Files

- app.py: The main application script containing the GUI logic and object detection loop.
- MobileNetSSD_deploy.prototxt.txt: The architecture definition for the Caffe model.
- MobileNetSSD_deploy.caffemodel: The pre-trained weights for the MobileNet-SSD model.
- requirements.txt: Lists the Python packages required to run the project.

## Screenshots

<img width="1156" alt="Application GUI and a frame from a detected video" src="https://github.com/user-attachments/assets/5d584eed-2ed9-4356-a1b5-01c984a94bb2" />



https://github.com/user-attachments/assets/7e88a148-3ede-42d3-b2ae-2ccdae899fbf
