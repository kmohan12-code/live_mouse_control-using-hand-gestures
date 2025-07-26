README.md
markdown
Copy
Edit
# Hand Gesture Mouse Control Project

This project uses **MediaPipe**, **OpenCV**, and **Python** to control the mouse with hand gestures via your webcam.

---

## Prerequisites

- Python 3.7 or higher installed on your system
- VS Code installed
- Webcam connected and working
- Basic knowledge of running Python scripts in VS Code

---

## Step 1: Open the Project in VS Code

1. Launch **Visual Studio Code**.
2. Click **File > Open Folder**.
3. Select the project folder containing your scripts (`gesture_mouse.py` and `util.py`).
4. Open the integrated terminal by clicking **Terminal > New Terminal**.

---

## Step 2: Create and Activate a Virtual Environment

In the VS Code terminal:

### On Windows (PowerShell):

```powershell
python -m venv venv
.\venv\Scripts\activate
On macOS/Linux:
bash
Copy
Edit
python3 -m venv venv
source venv/bin/activate
You should see (venv) prefix in the terminal prompt, indicating the environment is activated.

Step 3: Install Required Packages
Run this command in the activated environment:

bash
Copy
Edit
pip install -r requirements.txt
If you don’t have requirements.txt, create it with the following packages:

Copy
Edit
opencv-python
mediapipe
pyautogui
pynput
numpy
Step 4: Run the Gesture Mouse Control Script
Make sure your webcam is connected.

In the terminal, run:

bash
Copy
Edit
python gesture_mouse.py
A window will open showing your webcam feed.

Show your hand clearly in front of the camera.

The program will detect your hand and respond to gestures like mouse movement and clicks.

Step 5: How to Stop the Program and Turn Off the Camera
Click the video window and press the q key to quit and close the webcam.

Or, go to the terminal and press Ctrl + C to forcibly stop the program.

The camera will be released automatically upon exit.

Troubleshooting
If the window doesn’t show or hand is not detected, ensure:

Good lighting and a clear background.

Your webcam is working with other applications.

You activated the virtual environment before running.

If you get errors about missing packages, run pip install -r requirements.txt again.

Additional Notes
For any modifications, edit gesture_mouse.py and util.py files.

Always activate the virtual environment before running the script.

To exit the virtual environment, type:

bash
Copy
Edit
deactivate
Contact
If you have any issues or questions, feel free to reach out!

Happy coding! 🚀

yaml
Copy
Edit

---

If you want me to generate a ready `.md` file to download or help customize it further, just say!







You said:
i need complete readme file to add in github


ChatGPT said:
Absolutely, Mohan! Here's a complete, polished README.md for your GitHub repo that explains your project, setup, usage, and troubleshooting clearly.

markdown
Copy
Edit
# Hand Gesture Mouse Control

A Python application that uses **MediaPipe** and **OpenCV** to control your mouse pointer and clicks using hand gestures detected via your webcam.

---

## Features

- Move mouse pointer by pointing your index finger
- Perform left, right, and double clicks with different hand gestures
- Take screenshots using specific gestures
- Real-time hand tracking using MediaPipe
- Cross-platform support (Windows, macOS, Linux)

---

## Demo

![Demo Screenshot or GIF](link-to-your-demo-image-or-gif-if-any)

---

## Prerequisites

- Python 3.7 or higher
- Webcam connected and working
- Visual Studio Code (recommended) or any Python IDE/terminal

---

## Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/hand-gesture-mouse-control.git
cd hand-gesture-mouse-control
2. Create and activate a virtual environment
Windows (PowerShell)

powershell
Copy
Edit
python -m venv venv
.\venv\Scripts\activate
macOS/Linux

bash
Copy
Edit
python3 -m venv venv
source venv/bin/activate
3. Install dependencies
bash
Copy
Edit
pip install -r requirements.txt
If requirements.txt is missing, install packages manually:

bash
Copy
Edit
pip install opencv-python mediapipe pyautogui pynput numpy
Usage
Make sure your webcam is connected and working.

Run the gesture control script:

bash
Copy
Edit
python gesture_mouse.py
A window will open showing your webcam feed with hand landmarks.

Use your hand to control the mouse pointer and perform clicks based on gestures:

Move mouse: Point your index finger.

Left click: Specific gesture (see source code for gesture details).

Right click: Specific gesture.

Double click: Specific gesture.

Screenshot: Specific gesture.

To exit, click on the video window and press the q key or press Ctrl + C in the terminal.

File Structure
bash
Copy
Edit
hand-gesture-mouse-control/
│
├── gesture_mouse.py        # Main application file
├── util.py                 # Utility functions for angle and distance calculations
├── requirements.txt        # Python dependencies
├── README.md               # This file
└── venv/                   # (Optional) Virtual environment folder
Troubleshooting
No window opens or hand not detected:

Check your webcam connection.

Ensure good lighting and clear background.

Confirm virtual environment is activated.

Try running the minimal MediaPipe hand tracking example to verify setup.

Packages missing or import errors:

Run pip install -r requirements.txt again.

Ensure you are in the activated virtual environment.

Program doesn’t stop with q key:

Use Ctrl + C in the terminal to force stop.

Virtual environment issues:

To exit the virtual environment, type deactivate in your terminal.

Contributing
Feel free to submit issues or pull requests to improve the project!


Contact
Created by Mohan Koduri
For any questions or support, open an issue or contact me via GitHub.
