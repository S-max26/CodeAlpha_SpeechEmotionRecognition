# Speech Emotion Recognition using Deep Learning

## 📌 Project Overview

Speech Emotion Recognition (SER) is a Deep Learning-based application that identifies human emotions from speech audio recordings. The system extracts MFCC (Mel Frequency Cepstral Coefficients) features from audio signals and uses an LSTM (Long Short-Term Memory) neural network to classify emotions.

The application provides an interactive Gradio web interface where users can upload or record audio and receive real-time emotion predictions.

---

## 🎯 Features

* Detects emotions from speech audio
* Uses MFCC feature extraction
* LSTM-based Deep Learning model
* Real-time emotion prediction
* User-friendly Gradio interface
* Supports audio upload and microphone recording

---

## 🧠 Emotions Detected

The model can classify speech into the following emotions:

* Angry 😠
* Calm 😌
* Disgust 🤢
* Fearful 😨
* Happy 😄
* Neutral 😐
* Sad 😢
* Surprised 😲

---

## 🛠️ Technologies Used

* Python 3.10
* TensorFlow 2.13.0
* Keras 2.13.1
* Librosa
* NumPy
* Gradio
* Resampy
* SoundFile

---

## 📂 Project Structure

```text
CodeAlpha_SpeechEmotionRecognition/
│
├── emotion_app.py
├── speech_emotion_lstm_model.h5
├── requirements.txt
├── README.md
│
├── gradio_app.ipynb
├── gui.ipynb
└── SPEECH RECOGNITION LSTM DL.ipynb
```

---

## ⚙️ Installation

### 1. Clone the Repository

```bash
git clone <repository-link>
cd CodeAlpha_SpeechEmotionRecognition
```

### 2. Create Virtual Environment

```bash
python -m venv venv
```

### 3. Activate Virtual Environment

Windows:

```bash
venv\Scripts\activate
```

### 4. Install Dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Run the Application

```bash
python emotion_app.py
```

After running the command, Gradio will generate a local URL similar to:

```text
http://127.0.0.1:7860
```

Open the URL in your browser.

---

## 🔍 How It Works

1. User uploads or records an audio sample.
2. Audio is processed using Librosa.
3. MFCC features are extracted from the speech signal.
4. Features are padded to a fixed size.
5. The trained LSTM model predicts the emotion.
6. The predicted emotion is displayed on the Gradio interface.

---

## 📊 Model Architecture

```text
Input Layer (174 × 40)

↓
LSTM (128 Units)

↓
Dropout (0.3)

↓
Dense (64 Units, ReLU)

↓
Dropout (0.3)

↓
Dense (8 Units, Softmax)
```

---

## 🚀 Future Improvements

* Improve model accuracy with larger datasets
* Add confidence visualization charts
* Support multilingual emotion recognition
* Deploy as a cloud-based web application
* Add real-time streaming emotion analysis

---

## 📷 Demonstration

1. Launch the application.
2. Upload or record an audio sample.
3. Click Submit.
4. View the detected emotion instantly.

---

## 👨‍💻 Internship Project

This project was developed as part of the **CodeAlpha Internship Program** to demonstrate the application of Deep Learning techniques in Speech Emotion Recognition.

---

## 📜 License

This project is intended for educational and learning purposes.

Developed by: Sanjana Barui
CodeAlpha Internship Project
