# Hand Gesture Mouse Control

Control your mouse pointer and clicks with hand gestures detected by your webcam using Python, MediaPipe, and OpenCV.

---

## Features

- Move mouse pointer by pointing your index finger
- Perform left, right, and double clicks with hand gestures
- Take screenshots using gestures
- Real-time hand tracking and gesture detection

---

## Prerequisites

- Python 3.7+
- Webcam connected and working
- Visual Studio Code (recommended) or any Python IDE/terminal

---

## Setup Instructions


### 2. Create and activate a virtual environment

- Windows (PowerShell):

```powershell
python -m venv venv
.\venv\Scripts\activate
```

- macOS/Linux:

```bash
python3 -m venv venv
source venv/bin/activate
```

You should see `(venv)` in your terminal prompt when activated.

### 3. Install required packages

If you have a `requirements.txt` file, run:

```bash
pip install -r requirements.txt
```

If not, install packages manually:

```bash
pip install opencv-python mediapipe pyautogui pynput numpy
```

Alternatively, create a `requirements.txt` file with the following content:

```
opencv-python
mediapipe
pyautogui
pynput
numpy
```

Save this file in the project root folder.

---

## Running the Application

Make sure your webcam is connected, then run:

```bash
python gesture_mouse.py
```

A window will open showing your webcam feed, and the hand gestures will control your mouse pointer and clicks.

---

## How to Stop the Program

- Click on the video window and press the **`q`** key to exit.
- Or press **Ctrl + C** in the terminal to force stop.

The webcam will be released automatically.

---

## Troubleshooting

- **No hand detected or no window:**
  - Ensure your webcam is working and not used by another app.
  - Make sure lighting and background are good.
  - Confirm you activated the virtual environment.
  - Try running a simple MediaPipe hand tracking example.

- **Missing packages or errors:**
  - Run `pip install -r requirements.txt` again.
  - Confirm the virtual environment is active.

- **Program won’t stop with `q`:**
  - Use Ctrl + C in the terminal.
  - Or close the terminal window.

- **Deactivate virtual environment:**

```bash
deactivate
```

---

## File Structure

```
hand-gesture-mouse-control/
│
├── gesture_mouse.py        # Main app code
├── util.py                 # Helper functions for angles and distances
├── requirements.txt        # Python dependencies (optional)
├── README.md               # This file
└── venv/                   # (Optional) Virtual environment folder
```

---
