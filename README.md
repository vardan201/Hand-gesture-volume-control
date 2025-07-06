# ✋🔊 Hand Gesture Volume Control using OpenCV, MediaPipe & Pycaw

A real-time computer vision project that controls system volume using hand gestures detected via webcam.  
Built using Python, OpenCV, MediaPipe, and Pycaw.

---

## 📹 Demo

https://github.com/yourusername/hand-gesture-volume-control/assets/demo.gif  
*(Add a screen recording or GIF of the hand gesture controlling volume)*

---

## 🧠 How It Works

This project uses your webcam to detect hand landmarks using **MediaPipe**, then:

- Measures the distance between **thumb tip (id 4)** and **index finger tip (id 8)**
- Maps this distance to the **system volume range**
- Changes the volume in real time using **Pycaw (Windows-only)**

Visual feedback is provided on-screen using **OpenCV**.

---

## 📁 Project Structure

hand-gesture-volume-control/
│
├── Hand_Detector.py # Hand tracking module using MediaPipe
├── volume_control.py # Main script to control system volume
├── requirements.txt # Required Python packages
├── README.md # This file


---

## ⚙️ Requirements

- Python 3.10
- Webcam (integrated or USB)
- Windows OS (required for Pycaw)

---

## 📦 Installation

1. **Clone the repository**:

```bash
git clone https://github.com/yourusername/hand-gesture-volume-control.git
cd hand-gesture-volume-control


Install dependencies:

bash

pip install -r requirements.txt

🚀 Run the Project
Make sure your webcam is accessible and not used by any other app.

bash

python volume_controller.py

🧱 Core Technologies
Library	Purpose
OpenCV	Image capture and drawing visuals
MediaPipe	Hand tracking and landmark detection
Pycaw	Control Windows system volume
NumPy	Interpolation of gesture-to-volume📌 Notes
Works only on Windows (due to Pycaw's dependency on Core Audio).

Make sure cv2.VideoCapture(0) corresponds to your actual webcam.

Adjust detection confidence or hand distance thresholds if needed.

🙋‍♂️ Author
Vardan Srivastava
If you like this project, feel free to ⭐ the repo and connect with me!

