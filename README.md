# Gesture Control Mouse and Screenshot Application

This project is a Python application that uses hand gesture recognition to control mouse actions (such as moving the cursor, left-click, right-click, double-click, and taking screenshots) via a webcam. The program leverages MediaPipe for hand tracking, OpenCV for real-time video processing, and PyAutoGUI for mouse and screenshot actions.

---

## Features

1. **Cursor Movement:** Move the cursor based on the index finger tip's position.
2. **Left Click:** Perform a left-click gesture.
3. **Right Click:** Perform a right-click gesture.
4. **Double Click:** Perform a double-click gesture.
5. **Screenshot:** Take a screenshot and save it to the current directory.

---

## Requirements

To run this application, ensure you have the following installed:

- Python 3.7+
- OpenCV
- MediaPipe
- PyAutoGUI
- Pynput

---

## Installation

1. Clone or download this repository.
2. Install the required libraries:
   ```bash
   pip install opencv-python mediapipe pyautogui pynput
   ```
3. Run the script:
   ```bash
   python script_name.py
   ```

---

## Usage

1. Run the script in a Python environment.
2. Ensure your webcam is functioning and the lighting is adequate for hand detection.
3. The application will display a video feed.
4. Perform the following gestures to trigger specific actions:

   - **Move Cursor:** Move your index finger to move the mouse cursor.
   - **Left Click:** Position your hand so the angle between specific finger landmarks matches the predefined threshold for a left-click.
   - **Right Click:** Adjust your hand so the gesture matches the criteria for a right-click.
   - **Double Click:** Position your hand to meet the criteria for a double-click gesture.
   - **Screenshot:** Perform the screenshot gesture to take a screenshot, which will be saved in the current directory as `my_screenshot_<random_label>.png`.

5. Press the `q` key to exit the program.

---

## Code Explanation

### Key Functions:

1. **`find_finger_tip(processed):`**
   - Identifies the position of the index finger tip using MediaPipe landmarks.

2. **`move_mouse(index_finger_tip):`**
   - Moves the mouse cursor based on the position of the index finger tip.

3. **`is_left_click`, `is_right_click`, `is_double_click`, `is_screenshot`:**
   - Check if the hand gesture matches the criteria for the respective mouse action or screenshot.

4. **`detect_gesture(frame, landmark_list, processed):`**
   - Detects gestures from the hand landmarks and executes the corresponding action.

5. **`main():`**
   - Captures video feed, processes frames, and detects gestures in a loop until the `q` key is pressed.

---

## Notes

1. Adjust the detection confidence thresholds if the hand tracking is inaccurate.
2. Modify the screen resolution mapping if your screen size differs significantly.
3. Ensure that `util.get_distance` and `util.get_angle` are properly defined in a `util.py` file or replace them with alternative distance/angle calculation logic.

---

## Known Issues

1. Gesture recognition may be inaccurate under poor lighting conditions or if the hand is partially obscured.
2. Limited to detecting one hand at a time.
3. Requires a webcam for real-time detection.

---

## Contributing

Feel free to fork the repository and submit pull requests for improvements or bug fixes.

---

