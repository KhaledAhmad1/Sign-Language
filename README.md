## Gesture Recognition System

### Overview
This project implements a real-time hand gesture recognition system using computer vision and machine learning techniques. The system captures hand gestures through a webcam, processes them using the MediaPipe library for hand tracking, and then classifies the gestures using a trained machine learning model.

### Usage Instructions

1. **Data Collection:**
   - Run the script `data_collection.py` to collect hand gesture data. This script captures images from your webcam and saves them in the data directory.

2. **Hand Initialization:**
   - Run the script `create_dataset.py`. This script initializes a hand tracking model using MediaPipe, loads images using OpenCV, and converts them to RGB format. It then saves the collected data and labels in a file named 'data.pickle'.

3. **Model Training:**
   - Run the script `train_model.py` to train the machine learning model using the collected data. This script trains a RandomForestClassifier using the hand gesture data.

4. **Real-time Gesture Recognition:**
   - Run the script `inference_classifier.py` to perform real-time hand gesture recognition. This script uses the trained model and MediaPipe to recognize hand gestures captured from your webcam.

5. **Follow the On-screen Instructions:**
   - Hold your hand in front of the webcam.
   - Make different gestures to see the predicted characters displayed on the screen.
   - Press 'Q' to exit the program.

6. **Adjustments:**
   - Feel free to modify the code to experiment with different machine learning models, data collection techniques, or gesture recognition algorithms.

### Requirements
- Python 3.x
- OpenCV
- Mediapipe
- Scikit-learn
- Matplotlib (optional)

### Credits
This project utilizes the MediaPipe library developed by Google for hand tracking, as well as scikit-learn for machine learning tasks.

### License
This project is licensed under the [MIT License](LICENSE).
