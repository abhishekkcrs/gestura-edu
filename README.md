# ✋ Gesture Detection System

A real-time gesture recognition system using hand landmarks and Dynamic Time Warping (DTW). Lightweight and efficient — no deep learning models required. Define gestures on-the-fly and link them to commands for intuitive interaction.

---

## 📘 Table of Contents
1. [Introduction](#1-introduction)  
2. [System Requirements](#2-system-requirements)  
3. [Installation and Running Instructions](#3-installation-and-running-instructions)  
4. [Gesture Matching Algorithm](#4-gesture-matching-algorithm)  
5. [Complexity Analysis](#5-complexity-analysis)  
6. [Conclusion](#6-conclusion)  
7. [Future Improvements](#7-future-improvements)  

---

## 1. Introduction

This system provides a **real-time gesture recognition interface** using **MediaPipe hand landmarks** and **FastDTW**. It is:
- Lightweight and efficient (no deep learning model required)
- Customizable with on-the-fly gesture recording
- Ideal for hands-free desktop interactions or educational applications

---

## 2. System Requirements

### 🧑‍💻 Software

- Python 3.x

### 🧩 Python Libraries

| Library | Version | Description |
|--------|---------|-------------|
| `mediapipe` | 0.10.21 | Hand gesture detection & tracking |
| `numpy` | 1.26.4 | Numerical operations |
| `opencv-contrib-python` | 4.11.0.86 | Image & video processing |
| `fastdtw` | 0.3.4 | Fast Dynamic Time Warping |
| `scipy` | 1.15.2 | Scientific computation |
| `matplotlib` | 3.10.1 | Debugging & visualization |
| `jsonschema` | 4.23.0 | JSON format validation |
| `pillow` | 11.1.0 | Image handling |
| `customtkinter` | 5.2.2 | GUI components |
| `PyAutoGUI` | 0.9.54 | Mouse & keyboard simulation |
| `fastapi` | 0.115.11 | Backend API server |
| `requests` | 2.32.3 | HTTP request handler |
| `python-dotenv` | 1.0.1 | Environment variable management |

### 🖥️ Hardware

- CPU (GPU optional)
- Webcam (for real-time input)

---

## 3. Installation and Running Instructions

### 3.1 Directory Structure

gesture-edu/
├── assets/
│ └── gesturalogo.png
├── backend/
│ ├── gestures.json
│ ├── lessons.py
│ ├── lessons_endpoint.py
│ ├── main.py
│ ├── secret.env
│ └── venv/
├── index.html
├── playground.html
├── predictor.html
├── scripts.js
├── styles.css
├── .gitignore
└── README.md


### 3.2 Backend Setup

```bash
cd your/extracted/location/gesture-edu
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
