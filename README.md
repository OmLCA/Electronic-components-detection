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
* Anaconda

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

## 💻 Steps to Deploy on PC/Laptop (Windows)

1. Install **Python** on your Windows PC/Laptop.

2. Open **Anaconda Prompt** and navigate to the project folder.

3. Create a new Conda environment:

```bash
conda create -n yolo-env python=3.10

```
4. Activate the environment:

```bash
conda activate yolo-env

```
5. Install the required Python libraries:

pip install ultralytics opencv-python numpy

6. Make sure my_model.pt and yolo_detect.py are present in the same folder.

7. Connect a webcam to the PC/Laptop.

8. Run the detection program:

python yolo_detect.py --model my_model.pt --source usb0

The webcam window will open and the model will detect the trained electronic components.
Press Q to stop the detection.

Note: usb0 refers to camera index 0. If your webcam uses a different index, try usb1 or usb2

## 📚 Reference

This project was developed with the help of the following tutorial:

[YouTube Tutorial](https://youtu.be/r0RspiLG260)
