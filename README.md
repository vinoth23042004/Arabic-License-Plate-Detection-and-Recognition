🔍 Arabic License Plate Recognition System
A computer vision-based Python project designed to detect and recognize Arabic license plates using YOLOv8 for object detection and Tesseract OCR for text extraction. Ideal for smart surveillance systems, parking automation, and law enforcement applications.

🎥 Demo Video
https://user-images.githubusercontent.com/demo-video-link/sample.mp4

📌 (Replace with your actual uploaded video GitHub link)

🚀 Features
🔎 Real-Time Detection – Detect Arabic license plates in real-time from webcam or images.

🧠 YOLOv8 Model – High-performance plate detection using Ultralytics YOLOv8.

📝 Tesseract OCR – Extract Arabic text accurately from detected plates.

💡 OpenCV GUI – Visual interface to show detection results live.

🖼️ Static Image Support – Works on pre-stored image inputs as well.

🗃️ Folder Structure
graphql
Copy
Edit
Vinoth_LPR_Files/
├── arabic_plate_detector.py          # Main detection and recognition script
├── dataset/
│   └── data.yaml                     # YOLO training configuration file
├── runs/                             # YOLO training output folder
├── weights/                          # YOLOv8 trained weights
├── utils/                            # Image preprocessing and helper functions
├── LICENSE                           # License info (MIT)
└── README.md                         # Project documentation
🛠️ Tech Stack
Technology	Purpose
Python 3.11	Core programming language
OpenCV	Image processing and display
YOLOv8	Object detection (Ultralytics)
Tesseract	OCR engine for text extraction
NumPy	Numerical computation
Google Colab	Model training and testing platform

📦 Requirements
Create a requirements.txt file with the following content:

Copy
Edit
opencv-python
numpy
pytesseract
ultralytics
Install all dependencies using:

bash
Copy
Edit
pip install -r requirements.txt
🖥️ How to Run
Clone the Repository

bash
Copy
Edit
git clone https://github.com/yourusername/arabic-lpr.git
cd arabic-lpr
Install Dependencies

bash
Copy
Edit
pip install -r requirements.txt
Install Tesseract OCR

Windows: Download from UB Mannheim

Linux:

bash
Copy
Edit
sudo apt install tesseract-ocr
Run the Application

bash
Copy
Edit
python arabic_plate_detector.py
Quit Webcam Feed
Press q to exit the OpenCV stream.

📚 Use Cases
Smart Traffic Surveillance

Arabic Plate Parking Management

Automated Toll Collection

Law Enforcement & Vehicle Tracking

📌 Future Enhancements
Add voice feedback for recognized numbers

Integrate with cloud for plate logging

Add multi-language OCR support

Deploy as a web or mobile application

👨‍💻 Author
Vinoth Kumar
LinkedIn • GitHub

📜 License
This project is licensed under the MIT License – see the LICENSE file for details.

Let me know if you'd like a version with markdown preview links or image placeholder fixes!








