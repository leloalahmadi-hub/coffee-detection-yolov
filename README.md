<h1 align="center">☕ Coffee Cup Detection with YOLOv5</h1> <p align="center"> <img src="https://img.shields.io/badge/YOLOv5-Object%20Detection-00FFFF?style=for-the-badge" /> <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" /> <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" /> <img src="https://img.shields.io/badge/STATUS-In%20Progress-orange?style=for-the-badge" /> </p>
<h2>📋 About</h2> <ul> <li>☕ Object detection model that identifies coffee cups &amp; drinks in images</li> <li>🧠 Built with <b>YOLOv5</b> (Ultralytics/PyTorch)</li> <li>🎯 Goal: detect and classify different coffee cup / drink types</li> </ul>
<h2>📁 Project Structure</h2>
coffee-detection-yolov/
├── data/
│   ├── images/          # raw training/validation images
│   ├── labels/          # YOLO-format annotation files
│   └── data.yaml         # dataset config (classes, paths)
├── models/               # trained weights (best.pt, last.pt)
├── notebooks/            # exploration / experiments
├── train.py               # training script
├── detect.py              # inference script
├── requirements.txt
└── README.md
<h2>⚙️ Setup</h2>
bash
git clone https://github.com/leloalahmadi-hub/coffee-detection-yolov.git
cd coffee-detection-yolov
pip install -r requirements.txt
<h2>🏋️ Training</h2>
bash
python train.py --data data/data.yaml --weights yolov5s.pt --epochs 100 --img 640
<h2>🔍 Inference</h2>
bash
python detect.py --weights models/best.pt --source data/images/test
<h2>🗺️ Roadmap</h2> <ul> <li>☐ Collect &amp; label coffee cup dataset</li> <li>☐ Train baseline YOLOv5 model</li> <li>☐ Evaluate accuracy (mAP)</li> <li>☐ Improve dataset &amp; retrain</li> <li>☐ Deploy / demo</li> </ul>
