# 👕 People Clothing Segmentation using U-Net

A deep learning project for **human clothing semantic segmentation** using a custom **U-Net Encoder-Decoder architecture** implemented with **TensorFlow/Keras**.

The model performs **pixel-level classification** to segment different clothing items and human body parts from images.

<img width="676" height="248" alt="clothes" src="https://github.com/user-attachments/assets/3fd6045e-0ced-4045-9bb8-22773508273c" />


This project can be used in applications such as:

- Virtual Try-On Systems
- Fashion Analysis
- Human Parsing
- Intelligent Retail Systems
- Image Editing Applications

---

# 📌 Project Overview

Human clothing segmentation is a computer vision task that aims to classify every pixel of an image into a specific semantic category.

In this project, a **U-Net based segmentation model** is trained to predict **59 semantic classes** from human images.

## Model Workflow

```
Input Image
     |
     ↓
U-Net Segmentation Network
     |
     ↓
Pixel-wise Classification
     |
     ↓
Segmentation Mask
```

---

# 🏗️ Model Architecture

The model is based on the popular **U-Net architecture**, designed for semantic segmentation tasks.

## Encoder

The encoder extracts high-level visual features using:

- Convolution Layers
- ReLU Activation
- Max Pooling
- Increasing Feature Channels

Architecture:

```
Input
 |
Conv Block (32)
 |
Conv Block (64)
 |
Conv Block (128)
 |
Conv Block (256)
 |
Bottleneck (512)
```

---

## Decoder

The decoder reconstructs the segmentation map using:

- Transposed Convolution
- Skip Connections
- Feature Concatenation

Architecture:

```
Bottleneck
 |
Upsampling
 |
Skip Connection
 |
Decoder Blocks
 |
Output Segmentation Mask
```

---

## Output Layer

The final segmentation layer:

```python
Conv2D(
    filters=59,
    kernel_size=(1,1),
    activation="softmax"
)
```

generates a probability map for **59 clothing and body-part classes**.

---

# 📂 Project Structure

```
people-clothing-segmentation/
│
├── Data/
│   ├── images/
│   └── masks/
│
├── Notebooks/
│   └── People_clothing_Segmentation.ipynb
│
├── Requirements.txt
└── README.md
```

---

# 🛠️ Technologies

The project is developed using:

- Python
- TensorFlow
- Keras
- OpenCV
- NumPy
- Matplotlib
- Scikit-learn

---

# 📦 Installation

Clone the repository:

[![GitHub Repository](https://img.shields.io/badge/GitHub-Repository-black?logo=github)](https://github.com/Ramin0036/People-Clothing-Segmentation)

```bash
git clone https://github.com/Ramin0036/People-Clothing-Segmentation.git

cd People-Clothing-Segmentation

Install required packages:

```bash
pip install -r Requirements.txt
```

---

# 📊 Evaluation Metrics

The model performance can be evaluated using:

| Metric | Description |
|---|---|
| mIoU | Mean Intersection over Union |
| Pixel Accuracy | Correct pixel classification rate |
| Dice Score | Segmentation similarity metric |
| Cross Entropy Loss | Training optimization loss |

---

# 🎯 Applications

Possible applications include:

## 👗 Virtual Try-On

Automatic clothing segmentation for online fashion fitting systems.

## 🛍️ Fashion Recommendation

Understanding clothing items for personalized recommendations.

## 🧍 Human Parsing

Pixel-level understanding of human body parts and clothing.

## ✂️ Image Editing

Removing, replacing, or modifying clothing regions.

---

# 🤝 Contribution

Contributions are welcome!

If you would like to improve this project:

1. Fork the repository
2. Create a new branch
3. Make your changes
4. Submit a Pull Request

---

# ⭐ Support

If you find this project useful, consider giving it a ⭐ star on GitHub.

---

# 👨‍💻Author: Ramin Allahverdizadeh

Developed as a deep learning computer vision project using:

**TensorFlow + Keras + U-Net**

---

# 🔑 Keywords

```
deep-learning
computer-vision
semantic-segmentation
unet
tensorflow
keras
image-segmentation
fashion-ai
human-parsing
clothing-segmentation
```
