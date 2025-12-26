# ASL Recognition System

## Overview
The **ASL Recognition System** is a Python-based desktop application that recognizes **American Sign Language (ASL) gestures** in real-time using a webcam. 
It converts hand gestures into readable text, enabling effective communication for the deaf and mute community. 
This project demonstrates practical use of **computer vision, deep learning, and GUI development** in Python.

---

## Key Features
- **Real-Time Gesture Recognition** – Detects ASL letters and commands like `Space`, `Delete`, and `Nothing` using a trained deep learning model.  
- **Word Formation** – Forms words dynamically by combining recognized letters, with the ability to delete the last letter or clear the entire word.  
- **Interactive GUI** – Built with `customtkinter` for a modern, user-friendly interface displaying video feed, predictions, and the current word.  
- **Stable Predictions** – Implements smoothing logic to ensure consistent recognition before updating the word.  
- **Python-Powered Solution** – Combines `OpenCV`, `TensorFlow/Keras`, `NumPy`, `Pillow`, and threading for smooth real-time performance.

---

## How It Works
1. **Capture Video** – Uses OpenCV to access the webcam feed.  
2. **Region of Interest (ROI)** – Focuses on the area of the frame where hand gestures appear.  
3. **Preprocessing** – Resizes and normalizes the ROI before feeding it into the model.  
4. **Prediction** – Uses the trained Keras model (`ASL2.h5`) to classify gestures.  
5. **Smoothing Mechanism** – Adds gestures to the word only if predicted consistently for multiple frames.  
6. **Display** – Updates the GUI with the current word and predicted label while handling commands like `Space` and `Delete` intelligently.

---

## GUI Functionalities
- **Start Prediction** – Initiates real-time gesture recognition.  
- **Stop Prediction** – Stops the prediction loop safely.  
- **Delete Last Letter** – Removes the last letter from the current word.  
- **Clear Word** – Clears the entire word from the display.  
- **Keyboard Backspace** – Provides additional keyboard control to delete letters.

---

## Technologies Used
- **Python 3.x** – Core programming language.  
- **OpenCV** – Real-time video capture and image processing.  
- **TensorFlow / Keras** – Deep learning model for gesture recognition.  
- **NumPy** – Numerical operations and preprocessing.  
- **Pillow (PIL)** – Image conversion for GUI display.  
- **customtkinter** – Desktop GUI framework.  
- **Threading** – Ensures non-blocking real-time prediction.

---

## Learning Outcomes
- Applied **computer vision techniques** to capture and process live video feed.  
- Built a **deep learning pipeline** for accurate gesture recognition using Keras.  
- Developed a **real-time GUI** integrating predictions with user interactions.  
- Implemented **prediction smoothing logic** to enhance recognition stability.  
- Gained hands-on experience in **Python application development** combining ML, image processing, and GUI design.

---

## Future Enhancements
- Integrate **text-to-speech** functionality for the formed word.  
- Expand gesture vocabulary to recognize **full sentences and phrases**.  
- Optimize model for **higher prediction speed and accuracy**.  
- Deploy as a **cross-platform mobile application** for wider accessibility.

---

## Author
**Shafi S** – Backend-focused Python developer with expertise in **computer vision, deep learning, and interactive GUI applications**.

---

## License
This project is licensed under the MIT License.
