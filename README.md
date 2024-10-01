# Brain Metastasis Segmentation

## Overview

This repository contains implementations of two advanced neural network architectures—Nested U-Net (U-Net++) and Attention U-Net—specifically designed for the task of brain metastasis segmentation in medical imaging. The goal is to accurately segment metastatic brain tumors from MRI scans, which is critical for diagnosis and treatment planning.

## Architectures

### Nested U-Net (U-Net++)

Nested U-Net, also known as U-Net++, is an improvement over the traditional U-Net architecture. It introduces dense skip pathways, which allow for better feature propagation and reuse. The architecture consists of a series of nested skip pathways that enhance the learning capability of the model, leading to improved segmentation accuracy.

#### Key Features:
- **Dense Skip Connections**: Helps in retaining high-resolution features, improving context understanding.
- **Deep Supervision**: Allows intermediate outputs to contribute to the final loss calculation, aiding in gradient flow and learning.

### Attention U-Net

Attention U-Net extends the U-Net architecture by incorporating attention gates, which allow the model to focus on relevant features and suppress irrelevant ones. This is particularly useful in medical imaging, where precise segmentation of tumor boundaries is essential.

#### Key Features:
- **Attention Gates**: Dynamically emphasize important features while ignoring irrelevant ones, improving segmentation quality.
- **Efficient Use of Computational Resources**: Focuses on significant areas in the image, making the model more interpretable and robust.

## Application to Metastasis Segmentation

Both architectures are tailored for the challenge of segmenting brain metastases from MRI scans. Their capabilities to extract intricate patterns and highlight significant features are crucial in distinguishing cancerous tissues from healthy ones. The combined strengths of these architectures contribute to enhanced segmentation performance, which is vital for accurate diagnosis and treatment planning.

## Setup Instructions

To run the code in this repository, follow these steps:

### Prerequisites
- Python 3.6 or higher
- TensorFlow 2.x
- Keras
- Other dependencies are listed in `requirements.txt`

### Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/yourusername/brain-metastasis-segmentation.git
   cd brain-metastasis-segmentation
