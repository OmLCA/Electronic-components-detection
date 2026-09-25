# Electronics Component Detection using YOLO26

A real-time computer vision project that detects common electronic components using a **webcam, OpenCV, and YOLO26**.

## 🔍 Components Detected

* Arduino Uno
* Raspberry Pi 4
* HC-SR04 Ultrasonic Sensor
* MPU6050
* Mini Breadboard

## ⚙️ Technologies Used

* Python
* OpenCV
* YOLO26
* Label Studio
* Google Colab
* PyTorch

## 🚀 How It Works

```text
Webcam
   ↓
OpenCV
   ↓
YOLO26 Model
   ↓
Object Detection
   ↓
Bounding Boxes + Confidence
```

The model was trained on a custom dataset created by capturing and annotating images of the components using **Label Studio**. Model training was performed using **Google Colab**.

## 📊 Dataset

The initial prototype was trained using **20 images** containing the five components from different angles and arrangements.

Because of the small dataset size, this project is intended as a **proof-of-concept/demo** rather than a highly accurate production system.

## 🔮 Future Improvements

* Increase the size and diversity of the dataset
* Improve detection accuracy
* Add more electronic components
* Evaluate using precision, recall and mAP
* Deploy on edge devices such as Raspberry Pi

## 📚 Reference

This project was developed with the help of the following tutorial:

[YouTube Tutorial](https://youtu.be/r0RspiLG260)
