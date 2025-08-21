# Traffic Detection Using Machine Learning

A comparative study of YOLOv8n vs YOLOv8s for traffic object detection.

## Overview

This project compares two YOLO models for detecting traffic objects in images. The study analyzes the trade-offs between accuracy and speed for real-world traffic monitoring applications.

## Models Compared

- **YOLOv8n**: Lightweight model optimized for speed
- **YOLOv8s**: Larger model optimized for accuracy

## Dataset

- 6,633 traffic images
- 5 object classes: bicycle, bus, car, motorbike, person
- 79,628 total annotations

## Key Results

| Model | mAP50 | Inference Time | Model Size |
|-------|-------|---------------|------------|
| YOLOv8n | 92.3% | 2.1ms | 6.0MB |
| YOLOv8s | 94.4% | 23.6ms | 21.5MB |

## Main Findings

- YOLOv8s achieves 2.3% better accuracy than YOLOv8n
- YOLOv8n is 11x faster than YOLOv8s
- Both models perform well for traffic detection
- Choice depends on application requirements (speed vs accuracy)

## Project Structure

```
├── notebooks/           # Jupyter notebooks with code
├── yolov8n_results/     # YOLOv8n training results
├── yolov8s_results/     # YOLOv8s training results
├── model_comparison/    # Comparative analysis
├── thesis_results/      # Academic documentation
└── predictions/         # Sample prediction outputs
```

## Requirements

- Python 3.8+
- PyTorch
- Ultralytics YOLOv8
- OpenCV
- Matplotlib

## Usage

1. Install dependencies from `requirements.txt`
2. Run the Jupyter notebook in `notebooks/` folder
3. View results in respective result folders

## Conclusion

This study demonstrates clear trade-offs between model efficiency and accuracy for traffic detection tasks. YOLOv8n is recommended for real-time applications, while YOLOv8s is better for high-accuracy requirements.
