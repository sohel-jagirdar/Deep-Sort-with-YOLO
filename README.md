# Deep-Sort-with-YOLO
This application designed for tracking object with help of YLO and Deep Sort

This repository implements YOLOv3 and Deep SORT in order to perfrom real-time object tracking. Yolov3 is an algorithm that uses deep convolutional neural networks to perform object detection. We can feed these object detections into Deep SORT (Simple Online and Realtime Tracking with a Deep Association Metric) in order for a real-time object tracker to be created.

# Conda Setup
### Tensorflow CPU
conda env create -f conda-cpu.yml
conda activate tracker-cpu

### Tensorflow GPU
conda env create -f conda-gpu.yml
conda activate tracker-gpu

# pip setup
### TensorFlow CPU
pip install -r requirements.txt

### TensorFlow GPU
pip install -r requirements-gpu.txt

# Downloading YOLO Weights

### yolov3
wget https://pjreddie.com/media/files/yolov3.weights -O weights/yolov3.weights

### yolov3-tiny
wget https://pjreddie.com/media/files/yolov3-tiny.weights -O weights/yolov3-tiny.weights

# Detection Running
python detectorTracker.py

# Output / Result![output](https://user-images.githubusercontent.com/52422511/196026195-5c58b6bd-bf8e-4b04-8ccf-06e4aa04dffa.gif)

