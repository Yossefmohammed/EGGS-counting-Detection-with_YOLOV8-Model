# Egg Counting Detection with YOLOv8

This project implements an automated egg counting system using YOLOv8 for object detection and segmentation. The system can detect and count eggs in video streams with high accuracy.

[![GitHub](https://img.shields.io/badge/GitHub-Repository-blue)](https://github.com/Yossefmohammed/EGGS-counting-Detection-with_YOLOV8-Model)

## Features

- Real-time egg detection and counting
- Object tracking to prevent double counting
- Segmentation of eggs for precise detection
- Visual feedback with bounding boxes and tracking IDs
- Performance metrics display (FPS and detection speed)

## Requirements

- Python 3.x
- OpenCV
- Ultralytics YOLOv8
- NumPy
- CVZone

## Installation

1. Clone the repository:
```bash
git clone https://github.com/Yossefmohammed/EGGS-counting-Detection-with_YOLOV8-Model.git
cd EGGS-counting-Detection-with_YOLOV8-Model
```

2. Install the required packages:
```bash
pip install ultralytics opencv-python numpy cvzone
```

## Usage

1. Place your video file in the project directory (default: `egg.mp4`)
2. Run the Jupyter notebook:
```bash
jupyter notebook counting_model.ipynb
```

3. Execute the cells in sequence to start the detection and counting process

## Project Structure

- `counting_model.ipynb`: Main Jupyter notebook containing the implementation
- `Yolo_model.py`: YOLOv8 model wrapper class
- `tracker.py`: Object tracking implementation
- `best.pt`: Pre-trained YOLOv8 model weights
- `coco1.txt`: Class labels file

## How It Works

1. The system uses YOLOv8 for object detection and segmentation
2. A custom tracker maintains object IDs to prevent double counting
3. The detection area is defined by a polygon
4. Objects crossing the defined area are counted
5. Real-time visualization shows:
   - Bounding boxes around detected eggs
   - Tracking IDs
   - Total count
   - Performance metrics

## Performance

The system achieves real-time performance with:
- Average inference time: ~130-140ms per frame
- Preprocessing time: ~3ms
- Postprocessing time: ~13-14ms

## Contact

For any questions or support, please contact:

- Email: ypssefmohammedahmed@gmail.com
- Phone: 01126078938

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Repository

Visit the [GitHub repository](https://github.com/Yossefmohammed/EGGS-counting-Detection-with_YOLOV8-Model) for the latest updates and to contribute to the project.
