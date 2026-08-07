# 🍎 Fruit Image Classification using a Custom CNN

A deep learning project that implements a **Custom Convolutional Neural Network (CNN)** for **multiclass fruit image classification**.

The model was developed using **TensorFlow/Keras** and trained on the **Fruits-360 Dataset**, achieving excellent classification performance across a large number of fruit categories.

The proposed architecture combines **Data Augmentation**, **Batch Normalization**, **Dropout**, and **Global Average Pooling** to improve generalization while maintaining a lightweight model.

---

# 🎯 Model Performance

| Metric | Score |
|--------|-------:|
| **Training Accuracy** | **99.35%** |
| **Validation Accuracy** | **99.28%** |
| **Test Accuracy** | **97.40%** |

These results demonstrate the effectiveness of the proposed CNN architecture for multiclass fruit image recognition.

---

# 📂 Project Structure

```text
Fruit-Image-Classification-Custom-CNN/
│
├── Fruit_Classification.ipynb
├── README.md
├── requirements.txt


---

# ⚙️ Requirements

Install the required libraries:

```bash
pip install tensorflow numpy pandas matplotlib seaborn scikit-learn
```

### Dependencies

- Python 3.x
- TensorFlow / Keras
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

---

# 📥 Dataset

The project uses the **Fruits-360 Dataset** available on Kaggle.

**Dataset Link**

https://www.kaggle.com/datasets/moltean/fruits

The dataset contains thousands of high-quality images belonging to numerous fruit categories, making it suitable for multiclass image classification tasks.

---

# 🏗️ Model Architecture

The proposed CNN architecture consists of:

- Input Layer (100 × 100 × 3)
- Image Rescaling
- Data Augmentation
- Five Convolutional Feature Extraction Blocks
- Batch Normalization
- ReLU Activation
- Max Pooling
- Global Average Pooling
- Fully Connected Layer (512 neurons)
- Dropout Regularization
- Fully Connected Layer (256 neurons)
- Softmax Output Layer

---

# 🧠 Network Architecture

### Block 1

- Conv2D (32 Filters)
- ReLU Activation
- Batch Normalization

### Block 2

- Conv2D (64 Filters)
- ReLU Activation
- Batch Normalization

### Block 3

- Conv2D (128 Filters)
- MaxPooling2D
- ReLU Activation
- Batch Normalization

### Block 4

- Conv2D (128 Filters)
- MaxPooling2D
- ReLU Activation
- Batch Normalization

### Block 5

- Conv2D (256 Filters)
- MaxPooling2D
- ReLU Activation
- Batch Normalization

### Classification Head

- GlobalAveragePooling2D
- Dense (512 neurons, ReLU)
- Dropout (0.5)
- Dense (256 neurons, ReLU)
- Dropout (0.2)
- Softmax Output Layer

---


# 📊 Final Results

| Metric | Accuracy |
|---------|---------:|
| Training Accuracy | **99.35%** |
| Validation Accuracy | **99.28%** |
| Test Accuracy | **97.40%** |

The model demonstrates excellent classification performance with strong generalization on unseen fruit images.

---

# 🧮 Model Summary

| Property | Value |
|----------|-------|
| Input Size | 100 × 100 × 3 |
| Total Parameters | 868,164 |
| Trainable Parameters | 866,948 |
| Non-trainable Parameters | 1,216 |
| Model Size | 3.31 MB |

---

# ✨ Key Features

- Custom CNN built entirely from scratch.
- Data Augmentation for improved robustness.
- Image normalization using Rescaling.
- Batch Normalization for stable and faster convergence.
- ReLU activation across convolutional layers.
- Global Average Pooling instead of Flatten.
- Dropout Regularization to reduce overfitting.
- Lightweight architecture (~868K parameters).
- High multiclass classification accuracy.
- TensorFlow/Keras implementation.
- Easily deployable for desktop, web, or mobile applications.

---

# 📝 Training Configuration

| Parameter | Value |
|-----------|-------|
| Image Size | 100 × 100 |
| Optimizer | Adam |
| Learning Rate | 0.0005 |
| Loss Function | Sparse Categorical Crossentropy |
| Activation | ReLU |
| Output Activation | Softmax |
| Pooling | MaxPooling2D |
| Final Pooling | GlobalAveragePooling2D |
| Dense Layers | 512 → 256 |
| Dropout | 0.5 / 0.2 |

---

# 🍓 Applications

This model can be applied to:

- Smart Fruit Recognition
- Automated Fruit Sorting
- Agricultural AI Systems
- Grocery Store Automation
- Food Quality Inspection
- Retail Inventory Management
- Mobile Fruit Identification Apps
- Educational Computer Vision Projects

---

# 📌 Conclusion

This project demonstrates that a carefully designed **Custom Convolutional Neural Network (CNN)** can achieve **97.40% test accuracy** for multiclass fruit image classification.

By integrating:

- Data Augmentation
- Batch Normalization
- Dropout Regularization
- Global Average Pooling

the model achieves excellent classification performance while maintaining a lightweight architecture suitable for real-world computer vision applications.

---

## ⭐ If you found this project useful, consider giving it a star!
