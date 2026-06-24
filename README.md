Click here for the project code: https://drive.google.com/drive/folders/1FExMxxGRMSdY0T5B92kVmcH0ktJS48Pk?usp=drive_link
# Real-Time Skin Tone Detection with Deep Learning & Django

<img width="1612" height="881" alt="Screenshot 2026-06-24 182300" src="https://github.com/user-attachments/assets/b3cabac7-1c10-4829-b160-bf81d4e87e75" />


## Overview


Real-Time Skin Tone Detection is an AI-powered web application that detects and classifies human skin tones from uploaded images or real-time webcam input. The system leverages a custom-trained Convolutional Neural Network (CNN) built using TensorFlow/Keras to analyze facial skin regions and predict one of ten predefined skin tone categories.

The project combines Deep Learning, Computer Vision, and Web Development technologies to provide an interactive and user-friendly platform for skin tone analysis and personalized makeup recommendations.

---

## Features

### Skin Tone Classification

* Detects skin tone from uploaded facial images.
* Supports real-time webcam-based prediction.
* Classifies users into 10 skin tone categories:

  * Porcelain
  * Ivory
  * Fair
  * Light Beige
  * Beige
  * Tan
  * Honey
  * Caramel
  * Mocha
  * Ebony

### Deep Learning Powered

* Custom CNN model trained using TensorFlow/Keras.
* Optimized for skin tone classification tasks.
* Fast and accurate predictions.

### Computer Vision Integration

* Image preprocessing using OpenCV and Pillow.
* Facial image handling and enhancement before prediction.

### Makeup Recommendation System

* Recommends makeup products based on detected skin tone.
* Uses a curated dataset containing product links and recommendations.

### User-Friendly Interface

* Built using Django and Bootstrap.
* Responsive design for desktop and mobile devices.
* Displays predicted skin tone along with recommendations.

### Deployment Ready

* Easily deployable on Render, Heroku, AWS, or DigitalOcean.

---

## Technology Stack

### Backend

* Python
* Django

### Deep Learning

* TensorFlow
* Keras

### Computer Vision

* OpenCV
* Pillow

### Data Processing

* NumPy
* Pandas

### Frontend

* HTML
* CSS
* Bootstrap
* JavaScript

### Database

* SQLite

---

## System Workflow

```text
User Uploads Image / Webcam Capture
                │
                ▼
      Image Preprocessing
      (OpenCV + Pillow)
                │
                ▼
       Face Detection
                │
                ▼
     CNN Model Prediction
      (TensorFlow/Keras)
                │
                ▼
     Skin Tone Classification
                │
                ▼
 Makeup Recommendation Engine
                │
                ▼
      Display Results in UI
```

---

## Project Structure

```text
Real-Time-Skin-Tone-Detection/
│
├── static/                         # CSS, JavaScript, Images
├── media/                          # Uploaded images
│
├── product_rec/                    # Django Application
│   ├── migrations/
│   ├── templates/
│   │   └── product_rec/
│   ├── admin.py
│   ├── apps.py
│   ├── models.py
│   ├── tests.py
│   ├── views.py
│   ├── urls.py
│   └── __init__.py
│
├── makeup_recommendation/          # Django Project
│   ├── settings.py
│   ├── urls.py
│   ├── asgi.py
│   ├── wsgi.py
│   └── __init__.py
│
├── Skin_tone_detect.h5             # Trained CNN Model
├── skin_data_with_links.csv        # Makeup Recommendation Dataset
├── real time detection.ipynb       # Model Training Notebook
├── db.sqlite3                      # SQLite Database
├── manage.py
├── requirements.txt
├── README.md
└── .gitignore
```

---

## Dataset

The model was trained on a skin tone dataset containing labeled facial images categorized into ten skin tone classes.

### Data Preparation

* Image resizing
* Image normalization
* Data augmentation
* Train-test split
* Label encoding

### Output Classes

```text
Porcelain
Ivory
Fair
Light Beige
Beige
Tan
Honey
Caramel
Mocha
Ebony
```

---

## Model Architecture

The CNN model includes:

* Convolution Layers
* ReLU Activation Functions
* Max Pooling Layers
* Dropout Layers
* Fully Connected Dense Layers
* Softmax Output Layer

### Training Configuration

```python
Optimizer = Adam
Loss Function = Categorical Crossentropy
Batch Size = 32
Epochs = 25-50
Metrics = Accuracy
```

---

## Installation

### Clone Repository

```bash
git clone https://github.com/yourusername/real-time-skin-tone-detection.git
cd real-time-skin-tone-detection
```

### Create Virtual Environment

```bash
python -m venv venv
```

Activate Environment

Windows:

```bash
venv\Scripts\activate
```

Linux/Mac:

```bash
source venv/bin/activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Run Migrations

```bash
python manage.py migrate
```

### Start Server

```bash
python manage.py runserver
```

Open your browser:

```text
http://127.0.0.1:8000
```

---

## Applications

### Beauty Industry

* Foundation shade matching
* Personalized cosmetic recommendations

### Skincare Platforms

* Customized skincare suggestions
* Beauty consultation systems

### E-Commerce

* Smart product recommendation engines
* Virtual beauty assistants

### Research & AI

* Inclusive beauty technology
* Computer vision applications in cosmetics

---

## Future Enhancements

* Skin Undertone Detection
* Advanced Makeup Shade Matching
* Skincare Product Recommendation
* Mobile Application Development
* REST API Integration
* Multi-Face Detection Support
* Real-Time Video Stream Analysis

---

## Results

The application successfully predicts skin tones from uploaded images and live webcam feeds while providing relevant makeup recommendations through a responsive Django web interface.

---

## Author

**Fathima Azeez**

Data Science Trainer | Python Developer | AI & Computer Vision Enthusiast

LinkedIn: Add Your LinkedIn Profile

GitHub: Add Your GitHub Profile

---

## License

This project is licensed under the MIT License.

Feel free to use, modify, and contribute to this project.
