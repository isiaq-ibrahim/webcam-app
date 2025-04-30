# 📸 Webcam App – Python OpenCV Project
This repository contains the source code for a simple Webcam App I built with Python and OpenCV. The application captures an image from the laptop's webcam and saves it locally on the computer.

## 🚀 Project Overview
This project demonstrates the basic usage of the OpenCV library for webcam interfacing and image capture in real-time. It's a beginner-friendly project designed to show how computer vision can be used for simple media tasks.

## 🧰 Technologies Used
- Python 3.10.7
- OpenCV (cv2)

## 📷 Features
- Accesses your computer’s webcam
- Captures a single image frame
- Saves the captured image as test.jpg in the working directory

## 🛠️ Installation

1. Clone the repository
```bash
git clone https://github.com/isiaq-ibrahim/webcam-app
cd webcam-app
```

2. Create a virtual environment (optional but recommended)
```bash
python -m venv venv
source venv/bin/activate  # For Linux/Mac
venv\Scripts\activate     # For Windows
```

3. Install the required library
```bash
pip install opencv-python
```

## ▶️ Usage

Run the script with Python:
```bash
python webcam_app.py
```

Once executed, the app will:
1. Open your webcam
2. Capture a single image frame
3. Save it as test.jpg
4. Exit after printing "Image Captured..."

## 🧠 How It Works
```bash
import cv2

imgCapture = cv2.VideoCapture(0)
result = True

while(result):
    ret, frame = imgCapture.read()
    cv2.imwrite("test.jpg", frame)
    result = False
    print("Image Captured...")

imgCapture.release()
```

- `cv2.VideoCapture(0)` – Accesses the default webcam.
- `cv2.imwrite()` – Writes the frame as an image file.

### 📂 Output

After running the script, you’ll find a file named `test.jpg` in your project directory.

### 📄 License

This project is licensed under the MIT License.

### 🙌 Acknowledgements

Thanks to the OpenCV community for providing extensive documentation and support for developers working in computer vision.
