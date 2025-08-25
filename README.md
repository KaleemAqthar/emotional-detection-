# Emotion Detection using Deep Learning and OpenCV
## Overview
This project is an **Emotion Detection System** that uses a pre-trained deep learning model to recognize human emotions from live webcam video feed. The system 
detects faces using OpenCV’s Haar Cascade Classifier and classifies emotions using a CNN model trained on facial expression datasets. It also displays real-time
probability bars for each emotion.
## Features

* Real-time face detection using OpenCV.
* Emotion classification using a pre-trained Keras model (`_mini_XCEPTION.102-0.66.hdf5`).
* Displays seven emotion categories: **Angry, Disgust, Fear, Happy, Sad, Surprise, Neutral**.
* Visualizes probabilities with a colored bar graph UI.
* Live webcam feed integration.

## Technologies Used

* **Python 3.8+**
* **OpenCV** for face detection and image processing.
* **TensorFlow/Keras** for deep learning model loading and prediction.
* **NumPy** for array manipulation.

## Installation

1. **Clone the repository** or copy the project files.
2. **Install dependencies**:

   ```bash
   pip install opencv-python tensorflow keras numpy
   ```
3. **Download the pre-trained model file** (`_mini_XCEPTION.102-0.66.hdf5`) and place it in the project directory.
4. Ensure the Haar Cascade XML file is available (comes with OpenCV by default).

## How to Run

1. Connect your webcam.
2. Run the Python script:

   ```bash
   python emotion_detection.py
   ```
3. The application will open a window showing:

   * Webcam feed with face bounding boxes and predicted emotion label.
   * A probability bar chart for all emotions on the right side.
4. Press **'q'** to quit the application.

## Project Structure

```
emotion_detection/
│
├── emotion_detection.py        # Main script
├── _mini_XCEPTION.102-0.66.hdf5 # Pre-trained model file
└── README.md                   # Project documentation
```
## Future Enhancements
* Add dataset training code for custom datasets.
* Deploy as a web app using Streamlit or Flask.
* Integrate with IoT or mobile devices for real-time monitoring.
## Notes
* Make sure your camera drivers are working properly.
* The pre-trained model must match the expected input size (64x64 grayscale images).
