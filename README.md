# Street Vision Detector

A smart computer vision project utilizing YOLOv8 for object detection and recognition.

## Before & After
Here is a comparison showing the input image before detection and the final output with bounding boxes:

### Original Image (Before)
<p align="center">
  <img src="original_image.jpg" alt="Original Input" width="600"/>
</p>

### Detection Result (After)
<p align="center">
  <img src="detection_result.png" alt="Object Detection Output" width="600"/>
</p>

## Installation & Setup

To run this project, make sure to install the required Ultralytics library using pip:

```bash
pip install ultralytics
```

## Usage

Import the YOLO class and load the pre-trained YOLOv8 Nano model:

```python
from ultralytics import YOLO

# Load the pre-trained YOLOv8 Nano model
model = YOLO("yolov8n.pt")

print("Model loaded successfully!")
```

Pass an image to the model to detect objects:

```python
# Run object detection on the input image
results = model("https://ultralytics.com/images/bus.jpg")

# Display the detection results with bounding boxes
results[0].show()
```

You can replace the sample image URL with your own image path.
