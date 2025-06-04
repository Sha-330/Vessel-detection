# 🚢 Ship Detector using YOLOv5 + Flask

A web-based application that uses YOLOv5 to detect ships in SAR (Synthetic Aperture Radar) satellite images. The application is built with Flask and provides a simple interface to upload an image and get ship detection results.

## 📁 Project Structure

```
ship detector/
├── app.py                               # Flask web application
├── templates/
│   └── index.html                       # Frontend UI for uploading images
├── uploads/                             # Directory where user images are uploaded
├── sar_output/
│   └── ship_detector_run/
│       └── weights/
│           └── best.pt                  # Trained YOLOv5 model weights
│   └── ship_predictions/                # Folder where predictions are saved
```

## ⚙️ Features

- Upload a satellite SAR image and detect ships using YOLOv5.
- Auto-download YOLOv5 repository if not present.
- Uses Flask as the backend framework.
- Prediction results saved and displayed via web interface.

## 🚀 How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/Sha-330/Vessel-detection.git
cd ship-detector
```

### 2. Set Up Environment

Make sure you have Python ≥3.8 and pip installed.

```bash
pip install -r yolov5/requirements.txt
pip install flask
```

### 3. Run the App

```bash
python app.py
```

Navigate to `http://127.0.0.1:5000` in your browser.

## 🧠 Model Info

- Model: YOLOv5
- Weights: Trained and stored in `sar_output/ship_detector_run/weights/best.pt`
- Predictions output to `sar_output/ship_predictions/`

## 🖼️ Sample Images

Sample input and prediction images are available in the `uploads/` and `ship_predictions/` directories respectively.

## 🛠️ Notes

- If `yolov5/` directory doesn't exist, it is automatically cloned from Ultralytics' GitHub repo.
- Make sure `git` and `pip` are installed on your system.
- The app assumes a Unix-like path structure for saving outputs.


