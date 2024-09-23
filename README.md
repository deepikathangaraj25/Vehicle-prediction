# REVOLUTIONIZING ROAD SAFETY FOR ADVANCED VEHICULAR ACCIDENT PREDICTION
# Application
  This project developed a real-time vehicle tracking system designed to optimize traffic flow and enhance road safety, particularly at road curves. The system leverages computer vision techniques to accurately detect and track vehicles, providing valuable insights for traffic management and monitoring.
# Technologies
  Computer Vision: Multi-scale Detector (a customized YOLO architecture) for object detection and a fusion of DeepSORT and Centroid Sort algorithms for vehicle tracking.
Dataset: A custom dataset was created to train the models, with augmentation techniques to prevent overfitting and improve generalization.
LED Display: A real-time display board provides information on vehicle types, passage time, and vehicle count to oncoming traffic.
# Table of Contents 
•	Implemented a customized YOLO architecture, specifically a multi-scale detector, for precise vehicle identification.
•	Utilized a combined approach of DeepSORT and Centroid Sort algorithms to ensure reliable and consistent vehicle tracking.
•	Achieved a remarkable mean average precision (mAP) of 0.954, demonstrating outstanding accuracy in vehicle detection.
# Steps to run Code
**Clone the repository**
git clone https://github.com/MuhammadMoinFaisal/YOLOv8_Segmentation_DeepSORT_Object_Tracking.git
**Go to the cloned folder**
cd yolov8_DeepSort
**Install the Dependencies**
pip install -e '.[dev]'
**Setting the Directory**
cd ultralytics/yolo/v8/segment
**Downloading the DeepSORT Files From The Google Drive**
https://drive.google.com/drive/folders/1kna8eWGrSfzaR6DtNJ8_GchGgPMv3VC8?usp=sharing
. After downloading the DeepSORT Zip file from the drive, unzip it go into the subfolders and place the deep_sort_pytorch folder into the ultralytics/yolo/v8/segment folder
. Downloading a Sample Videos from the Google Drive
**Input Video**
gdown "https://drive.google.com/uc?id=19P9Cf9UiJ9gU9KHnAfud6hrFOgobETTX"
Run the code with mentioned command below.
**For yolov8 segmentation + Tracking**
python predict.py model=yolov8x-seg.pt source="videos.mp4"
# RESULTS
Object Segmentation and DeepSORT Tracking (ID + Trails) and Vehicles Counting


