# Stroma CV Challange (Multi-class Object Detection and Counting)

### Processing Unit
- GPU NVIDIA A100-SXM4-40GB, 40536MiB

### Changed Hyperparameters
- Batch sized increased to 16, lr selected as 0.01
- Confidence threshold increased to 0.65 to eliminate false detections
- trained yolov5 and yolov8 models and achieved best overall accuracy was visually %100 on test video with yolov5
- albumentations (horizontal flip, jitter, scale)

### Added Features
- Track labels contains class names and track trace line removed

### Pre-Requsities
- Python 3.9 (Python 3.7/3.8 can work in some cases)
- pip install -r requirements.txt

### data download 
- images, labels, custom yml file and trained model "best.pt" (yolov5)
- https://drive.google.com/drive/folders/1_h87v1ts_kUqZ5n5fOfQhJkevCvS-LdA?usp=sharing

### for object detection + object tracking + labels(edited v2 version)
- python obj_det_and_trk_2.py --weights yolov5s.pt --source "your video.mp4"
- 
### What is next (working on)
- **✨ Extra:** Inference optimizations (e.g. pruning, quantization) with libraries like TensorRT, ONNX runtime and a comparison of each
- **✨ Extra:** Optimizing  inference pipeline to work on an embedded system like a Jetson in real time. (>30fps)

### References
 - https://github.com/ultralytics/yolov5
 - https://github.com/RizwanMunawar/yolov5-object-tracking/commits?author=RizwanMunawar
 - https://github.com/abewley/sort
 <img align="right" width="200" height="200" src="https://github.com/cengizhunter/stroma_challange/blob/main/yolo.png">

 ![My Image](detection.gif)

