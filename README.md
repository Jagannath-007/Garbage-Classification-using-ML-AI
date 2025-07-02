# 🗑️ Garbage Classification using Transfer Learning

This project aims to classify images of garbage into appropriate categories using **Transfer Learning** techniques with deep learning models such as **EfficientNetV2B2**. This helps support environmental sustainability efforts like automated waste segregation and smart recycling.

---

## 📁 Dataset

- The dataset is divided into **train**, **validation**, and **test** directories.
- Each directory contains images categorized into multiple garbage classes (e.g., cardboard, glass, metal, paper, plastic, trash).

---

## 📦 Libraries Used

- `TensorFlow`, `Keras`
- `NumPy`, `Matplotlib`, `Seaborn`
- `EfficientNet` from `keras.applications`

---

## 🔧 Setup & Data Preprocessing

- **ImageDataGenerator** was used for real-time data augmentation:
  - Rescaling
  - Rotation
  - Horizontal/Vertical Flips
  - Zoom and Shear transformations

```python
train_generator = train_datagen.flow_from_directory(...)
