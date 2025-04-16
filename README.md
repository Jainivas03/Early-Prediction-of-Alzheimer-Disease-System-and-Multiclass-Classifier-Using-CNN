# 🧠 Early-Prediction-of-Alzheimer-Disease-System-and-Multiclass-Classifier-Using-CNN

This project is dedicated to the **early prediction and classification of Alzheimer's disease** using advanced deep learning techniques. A custom **Convolutional Neural Network (CNN)** model is trained on brain MRI images to classify them into different stages of Alzheimer's with high accuracy. The model is further integrated with a **Gradio UI** to provide an interactive interface for real-time predictions.

---

## 📌 Project Highlights

- Achieved **99.22% training accuracy** and **99.65% testing accuracy**
- Built a custom **CNN** model using **TensorFlow & Keras**
- Applied **image resizing** and **normalization** techniques
- Added interactive **Gradio interface** for real-time predictions
- Visualized model performance using **accuracy and loss plots**

---

## 🧪 Dataset Preprocessing

- **Image Resizing**: All images resized to a consistent shape
- **Normalization**: Pixel values scaled between 0 and 1 using `Rescaling(1./255)`

---

## 🏗️ Model Architecture

The CNN model consists of:

- Input layer: `(IMG_HEIGHT, IMG_WIDTH, 3)`
- Convolutional blocks with filters `[16, 32, 64]`
- MaxPooling layers after each convolution
- Dropout layers: 0.20 and 0.25
- Fully Connected Dense layers: `[128, 64]`
- Output layer: `Dense(4, activation='softmax')` for multiclass classification

---

## ⚙️ Training Details

- **Optimizer**: Adam
- **Loss Function**: Categorical Crossentropy
- **Metrics**: Accuracy
- **Callbacks**: EarlyStopping & ModelCheckpoint to avoid overfitting

---

## 📊 Evaluation & Visualization

- Training & Validation **accuracy/loss curves**
- Sample prediction output showing:
  - 🖼️ Input Image
  - ✅ Actual Label
  - 🔍 Predicted Label

---

## 🚀 Gradio UI

An interactive web UI using **Gradio** allows users to:

- Upload brain MRI images
- Get predicted stage of Alzheimer’s disease
- View confidence scores for all classes


