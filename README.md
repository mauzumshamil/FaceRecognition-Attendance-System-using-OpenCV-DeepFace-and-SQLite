# FaceRecognition Attendance System using OpenCV, DeepFace, and SQLite

## Introduction

The **FaceRecognition Attendance System** is an advanced solution designed to automate the process of recording attendance using facial recognition technology. This project leverages the capabilities of **OpenCV**, **DeepFace**, and **SQLite** to create a reliable and efficient attendance tracking system.

### Key Technologies

- **OpenCV**: Used for capturing and processing images from a webcam. OpenCV's robust image processing libraries enable accurate face detection in real-time.
- **DeepFace**: A powerful facial recognition library that identifies individuals by comparing captured images with a pre-existing database of known faces.
- **SQLite**: A lightweight database management system that stores attendance records, ensuring easy access and management of data.

### Project Overview

1. **Face Detection and Recognition**: 
    - The system uses a webcam to capture live video feeds and detect faces in real-time.
    - Detected faces are then recognized using the DeepFace library by matching them against a database of known faces.

2. **Attendance Logging**:
    - Upon successful recognition, the system logs the attendance details (name, date, and time) into an SQLite database.
    - This ensures that attendance records are accurately maintained and easily retrievable.

3. **User Interface**:
    - A simple graphical user interface (GUI) displays real-time attendance status, showing recognized faces and marking attendance automatically.
    - The system can also handle unrecognized faces by labeling them as "Unknown" and optionally sending alerts.

### Benefits

- **Efficiency**: Automates the attendance recording process, reducing manual effort and errors.
- **Accuracy**: Utilizes state-of-the-art facial recognition technology to ensure precise identification.
- **Scalability**: Easily expandable to accommodate more users and additional functionalities.

This project aims to demonstrate the integration of computer vision, machine learning, and database management to solve real-world problems effectively. The **FaceRecognition Attendance System** provides a robust and scalable solution for various environments, including schools, offices, and events.

## Summary

### Project Overview

The **FaceRecognition Attendance System** is designed to automate attendance tracking using facial recognition technology. This project integrates three key technologies: **OpenCV**, **DeepFace**, and **SQLite**. Below is a brief explanation of the code, its usage, and the advantages of this system.

### Code Explanation

1. **Environment Setup**:
    - Install the necessary libraries: OpenCV, DeepFace, and SQLite.
    - Initialize the SQLite database to store attendance records.

2. **Face Detection**:
    - Use OpenCV to capture images from the webcam.
    - Detect faces in real-time using OpenCV's Haar Cascade classifier.

3. **Face Recognition**:
    - Use DeepFace to compare detected faces with a database of known faces.
    - Identify the person and retrieve their name.

4. **Attendance Logging**:
    - Mark attendance by logging the recognized name, date, and time into the SQLite database.
    - Handle unrecognized faces by labeling them as "Unknown."

5. **User Interface**:
    - Display real-time video feed with detected and recognized faces.
    - Provide visual feedback by drawing rectangles around faces and displaying names.

### Usage

To use the system, follow these steps:

1. **Prepare Known Faces**:
    - Create a directory named `known_faces` and save images of individuals with filenames as their names (e.g., `Alice.jpg`, `Bob.jpg`).

2. **Run the System**:
    - Execute the Python notebook or script to start the webcam feed.
    - The system will automatically detect and recognize faces, logging attendance for recognized individuals.

3. **View Attendance Records**:
    - Attendance records are stored in the `attendance.db` SQLite database.
    - Use any SQLite viewer or command-line tool to query and view attendance logs.

### Pros

- **Efficiency**: The system automates attendance recording, saving time and reducing manual errors.
- **Accuracy**: Utilizes advanced facial recognition to ensure precise identification of individuals.
- **Scalability**: Easily expandable to include more users and additional features.
- **Real-Time**: Provides immediate feedback on attendance status with real-time face detection and recognition.

### Keywords

- **OpenCV**: An open-source computer vision library used for image processing and real-time video capture.
- **DeepFace**: A Python library for deep learning-based facial recognition, providing state-of-the-art accuracy in identifying faces.
- **SQLite**: A lightweight, disk-based database management system used to store attendance records.
- **Face Detection**: The process of identifying and locating human faces in images or video streams.
- **Face Recognition**: The process of comparing detected faces with a database of known faces to identify individuals.
- **Attendance Logging**: Recording the presence of individuals by logging their identity along with the date and time.

### Conclusion

The **FaceRecognition Attendance System** combines cutting-edge technologies to provide a robust and efficient solution for automating attendance tracking. By leveraging OpenCV for real-time face detection, DeepFace for accurate face recognition, and SQLite for reliable data storage, this system addresses the needs of various environments such as schools, offices, and events. Its ease of use, accuracy, and scalability make it a valuable tool for modern attendance management.
