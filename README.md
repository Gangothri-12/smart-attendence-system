# smart-attendence-system
# 🎓 Smart Attendance System using Face Recognition

This project is a **Smart Attendance System** that uses **face recognition** to automate the process of taking attendance in classrooms or organizations. It utilizes **OpenCV**, **dlib**, and the **face_recognition** library in Python.

---

## 📁 Folder Structure

SmartAttendanceSystem/
│
├── students/ # Stores student images
├── register.py # Captures and stores face images
├── generate_encodings.py # Creates facial encodings
├── recognize.py # Marks attendance using face recognition
├── attendance.csv # Stores attendance log
└── encodings.pkl # Serialized face encodings

---

## 🚀 How It Works

1. **Run `register.py`**  
   Captures 5 images of each student from the webcam and stores them in the `students/` folder.

2. **Run `generate_encodings.py`**  
   Extracts and encodes face data from the images and stores it in a file `encodings.pkl`.

3. **Run `recognize.py`**  
   Opens webcam, recognizes registered faces in real-time, and logs attendance in `attendance.csv`.

---

## 🧠 Technologies Used

- Python 3.8+
- OpenCV
- face_recognition
- dlib
- pickle

---

## ⚙️ Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/SmartAttendanceSystem.git
   cd SmartAttendanceSystem
Install dependencies:
pip install opencv-python face_recognition
Make sure you have dlib installed (can be tricky on Windows).
You can download a precompiled .whl for your Python version from Gohlke’s site.

 Output
The output is stored in attendance.csv in this format:
Name, Date, Time
Ravi, 2025-07-07, 10:42:33
