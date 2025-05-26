# smart-cctv-tkinter
This is a tkinter gui app for smart camera.


you just need to run main.py file inorder to run full app 

you would need :
opencv
tkinter

installed to run these scripts properly

Thank You !

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
