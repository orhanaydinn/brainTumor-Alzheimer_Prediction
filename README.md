# 🧠 Brain Tumor & Alzheimer Disease Detection with Deep Learning

This project aims to build an image classification system that can detect **brain tumors** and **Alzheimer’s disease stages** from MRI images using machine learning and deep learning techniques. The goal is to support early diagnosis by providing accurate predictions based on medical imaging.

---

## 📁 Dataset

The dataset consists of MRI brain scan images divided into the following classes:

### 🧠 Alzheimer Classes:
- `alzheimer_mild_demented`
- `alzheimer_moderate_demented`
- `alzheimer_non_demented`
- `alzheimer_very_mild_demented`

### 🎯 Tumor Classes:
- `tumor_yes`
- `tumor_no`

> Augmentation has been applied only to **tumor_no** classes to balance the dataset and avoid overfitting.

---

## 🔍 Project Flow

### ✅ Step 1: Data Loading & Structure Visualization
- ZIP file manually uploaded and extracted in Colab.
- Folder structure printed and random sample images visualized.

### ✅ Step 2: Data Preprocessing
- Images resized to `64x64` or `96x96` depending on the model.
- Normalization performed using `pixel / 255.0`.
- Labels encoded using a mapping dictionary.
- Train-test split applied (80/20, stratified).

### ✅ Step 3: Data Augmentation
- Custom augmentation techniques applied separately using:
  - `ImageDataGenerator` for `tumor_no`

### ✅ Step 4: Model Development

**Implemented Models:**
- ✅ Baseline CNN
- ✅ VGG16 (Transfer Learning)
- ✅ EfficientNetB0 (Transfer Learning)
- ✅ ResNet50 (Transfer Learning)
- ✅ DenseNet121 (Transfer Learning)
---

## 📊 Evaluation & Visualization

- Accuracy and loss curves plotted.
- Class distribution visualized using bar plots.
- Confusion matrices and classification reports will be added.

---

## ⏱️ Training Time & Efficiency

Each model’s training duration is logged and compared for performance benchmarking.

---

## 📌 Technologies Used

- Python
- TensorFlow / Keras
- OpenCV
- Albumentations
- Scikit-learn
- Google Colab

---

## 📎 How to Run

1. Upload your dataset ZIP manually to Google Colab.
2. Run the notebook cells step by step.
3. If resuming, upload `.h5` or `.keras` models manually to avoid re-training.
4. Run evaluation cells directly to visualize results.

---

## 👤 Author

**Orhan Aydın**  
MSc Data Science & Artificial Intelligence  


![Image](https://github.com/user-attachments/assets/eebabb60-9e96-48a5-a1c7-d2c467c967ff)
