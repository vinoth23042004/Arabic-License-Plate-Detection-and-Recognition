# 🔍 Arabic License Plate Recognition System

A computer vision-based system to detect and recognize **Arabic license plates** using a combination of YOLOv8 for object detection and Tesseract OCR for text extraction.

## 🚀 Project Overview

This project implements an automatic number plate recognition (ANPR) system tailored for Arabic plates. The system uses a webcam or input image, detects the license plate using the YOLOv8 model, and then extracts the number using Tesseract OCR.

## ✅ Features

- 🔎 Real-time detection of Arabic license plates
- 🧠 YOLOv8 for high-performance plate detection
- 📝 Tesseract OCR integration for Arabic text recognition
- 💡 OpenCV GUI to display results
- 📷 Support for both live webcam input and static images

## 🛠️ Tech Stack

- **Python 3.11**
- **OpenCV**
- **YOLOv8** (via Ultralytics)
- **Tesseract OCR**
- **Google Colab**
- **NumPy**

## 📁 Folder Structure

\`\`\`
Vinoth_LPR_Files/
│
├── arabic_plate_detector.py     # Main detection script
├── dataset/                     # Custom labeled dataset
│   └── data.yaml                # YOLO format config
├── runs/                        # YOLO training output
├── weights/                     # Trained YOLOv8 model
├── utils/                       # Helper functions (image preprocess, etc.)
├── LICENSE                      # Optional license
└── README.md                    # This file
\`\`\`

## 🧪 Setup Instructions

1. **Clone the repository**:

\`\`\`bash
git clone https://github.com/yourusername/arabic-lpr.git
cd arabic-lpr
\`\`\`

2. **Install dependencies**:

\`\`\`bash
pip install opencv-python numpy pytesseract ultralytics
\`\`\`

3. **Install Tesseract OCR**:

- For Windows: https://github.com/UB-Mannheim/tesseract/wiki
- For Linux:

\`\`\`bash
sudo apt install tesseract-ocr
\`\`\`

4. **(Optional) Train the YOLOv8 model**:

\`\`\`bash
yolo task=detect mode=train model=yolov8s.pt data=dataset/data.yaml epochs=50 imgsz=640 batch=16 device=0
\`\`\`

## 🖥️ Run the Project

\`\`\`bash
python arabic_plate_detector.py
\`\`\`

- Press **'q'** to quit the webcam stream.

## 🧪 Sample Output

| Input Frame | Detection Output |
|-------------|------------------|
| ![Sample](path/to/input.png) | ![Result](path/to/output.png) |

> 📌 **Output**: The recognized plate number will be printed and displayed on the frame.

## 👨‍💻 Author

**Vinoth Kumar**  
[LinkedIn](https://www.linkedin.com/in/yourprofile) | [GitHub](https://github.com/yourusername)

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
EOF
