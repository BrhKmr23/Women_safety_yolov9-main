# Women Safety - YOLOv9

## Overview

This repository contains a **Women Safety Detection System** built using **YOLOv9** (You Only Look Once version 9). The model aims to improve safety by detecting potential threats in real-time, allowing for timely alerts. It leverages advanced deep learning techniques to analyze images and videos, ensuring effective monitoring of safety concerns.

## Features

- **Real-time Object Detection**: Detects potential threats such as individuals or objects that may pose a risk to women.
- **High Accuracy**: The model is fine-tuned for identifying safety-related objects and persons in diverse environments.
- **YOLOv9 Architecture**: Utilizes the latest YOLOv9 model for fast, accurate, and reliable detection.
- **Customizable**: Easily train the model on your own dataset to adapt to specific safety concerns or environments.

## Installation

### Prerequisites

Ensure that the following dependencies are installed:

- **Python** 3.8 or higher
- **PyTorch** 1.10 or higher
- **CUDA** (for GPU acceleration)
- Other dependencies listed in `requirements.txt`

### Installation Steps

1. Clone the repository:
   ```bash
   git clone [[https://gitlab.com/yourusername/women-safety-yolov9.git]()](https://github.com/BrhKmr23/Women_safety_yolov9-main.git)
   cd women-safety-yolov9
   ```
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Verify the installation by running a test script:
   ```bash
   python test.py
   ```

## Usage

### Training the Model

1. Prepare your dataset in the appropriate format (images and annotations).
2. Configure the dataset path in the training script:
   ```bash
   python train.py --data dataset.yaml --epochs 50 --batch-size 16
   ```

### Running Inference

Use the pre-trained model for inference:

```bash
python detect.py --source data/images --weights yolov9.pt --conf 0.5
```

### Customization

To adapt the model for a specific use case:

- Modify the dataset configuration file (`dataset.yaml`).
- Train the model on your custom dataset.

## Results








### Precision-Recall Curve

The PR curve demonstrates the model's performance across various thresholds:

### Precision-Recall Curve
<div style="text-align: center; display: inline-block; margin-right: 20px;">
  ![Training Loss](https://i.ibb.co/7SNM7DM/image.png)
</div>
### F1 Score

<div style="text-align: center; display: inline-block; margin-right: 20px;">
  ![Training Accuracy](https://i.ibb.co/Mk5tf1b/image.png)
</div>



The model achieved an F1 score of **0.92**, indicating a strong balance between precision and recall.

### Result Graph

The graph below shows the true vs. predicted values during evaluation:
<div style="text-align: center; display: inline-block;">
  ![PR Curve](https://i.ibb.co/vzjTVZc/image.png)
</div>


## Key Metrics

- **Accuracy**: 87
%
- **F1 Score**: 0.92
- **Precision**: 0.93
- **Recall**: 0.91

## Contributors


Dharunraagav

[GitLab Profile](https://gitlab.com/dharunraagav)

Bharath Kumar



## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## Acknowledgments

Special thanks to the contributors of YOLOv9 and PyTorch for providing excellent tools and frameworks to build this project.

