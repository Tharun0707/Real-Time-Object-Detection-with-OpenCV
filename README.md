# Real-Time-Object-Detection-with-OpenCV

This project demonstrates real-time object detection using the YOLOv4 (You Only Look Once) model with OpenCV and a webcam.
The model detects objects from the COCO dataset (80 classes) such as person, car, dog, bicycle, etc.

## PROJECT STRUCTURE 
```
YOLOv4-Object-Detection/
│── yolov4.cfg          # YOLOv4 configuration file
│── yolov4.weights      # YOLOv4 pre-trained weights
│── coco.names          # COCO dataset class labels (80 objects)
│── detect.py           # Main Python script
│── README.md           # Documentation
```

## Dependencies
Python Libraries
Install required libraries with:
```
pip install opencv-python numpy
```

## External Files
Download the following and place them in your project folder:

yolov4.weights (248 MB)
yolov4.cfg
coco.names

## How to Run
1. Clone or download this project folder.
2. Make sure the following files are in the same directory:
yolov4.cfg
yolov4.weights
coco.names
detect.py
3. Run the script:
```
python detect.py
```
4. The webcam will open, and YOLOv4 will start detecting objects in real-time.
5. Press q to exit the window.

## EXAMPLE OUTPUT
Objects detected will be shown with bounding boxes and class labels:
```
person 0.95
dog 0.88
car 0.79
```

## Notes
Default confidence threshold is 0.5 (50%).
Non-Max Suppression (NMS) is applied to avoid overlapping boxes.
Works with any webcam accessible to OpenCV.

## Future Enhancements
Add GPU (CUDA) support for faster inference.
Save detection results to a file.
Extend to process videos instead of webcam.
