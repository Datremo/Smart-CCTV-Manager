# Smart-CCTV-Manager

A Python-based smart CCTV management system built with OpenCV and Tkinter, featuring motion detection, in-out logging, video recording, and facial recognition.

## 🌟 Features

- **Motion Detection**  
  Continuously monitors the video feed and flags any movement.

- **In-Out Visitor Logging**  
  Tracks when people enter or leave the frame, with timestamps.

- **Video Recording**  
  Automatically records video clips when motion is detected.

- **Facial Recognition**  
  Uses OpenCV’s `haarcascade_frontalface_default.xml` to detect and log faces.

- **User Interface**  
  Simple GUI built in Tkinter to start/stop monitoring, view live feed, and browse logs.

## 📋 Repository Structure

smart-cctv-manager/
├── find_motion.py # Core motion-detection logic
├── motion.py # Frame-differencing and alert routines
├── record.py # Video capture & file-writing
├── in_out.py # Visitor in/out timestamp logging
├── haarcascade_frontalface_default.xml # Pretrained face detector
├── gui.py # Tkinter GUI launcher & controls
├── requirements.txt # Python dependencies
└── README.md # This file

## ⚙️ Installation

1. **Clone the repo**  
   ```bash
   git clone https://github.com/<your-username>/smart-cctv-manager.git
   cd smart-cctv-manager

   python3 -m venv venv
source venv/bin/activate   # on Windows: venv\Scripts\activate

pip install -r requirements.txt

🚀 Usage
Run the GUI

bash
Copy
Edit
python gui.py
Monitor & control

Start/stop live feed, enable motion detection, review recordings and logs.

Motion events trigger automatic recording clips in ./recordings/.

Visitor in/out timestamps are saved in ./logs/visitors.csv.

Facial Recognition

Detected faces are logged with timestamps in ./logs/faces.csv.

🛠️ Scripts Overview
find_motion.py – Implements background subtraction and frame differencing.

motion.py – Defines alert thresholds and motion-trigger callbacks.

record.py – Wraps OpenCV’s VideoWriter to save video segments.

in_out.py – Uses contour detection to decide when a person enters/exits the scene.

gui.py – Builds a Tkinter window, displays video frames, and wires up all controls.

📦 Dependencies
Listed in requirements.txt:

bash
Copy
Edit
opencv-python
numpy
Pillow
tkinter         # (usually included with standard Python installer)
Install via:

bash
Copy
Edit
pip install opencv-python numpy Pillow
