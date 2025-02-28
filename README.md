# Automating Hidden Object Games with Object Detection

**Description:** A user-friendly Jupyter app for object detection using YOLOv11 and Faster R-CNN, trained on self-driving, UNO card, and synthetic fruit datasets from Roboflow. Detects objects with bounding boxes and labels.

## Overview
This project automates hidden object detection with a modular Jupyter interface. It uses YOLOv11 and Faster R-CNN, fine-tuned on custom datasets, to identify objects in uploaded images, supporting use cases like games and self-driving.

## Features
- **Model Selection**: Choose YOLOv11 or Faster R-CNN via dropdown.
- **Image Upload**: Upload an image for inference.
- **Object Detection**: View bounding boxes and labels on detected objects.
- **Customizable**: Add new models/datasets via training notebooks.

## Models and Datasets
- **YOLOv11**:
  - **Trained On**: Self-driving (cars, pedestrians), UNO cards/numbers (Roboflow).
  - **Notebook**: `yolo_training.ipynb` (edit `data.yaml` for custom data).
- **Faster R-CNN**:
  - **Trained On**: Synthetic fruits, UNO cards/numbers (Roboflow).
  - **Notebook**: `faster_rcnn_training.ipynb`.
- **Source**: Datasets from [Roboflow](https://roboflow.com/).

## Implementation
- **Tools**: Python, PyTorch, OpenCV, Jupyter Notebook.
- **Files**:
  - **`yolo_training.ipynb`**: Trains YOLOv11 on custom datasets.
  - **`faster_rcnn_training.ipynb`**: Trains Faster R-CNN on custom datasets.
  - **`app.ipynb`**: Runs the frontend for model selection, image upload, and detection.

## How to Run
1. **Setup**:
   - Install: `pip install torch torchvision opencv-python jupyter`.
   - Download datasets from Roboflow and update paths in notebooks.
2. **Training**:
   - Run `yolo_training.ipynb` (update `data.yaml`).
   - Run `faster_rcnn_training.ipynb` (update dataset paths).
3. **Frontend**:
   - Launch `app.ipynb` in Jupyter (`jupyter notebook`), run all cells, and use the interface.

## Output
- Trained YOLOv11 and Faster R-CNN models.
- Detection results in `app.ipynb` with bounding boxes/labels.

## Results
YOLOv11 is fast for self-driving/UNO detection; Faster R-CNN excels with fruits/UNO. 
## License
MIT License - see [LICENSE](LICENSE).
