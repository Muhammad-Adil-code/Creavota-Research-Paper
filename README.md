Automated School Attendance and Uniform Detection System
This repository contains the proposal and development materials for an Automated School Attendance and Uniform Detection System. The project aims to enhance administrative efficiency in educational institutions by leveraging computer vision for real-time student monitoring. 

📜 Project Overview
Manual attendance and uniform checks are often time-consuming and prone to errors.  This system automates these processes using real-time face recognition for attendance and object detection for uniform compliance verification.  The goal is to streamline administrative tasks through a centralized, web-based dashboard. 



✨ Key Features
Real-Time Face Recognition: Automates student attendance by identifying faces.
Uniform Compliance Detection: Uses a custom-trained YOLOv8 model to verify school uniforms. 
Robust Performance: Designed to operate effectively in various lighting conditions. 
Centralized Dashboard: A web interface provides live data on student attendance and attire status.
⚙️ Proposed Methodology
System Design
The system is designed with four core components that work together to provide a seamless monitoring experience:

Face Data Management: Student facial feature vectors are pre-loaded and stored in a MongoDB database. 
Recognition Pipeline: The system uses Haar Cascade detection and vector matching to verify a student's identity in real-time. 
Uniform Detection: A YOLOv8 object detection model, trained on school-specific attire, classifies uniform compliance. 
Dashboard Display: Live data, including student name, section, and uniform status, is presented on a user-friendly dashboard.
Development Plan
The development is planned in the following stages:

Capture a diverse dataset of student images in various lighting conditions. 
Preprocess images and encode facial features into storable vectors.
Store and manage facial data using MongoDB. 
Train the YOLOv8 model with a labeled dataset of school uniforms. 
Integrate the recognition and detection pipelines with a responsive user interface. 
🛠️ Tools & Technologies
Languages: Python, JavaScript
Libraries: OpenCV, PyTorch, face_recognition, Ultralytics YOLO
Database: MongoDB
Frameworks: Flask / Django
🎯 Expected Results
Facial Recognition Accuracy: Expected to exceed 95%. 
Uniform Detection Precision: Anticipated to be over 90%. 
Response Time: System response time is estimated to be under one second for real-time operation. 
Potential challenges include variations in lighting, partial uniform occlusion, and facial obstructions, which will be addressed through iterative development. 

📊 Current Status
The project is currently under active development. Key activities in progress include dataset creation, storing face vectors, and training the initial YOLOv8 model. 

🚀 Future Work
Future enhancements may include:

Mobile compatibility for on-the-go monitoring.
Advanced behavioral analysis features.
Cloud-based reporting tools for administrators.
