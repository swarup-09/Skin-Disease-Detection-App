# 🩺 Skin Disease Detection App

An Android + Flask-based system that allows users to upload skin images and receive predictions about potential skin diseases using a trained machine learning model.

## 📱 Android Frontend

### Features:
- Capture image via camera or upload from gallery.
- Sends image to Flask server using Retrofit.
- Displays prediction and confidence score.
- Handles error cases gracefully.

### Tech Stack:
- Kotlin
- Retrofit for API communication
- One activity: MainActivity (image input & result display)

---

## 🧠 Flask Backend

### Features:
- Receives image via POST request (`http://127.0.0.1:5000/predict` endpoint).
- Loads pre-trained ML model using TensorFlow/Keras.
- Processes the image and returns:
  - Predicted disease
  - Confidence score
  - Success status

### Requirements:
- Flask
- TensorFlow / Keras
- Pillow, NumPy, Flask-CORS

### Run Server:
```bash
pip install -r requirements.txt
python predict_image.py

