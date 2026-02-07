# 🌸 Flower Classification with CNN & Streamlit

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.0%2B-orange)
![Streamlit](https://img.shields.io/badge/Streamlit-1.0%2B-red)

This project is an end-to-end Deep Learning application capable of classifying images into **5 different flower categories**. It features a Convolutional Neural Network (CNN) built with **TensorFlow/Keras** and includes a user-friendly web interface powered by **Streamlit** for real-time predictions.

## 🚀 Project Overview
* **Goal:** To accurately identify flower species from uploaded images.
* **Model:** A custom CNN architecture trained from scratch.
* **Interface:** A web app where users can upload an image and get an instant classification result with a confidence score.
* **Data Handling:** Implements **Data Augmentation** (Flip, Rotation, Zoom) to prevent overfitting and improve model generalization.

---

## 📂 Dataset Details
The model was trained on a dataset containing **4,316 images** belonging to 5 classes:

| Flower Class | Image Count |
|:-------------|:-----------:|
| 🌼 Daisy     | 764         |
| 🍃 Dandelion | 1052        |
| 🌹 Rose      | 784         |
| 🌻 Sunflower | 732         |
| 🌷 Tulip     | 984         |

* **Image Size:** Resized to `180x180` pixels.
* **Split:** 80% Training, 20% Validation.

---

## 🛠 Technologies Used
* **[Python](https://www.python.org/)**
* **[TensorFlow & Keras](https://www.tensorflow.org/)** - For model creation and training.
* **[Streamlit](https://streamlit.io/)** - For the web application interface.
* **[NumPy](https://numpy.org/)** - For matrix operations.
* **[Matplotlib](https://matplotlib.org/)** - For data visualization.

---

## 🧠 Model Architecture
The model follows a `Sequential` architecture designed for image classification:

1.  **Rescaling Layer:** Normalizes pixel values to the `[0, 1]` range.
2.  **Data Augmentation:** RandomFlip, RandomRotation (0.1), RandomZoom (0.1).
3.  **Convolutional Blocks:** Three blocks of `Conv2D` (16, 32, 64 filters) followed by `MaxPooling2D`.
4.  **Dropout:** A dropout layer (0.2) to reduce overfitting.
5.  **Dense Layers:** Flatten, Dense (128 units, ReLU), Output (5 units).

---

## 💻 Installation & Usage

### 1. Clone the Repository
```bash
git clone [https://github.com/ilaydagunduz/flower-classification.git](https://github.com/ilaydagunduz/flower-classification.git)
cd flower-classification
