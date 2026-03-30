🌊 Underwater Object Detection using YOLOv11

A deep learning-based computer vision project for detecting underwater objects using the YOLOv11 framework. This system is designed for real-time marine monitoring, underwater robotics, and environmental analysis.

📌 Project Overview
This project leverages YOLOv11 (You Only Look Once v11) for detecting objects in underwater environments where challenges like low visibility, color distortion, and noise exist.

It can detect:
🐟 Marine species (fish, sharks, etc.)
🪸 Coral structures
🧴 Marine debris (plastic, waste)
⚓ Underwater objects (wrecks, tools, etc.)

🧠 Deep Learning Approach
Model: YOLOv11
Task: Object Detection
Framework: PyTorch + Ultralytics
Training Type: Supervised Learning

Key Challenges Solved:
🌫️ Low visibility
🎨 Color distortion
🌊 Light refraction
🧊 Noise & blur

📂 Project Structure
Underwater-YOLOv11/
│
├── data/
│   ├── images/
│   │   ├── train/
│   │   └── val/
│   ├── labels/
│
├── models/
│   └── yolov11.pt
│
├── runs/
│
├── main.py
├── Untitled.ipynb
├── data.yaml
├── requirements.txt
└── README.md

⚙️ Installation
1️⃣ Clone Repository
git clone https://github.com/your-username/underwater-yolov11.git
cd underwater-yolov11
2️⃣ Create Virtual Environment
python -m venv venv
venv\Scripts\activate   # Windows
# source venv/bin/activate  # Linux/Mac
3️⃣ Install Dependencies
pip install -r requirements.txt
📦 Requirements
Python ≥ 3.8
PyTorch
OpenCV
Ultralytics

Install manually if needed:
pip install ultralytics torch torchvision opencv-python matplotlib

🏋️ Model Training
yolo detect train model=yolov11.pt data=data.yaml epochs=50 imgsz=640 batch=16

🔍 Inference / Detection
Run using Python
python main.py
Run using CLI
yolo detect predict model=yolov11.pt source=0
Input Options:
0 → Webcam
video.mp4 → Video
images/ → Folder

📈 Results
🎯 Accurate bounding box detection
⚡ Real-time inference
📊 Confidence scores

Output saved in:
runs/detect/
🧪 Data Preprocessing Techniques

To improve underwater detection:
Histogram Equalization
CLAHE (Contrast Enhancement)
Color Correction (RGB balancing)
Image Denoising

🚀 Applications
🌊 Marine biodiversity monitoring
🤖 Underwater robotics
🛳️ Shipwreck exploration
♻️ Ocean pollution detection
🔬 Scientific research
🔧 Customization

You can tune:
Model variants (nano, small, medium, large)
Epochs & batch size
Image resolution
Dataset classes

📜 License
This project is licensed under the MIT License.

👨‍💻 Author
Janarthan B
🎓 B.Tech IT | Data Science Enthusiast
📍 Chennai, India
