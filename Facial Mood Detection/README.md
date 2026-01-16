Facial Mood Detection System
--Project Overview
This project is an automated system designed to recognize human emotions from facial expressions in real-time. It uses a custom-built Convolutional Neural Network (CNN) to classify faces into seven distinct mood categories: Angry, Disgust, Fear, Happy, Sad, Surprise, and Neutral.
The primary goal is to demonstrate fundamental computer vision techniques and deep learning implementation using Python, OpenCV, and TensorFlow.

--Key Features
Real-Time Detection: Processes live webcam feeds at high frame rates.
Live Probability Chart: Displays a dynamic bar chart showing the AI's confidence levels for all 7 emotions simultaneously.
Robust Face Tracking: Utilizes Haar Cascade classifiers for reliable face location even in varying lighting conditions.
Efficient Preprocessing: Automatically crops, grayscales, and normalizes facial regions of interest (ROI) for optimized model performance.

--Technology Stack
Programming Language: Python
Computer Vision: OpenCV
Deep Learning Framework: TensorFlow / Keras
Data Processing: NumPy

--Project Structure
Plaintext
.
├── model/
│   ├── fer.h5              # Pre-trained CNN weights
│   └── fer.json            # Model architecture configuration
├── face_detect.py          # Basic face detection script
├── mood_detect.py          # Main real-time emotion recognition script
├── requirements.txt        # List of dependencies
└── .gitignore              # Files to be excluded from GitHub

--Setup & Installation
Follow these steps to set up the project on your machine:

Clone the Repository:
Bash
git clone https://github.com/your-username/facial-mood-detection.git
cd facial-mood-detection
Create and Activate a Virtual Environment:

Bash
python -m venv facial_env
# Windows:
.\facial_env\Scripts\activate
Install Dependencies:

Bash
pip install -r requirements.txt
📖 How to Run
Once installed, launch the system with your webcam:

Bash
python mood_detect.py
Controls: Point your face at the camera to see the detected emotion and the probability bars.

Exit: Press the 'q' key to close the application.
