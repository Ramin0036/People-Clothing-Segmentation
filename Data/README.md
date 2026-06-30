# 👕 People Clothing Segmentation

This project focuses on **semantic segmentation of clothing items** using deep learning. The model predicts a pixel-wise segmentation mask for each input image, assigning every pixel to its corresponding clothing or body-part class.

---

## 📥 Dataset

The dataset is **not included** in this repository due to GitHub file size limitations.

Please download the dataset from Kaggle using the following link:

**Dataset Link:**  
https://www.kaggle.com/datasets/rajkumarl/people-clothing-segmentation

After downloading:

1. Extract the dataset.
2. Place the extracted folder inside the project directory (or update the dataset path in the notebook accordingly).

---

## 📂 Dataset Structure

The dataset contains the following files and folders:

```text
dataset/
│
├── images/
│   ├── 000001.png
│   ├── 000002.png
│   ├── ...
│
├── masks/
│   ├── 000001.png
│   ├── 000002.png
│   ├── ...
│
└── labels.csv
```

### Folder Description

| Folder | Description |
|---------|-------------|
| **images/** | RGB images of people wearing different types of clothing. |
| **masks/** | Pixel-level segmentation masks corresponding to each image. |
| **labels.csv** | List of segmentation classes and their label IDs. |

---

## 📊 Dataset Information

| Property | Value |
|----------|-------|
| Number of Images | 1,000 |
| Number of Masks | 1,000 |
| Image Format | PNG |
| Mask Format | PNG |
| Image Resolution | 825 × 550 |
| Number of Classes | 59 |

The segmentation classes include clothing items and body parts such as:

- Background
- Hair
- Face
- Skin
- Hat
- Sunglasses
- Shirt
- T-shirt
- Jacket
- Coat
- Dress
- Pants
- Shorts
- Skirt
- Socks
- Shoes
- Scarf
- Bag
- Belt

The complete class list can be found in **labels.csv**.

---

## 🎯 Project Objective

The goal of this project is to train a **semantic segmentation** model capable of identifying clothing items at the pixel level.

Given an RGB image, the model predicts a segmentation mask in which every pixel belongs to one of the predefined clothing categories.

---

## 🚀 Getting Started

Clone the repository:


Repository: [People-Clothing-Segmentation](https://github.com/Ramin0036/People-Clothing-Segmentation)


Download the dataset from Kaggle:

https://www.kaggle.com/datasets/rajkumarl/people-clothing-segmentation

Extract the dataset and organize it as follows:

```text
project/
│
├── dataset/
│   ├── images/
│   ├── masks/
│   └── labels.csv
│
├── notebooks/
├── models/
├── README.md
└── ...
```

Run the training or inference notebook after updating the dataset path if necessary.

---

## 📚 Dataset Source

**People Clothing Segmentation Dataset**

- **Author:** Rajkumar Lakshmanamoorthy
- **Platform:** Kaggle

Dataset URL:

https://www.kaggle.com/datasets/rajkumarl/people-clothing-segmentation

---
