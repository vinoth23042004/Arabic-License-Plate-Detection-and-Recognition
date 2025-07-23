# 🔍 Arabic License Plate Recognition System

A computer vision-based Python project designed to detect and recognize **Arabic license plates** using YOLOv8 for object detection and Tesseract OCR for text extraction. Ideal for smart surveillance systems, parking automation, and law enforcement applications.

---

## 🚀 Features

- 🔎 **Real-Time Detection** – Detect Arabic license plates in real-time from webcam or images.  
- 🧠 **YOLOv8 Model** – High-performance plate detection using Ultralytics YOLOv8.  
- 📝 **Tesseract OCR** – Extract Arabic text accurately from detected plates.  
- 💡 **OpenCV GUI** – Visual interface to show detection results live.  
- 🖼️ **Static Image Support** – Works on pre-stored image inputs as well.

---

## 🗃️ Folder Structure

```
Vinoth_LPR_Files/
├── arabic_plate_detector.py          # Main detection and recognition script
├── dataset/
│   └── data.yaml                     # YOLO training configuration file
├── runs/                             # YOLO training output folder
├── weights/                          # YOLOv8 trained weights
├── utils/                            # Image preprocessing and helper functions
├── LICENSE                           # License info (MIT)
└── README.md                         # Project documentation
```

---

## 🛠️ Tech Stack

| Technology      | Purpose                               |
|------------------|----------------------------------------|
| **Python 3.11**   | Core programming language              |
| **OpenCV**        | Image processing and display           |
| **YOLOv8**        | Object detection (Ultralytics)         |
| **Tesseract OCR** | OCR engine for text extraction         |
| **NumPy**         | Numerical operations                   |
| **Google Colab**  | (Optional) model training environment  |

---

## 📦 Requirements

Create a `requirements.txt` file with the following content:

```
opencv-python
numpy
pytesseract
ultralytics
```

Install all dependencies using:

```bash
pip install -r requirements.txt
```

---

## 🧪 Setup Instructions

1. **Clone the repository**:

```bash
git clone https://github.com/yourusername/arabic-lpr.git
cd arabic-lpr
```

2. **Install dependencies**:

```bash
pip install opencv-python numpy pytesseract ultralytics
```

3. **Install Tesseract OCR**:

- For Windows: https://github.com/UB-Mannheim/tesseract/wiki  
- For Linux:

```bash
sudo apt install tesseract-ocr
```

4. **(Optional) Train the YOLOv8 model**:

```bash
yolo task=detect mode=train model=yolov8s.pt data=dataset/data.yaml epochs=50 imgsz=640 batch=16 device=0
```

---

## 🖥️ Run the Project

```bash
python arabic_plate_detector.py
```

- Press **'q'** to quit the webcam stream.

---

## 📚 Use Cases

- Smart Traffic Surveillance  
- Arabic Plate Parking Management  
- Automated Toll Collection  
- Law Enforcement & Vehicle Tracking

---

## 🧪 Sample Output

| Input Frame | Detection Output |
|-------------|------------------|
| ![Sample](https://raw.githubusercontent.com/vinoth23042004/Arabic-License-Plate-Detection-and-Recognition/refs/heads/main/assests/test_image.jpg) | ![Result](https://raw.githubusercontent.com/vinoth23042004/Arabic-License-Plate-Detection-and-Recognition/refs/heads/main/assests/output_image.PNG) |

> 📌 **Output**: The recognized plate number will be printed and displayed on the frame.

---

## 📌 Future Enhancements

- Voice command integration  
- Cloud-based plate logging  
- Multi-language OCR support  
- Web/mobile deployment




