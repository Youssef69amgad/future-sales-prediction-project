# ASL Hand Gestures Recognition

A real-time American Sign Language (ASL) hand gesture recognition system that detects hand gestures from a webcam and converts them into readable text. The project uses computer vision and deep learning to recognize hand signs and support real-time interaction.

## Overview

This project is designed to recognize ASL hand gestures using a trained deep learning model. It captures hand movements through a camera, processes the hand landmarks, predicts the corresponding gesture, and displays the result as text.

The system can be useful as an assistive technology concept for improving communication accessibility for people who use sign language.

## Features

* Real-time hand gesture recognition using webcam input
* ASL gesture classification using a trained deep learning model
* Hand landmark detection and preprocessing
* Live prediction interface
* Converts recognized gestures into text
* Simple and easy-to-run Python implementation

## Technologies Used

* Python
* TensorFlow / Keras
* OpenCV
* MediaPipe
* NumPy
* Computer Vision
* Deep Learning

## Project Structure

```text
ASL-hand-gestures-recognition/
│
├── live_app.py                  # Main real-time recognition application
├── final.py                     # Final prediction / application script
├── prediction_wo_gui.py          # Prediction script without GUI
├── data_collection_binary.py     # Data collection script
├── data_collection_final.py      # Final data collection script
├── cnn8grps_rad1_model.h5        # Trained deep learning model
├── hand_landmarker.task          # Hand landmark detection model/task file
├── requirements_live.txt         # Required Python libraries
└── README.md
```

## How It Works

1. The webcam captures live video frames.
2. The hand is detected from the video stream.
3. Hand landmarks are extracted and processed.
4. The trained deep learning model predicts the gesture class.
5. The predicted sign is displayed as text in real time.

## Installation

### 1. Clone the Repository

```bash
git clone https://github.com/Youssef69amgad/ASL-hand-gestures-recognition.git
cd ASL-hand-gestures-recognition
```

### 2. Create a Virtual Environment

```bash
python -m venv venv
```

Activate the environment:

For Windows:

```bash
venv\Scripts\activate
```

For macOS/Linux:

```bash
source venv/bin/activate
```

### 3. Install Requirements

```bash
pip install -r requirements_live.txt
```

## Usage

Run the real-time application:

```bash
python live_app.py
```

Or run the final script:

```bash
python final.py
```

Make sure your webcam is connected and allowed to be used by Python/OpenCV.

## Model

The project uses a trained CNN-based model saved as:

```text
cnn8grps_rad1_model.h5
```

The model is used to classify hand gestures based on processed hand landmark or image input.

## Notes

* Good lighting improves recognition accuracy.
* The hand should be clearly visible to the camera.
* The model performance may vary depending on background, hand position, and camera quality.
* If the model file is too large for GitHub, it can be uploaded using Git LFS or stored externally with a download link added to this README.

## Future Improvements

* Improve model accuracy with more training data
* Add support for more ASL gestures
* Build a cleaner graphical user interface
* Add text-to-speech output
* Improve sentence formation from detected gestures
* Deploy the system as a desktop or web application

## Author

Developed by **Youssef Amgad**

## License

This project is for educational and research purposes.
