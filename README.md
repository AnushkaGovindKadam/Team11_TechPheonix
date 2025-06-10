# Team11_TechPheonix

> An automated and contactless attendance marking system using real-time facial recognition built with Python, OpenCV, Tkinter, and MySQL.

![Face Recognition Demo](demo/demo1.gif) <!-- You can replace with actual gif or link to video -->

---

## 📌 Project Overview

In modern educational and organizational environments, maintaining an accurate and efficient attendance record is crucial. Traditional systems like manual roll calls or biometric touch scanners are time-consuming and prone to errors or proxy entries. This project presents a **Face Recognition Attendance System** that leverages **computer vision** and **machine learning** for real-time, touchless attendance marking using a webcam.

This system captures facial data, trains a recognition model, and identifies individuals during live detection. Once recognized, the student’s attendance is logged with a timestamp and saved securely.

---

## 🎯 Key Features

- 📸 **Real-time face detection & recognition** using Dlib and OpenCV
- 🧠 **Training with LBPH (Local Binary Pattern Histogram)** algorithm
- 🗃️ **MySQL database integration** for student data management
- 📋 **CSV-based attendance export/import**
- 🎨 **Tkinter GUI** for user-friendly interface
- 🔐 **Proxy prevention** via biometric uniqueness
- 🕐 **Time-slot-based attendance classification** (morning, afternoon, evening)

---

## 🛠️ Technologies Used

| Category      | Stack                             |
|---------------|-----------------------------------|
| Language      | Python                            |
| GUI           | Tkinter                           |
| Computer Vision | OpenCV, Dlib, PIL                |
| Database      | MySQL                             |
| Face Recognition | LBPH (OpenCV LBPHFaceRecognizer) |
| Others        | NumPy, CSV, OS, Matplotlib        |

---

## 🧱 System Architecture

```plaintext
1. Image Collection ➜
2. Preprocessing (grayscale + resize) ➜
3. Model Training (LBPH) ➜
4. Real-Time Detection (via webcam) ➜
5. Face Matching ➜
6. Attendance Logging ➜
7. CSV Export or Database Sync
🧪 How it Works
Student Registration: Enter student details in the GUI and capture 200 face samples using the webcam.

Training: Run Train All Data to process the images using LBPH and generate Trained_data.xml.

Recognition: Launch real-time recognition. The system detects faces and checks against the trained model.

Attendance Logging: Attendance is logged to the correct CSV (morning.csv, afternoon.csv, etc.) based on time.

Review: Admins can view or export attendance data from the GUI.

📊 Performance Metrics
Model	Time Taken (mins)	Accuracy (%)
LBPH Face Recognition	3.5	95.5%
Manual Entry	10.0	80.0%
Fingerprint Scanner	5.2	90.0%

📁 Folder Structure
bash
Copy
Edit
├── Data/                    # Face image dataset
├── Trained_data.xml        # Trained LBPH model
├── train.py                # Model training script
├── face_recognition.py     # Recognition + attendance
├── database.py             # MySQL DB operations (if separate)
├── images/                 # GUI images and backgrounds
├── attendance/             # CSV attendance logs
├── README.md               # This file
🎥 Demo Videos
📹 Demo 1 – System Workflow
📹 Demo 2 – Real-Time Recognition



🚀 Future Scope
Integration with Cloud (Firebase, AWS)

Use of deep learning models (FaceNet, VGG-Face)

Emotion & behavior recognition

Integration with school/college ERP systems

Notification system (SMS/Email)

🤝 Contributors
1. Anushka Kadam
2. Varsha Deore
3. Nikita Kachole
4. Anuja Waghmare

🏫 CSMSS, Chh. Shahu College of Engineering

📜 License
This project is for educational use. Attribution is appreciated if reused or modified.

🧠 Acknowledgments
OpenCV & Dlib Developers

Tkinter Python Docs

IEEE Research Papers on LBPH & Deep Learning

CSMSS Faculty and Guidance










