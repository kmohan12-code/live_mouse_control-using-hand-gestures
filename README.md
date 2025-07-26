
# Hand Gesture Mouse Control Project

This project uses **MediaPipe**, **OpenCV**, and **Python** to control the mouse with hand gestures via your webcam.

---

## Prerequisites

- Python 3.7 or higher installed on your system
- VS Code installed
- Webcam connected and working
- Basic knowledge of running Python scripts in VS Code



## Step 1: Open the Project in VS Code

1. Launch **Visual Studio Code**.
2. Click **File > Open Folder**.
3. Select the project folder containing your scripts 
4. Open the integrated terminal by clicking **Terminal > New Terminal**.

## Step 2: Create and Activate a Virtual Environment

In the VS Code terminal:

### On Windows (PowerShell):

python -m venv venv
.\venv\Scripts\activate

macOS/Linux:

python3 -m venv venv
source venv/bin/activate

Install required packages

pip install -r requirements.txt
If you don’t find requirements.txt, install manually:

pip install opencv-python mediapipe pyautogui pynput numpy

File Structure

hand-gesture-mouse-control/
│
├── gesture_mouse.py        # Main app code
├── util.py                 # Helper functions for angles and distances
├── requirements.txt        # List of dependencies
├── README.md               # This file
└── venv/                   # (Optional) Virtual environment folder


Running the Application
Ensure your webcam is connected.

Run the gesture mouse control script:


python gesture_mouse.py

