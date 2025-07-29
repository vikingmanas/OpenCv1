# Face and Eye Tilt Detection 🤩

This project demonstrates real-time face and eye detection using OpenCV and Python, along with an estimation of face tilt based on the relative positions of the detected eyes.

## Table of Contents 📖
- [Features ✨](#features)
- [Prerequisites ✅](#prerequisites)
- [Installation 💻](#installation)
- [How to Run ▶️](#how-to-run)
- [How to Exit 🛑](#how-to-exit)
- [Credits 🙏](#credits)
- [License 📄](#license)

## Features ✨
* **Real-time Face Detection:** Detects faces in a live webcam feed. 🧑‍💻
* **Real-time Eye Detection:** Detects eyes within the detected face region. 👁️
* **Face Tilt Estimation:** Calculates the tilt angle of the face based on the alignment of the eyes. 📐
* **Visual Feedback:** Draws bounding boxes around faces (green) and eyes (red), and displays the tilt direction and angle on the screen. 🖼️

## Prerequisites ✅
Before you begin, ensure you have the following installed:

* **Python 3.x:** Download from [python.org](https://www.python.org/downloads/). 🐍
* **pip:** Python's package installer (usually comes with Python). 📦

## Installation 💻

1.  **Clone the repository (or create the project files):**
    If this is part of a larger repository, clone it:
    ```bash
    git clone <your-repository-url>
    cd <your-repository-name>
    ```
    Otherwise, simply create a folder for your project and save the Python script (`face_and_eye_tilt_detection.py`) inside it.

2.  **Install OpenCV:**
    Open your terminal or command prompt and run the following command to install the `opencv-python` library:
    ```bash
    pip install opencv-python numpy
    ```
    *Note: `numpy` is also required for numerical operations.*

3.  **Download Haar Cascade XML files:**
    Your script uses pre-trained Haar Cascade classifiers for face and eye detection. You need to download these files and place them in the same directory as your Python script.
    * Go to the OpenCV GitHub repository for Haar cascades: [https://github.com/opencv/opencv/tree/master/data/haarcascades](https://github.com/opencv/opencv/tree/master/data/haarcascades)
    * Download the following two files:
        * `haarcascade_frontalface_default.xml`
        * `haarcascade_eye.xml`
    * Place both downloaded XML files in the **same directory** as your `face_and_eye_tilt_detection.py` script. 📁

## How to Run ▶️

1.  **Open your Terminal / Command Prompt / PowerShell.** 2.  **Navigate to the project directory** where you saved `face_and_eye_tilt_detection.py` and the two XML files.
    For example, if your folder is `my_face_project` on your Desktop:
    ```bash
    cd C:\Users\YourUsername\Desktop\my_face_project
    ```
    (Replace `YourUsername` and `my_face_project` with your actual path and folder name.)

3.  **Execute the Python script:**
    ```bash
    python face_and_eye_tilt_detection.py
    ```

    A new window titled "Frame" will open, displaying your webcam feed with detection overlays. 📸

## How to Exit 🛑

To stop the application, simply press the **`Esc`** key on your keyboard while the "Frame" window is active.

## Credits 🙏
* This project utilizes the **OpenCV** library for computer vision functionalities.
* The face and eye detection relies on **Haar Cascade Classifiers**, which are part of the OpenCV distribution.