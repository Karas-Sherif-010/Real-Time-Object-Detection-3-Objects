# Real-Time Multi-Class Object Detection

A real-time multi-class object detection project built using custom data, **YOLO26**, and **RT-DETR**.

The project covers the complete pipeline from data collection and annotation to model training and real-time camera detection.

---

## 📌 Project Overview

The dataset was personally collected using objects available in a home environment.

The collected images were prepared and annotated using **Roboflow** with the assistance of **SAM 3**. Preprocessing, data augmentation, and negative samples were applied before training.

Two object detection models were trained and tested:

* **YOLO26**
* **RT-DETR**

The trained models were then used for **real-time object detection through a webcam**.

---

## 🔄 Project Pipeline

```text
Data Collection
       ↓
Dataset Preparation
       ↓
Annotation with SAM 3
       ↓
Preprocessing
       ↓
Data Augmentation
       ↓
Negative Samples
       ↓
Model Training
       ↓
Model Testing
       ↓
Real-Time Camera Detection
```

---

## 🗂️ Dataset

The dataset was collected manually using real objects available in the home environment.

Images were captured with variations in:

* Object position
* Object size
* Background
* Lighting
* Camera angle

This helped create a more diverse dataset for real-world detection.

---

## 🏷️ Annotation

**Roboflow** was used for dataset preparation and annotation.

**SAM 3** was used to assist with the annotation process.

The annotated dataset was prepared in a suitable format for object detection training.

---

## 🛠️ Data Preparation

The dataset preparation process included:

* Image preprocessing
* Label preparation
* Dataset organization
* Data augmentation
* Negative samples

### Negative Samples

Negative samples are images that do not contain any target objects.

They were included to help the models distinguish between target objects and background scenes and reduce false positive detections.

---

## 🤖 Models

### YOLO26

YOLO26 was trained on the custom dataset and tested for real-time object detection.

The trained model weights are included in the repository.

### RT-DETR

**RT-DETR (Real-Time Detection Transformer)** was also trained using the custom dataset.

It was used as a transformer-based object detection approach and tested with real-time camera input.

---

## 📷 Real-Time Detection

The trained models were tested using a live webcam.

The detection process follows:

```text
Webcam
   ↓
Video Frame
   ↓
Object Detection Model
   ↓
Bounding Boxes
   ↓
Class Labels
   ↓
Confidence Scores
   ↓
Live Detection
```

For every camera frame, the model predicts the detected objects and displays their bounding boxes, class labels, and confidence scores.

---

## 🧪 Testing

The models were tested using real-world camera input.

The testing focused on:

* Object detection
* Class prediction
* Bounding box localization
* Confidence scores
* Real-time inference

Both YOLO26 and RT-DETR were successfully tested for real-time detection.

---

## 📁 Repository Structure

```text
Real-Time-Object-Detection/
│
├── Object_Detection Notebook.ipynb
├── test_withCamera.ipynb
│
├── YOLO26n_best.pt
├── rt-deter_best.pt
│
└── README.md
```

> Model filenames may differ depending on the final repository version.

---

## 💻 Technologies

* Python
* PyTorch
* OpenCV
* Ultralytics
* YOLO26
* RT-DETR
* Roboflow
* SAM 3
* NumPy

---

## ▶️ How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/Karas-Sherif-010/Real-Time-Object-Detection.git
```

### 2. Navigate to the Project

```bash
cd Real-Time-Object-Detection
```

### 3. Open the Camera Notebook

Open:

```text
test_withCamera.ipynb
``
```
