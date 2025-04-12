# 🐾 Animal Image Classification with Robustness Evaluation

This project explores the performance and robustness of a Convolutional Neural Network (CNN) trained to classify animal images into **Cat**, **Dog**, and **Wild** categories.

Unlike typical classification tasks, this project evaluates the model's **resilience to real-world image distortions** by testing it on various transformed versions of the validation dataset, including **blurring, brightness changes, rotation, and noise**.

---

## 📂 Dataset

The dataset is organized into:
- `train/` — Clean training images for model learning
- `val/` — Clean validation images
- `transformed_val/` — Validation images with various transformations applied

👉 **[https://www.kaggle.com/datasets/andrewmvd/animal-faces/data]**

---

## 💡 Key Objectives

- Train a CNN to classify animal images accurately.
- Apply multiple realistic distortions to validation images.
- Measure how each transformation affects classification performance.
- Visualize and analyze robustness through plots and predictions.

---

## 🔧 Tech Stack

- **Python**
- **TensorFlow / Keras**
- **OpenCV**
- **Pillow**
- **Matplotlib / Seaborn**
- **Jupyter Notebook**

---

## 🧪 Transformations Evaluated

| Category     | Subtypes                                  |
|--------------|-----------------------------------------  |
| Blurred       | Gaussian blur: 9x9 to 21x21 kernels      |
| Brightened    | Brightness factors: 0.2, 0.5, 1.5, 1.8   |
| Rotated       | 90°, 180°                                |
| Noise         | Gaussian, Salt & Pepper, Speckle         |

---

## Transformed Validation Folder Structure
transformed_val/
│
├── blurred_9x9/
│   ├── cat/
│   ├── dog/
│   └── wild/
│
├── blurred_13x13/
├── blurred_17x17/
├── blurred_21x21/
│   ├── cat/
│   ├── dog/
│   └── wild/
│
├── brightened_0.2/
├── brightened_0.5/
├── brightened_1.5/
├── brightened_1.8/
│   ├── cat/
│   ├── dog/
│   └── wild/
│
├── rotated_90/
├── rotated_180/
│   ├── cat/
│   ├── dog/
│   └── wild/
│
├── noise_gaussian/
├── noise_saltpepper/
├── noise_speckle/
│   ├── cat/
│   ├── dog/
│   └── wild/

---

## 📊 Results Overview

- The model performs well on clean data and mild distortions.
- Accuracy decreases as transformation severity increases.
- Rotation and noise have the most significant negative impact.

Visualizations include:
- 📉 Line chart comparisons for blurred and brightened variants
- 📊 Bar chart comparisons for rotated and noise types
- 🎯 Accuracy comparison between original vs average transformed performance
- 🖼️ Random predictions per transformation for each category

---


