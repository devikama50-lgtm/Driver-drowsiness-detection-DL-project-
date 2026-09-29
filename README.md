# Driver Drowsiness Detection

A Deep Learning-based system for detecting driver drowsiness using facial landmarks and eye/mouth movements.

## Features

* Real-time face and facial landmark detection
* Eye Aspect Ratio (EAR) for detecting eye closure
* Mouth Aspect Ratio (MAR) for detecting yawning
* LSTM-based drowsiness classification
* OpenCV for real-time video processing
* Alert when prolonged drowsiness is detected

## Technologies Used

* Python
* TensorFlow / Keras
* OpenCV
* MediaPipe
* NumPy
* Pandas
* Scikit-learn

## Project Workflow

```text
Camera / Video
      ↓
Face Detection
      ↓
Facial Landmark Detection
      ↓
EAR & MAR Calculation
      ↓
Feature Extraction
      ↓
LSTM Model
      ↓
Drowsiness Detection
      ↓
Alert
```

## Dataset

The model is trained using facial landmark features extracted from driver images/video frames. The dataset contains features related to eye closure and mouth movement for classifying drowsy and non-drowsy states.

## Model

An **LSTM (Long Short-Term Memory)** model is used to learn temporal patterns from facial landmark features and classify the driver's state.

## How to Run

### 1. Clone the repository

```bash
git clone <your-repository-link>
cd <project-folder>
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Run the project

```bash
python app.py
```

## Project Structure

```text
Driver-Drowsiness-Detection/
│
├── dataset/
├── model/
├── notebooks/
├── app.py
├── requirements.txt
├── README.md
└── .gitignore
```

## Applications

* Driver safety systems
* Automotive monitoring
* Real-time fatigue detection
* Intelligent transportation systems

## Future Improvements

* Integrate an audible warning system
* Improve detection under different lighting conditions
* Deploy the model as a real-time web application
* Integrate with vehicle safety systems
