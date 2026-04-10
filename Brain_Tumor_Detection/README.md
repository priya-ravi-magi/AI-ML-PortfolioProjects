# 🧠 Brain Tumor Detection using Deep Learning

Dive into medical imaging using AI! This project explores how deep learning can be used to detect brain tumors from MRI scans. Using Convolutional Neural Networks (CNN), the model analyzes image patterns and classifies scans as **Tumor** or **Healthy**.

Deep learning implementation? Check it out in the `code/` folder.

---

# 📌 Background

Brain tumors are critical medical conditions that require early detection for effective treatment. Traditionally, MRI scans are analyzed manually by radiologists, which can be time-consuming and subject to human error.

With advancements in Artificial Intelligence, deep learning models like CNNs can automatically learn patterns from medical images and assist in faster and more accurate diagnosis.

This project focuses on building an end-to-end AI system for brain tumor detection using MRI images.

---

# ❓ Key Questions I Wanted to Answer

1. Can deep learning accurately detect brain tumors from MRI scans?  
2. How well does the model generalize to unseen data?  
3. What is the trade-off between precision and recall?  
4. How effective is data augmentation in improving performance?  
5. Can this approach support real-world medical diagnosis?  

---

# 📂 Dataset

- Source: Kaggle Brain Tumor Dataset  
- Total Images: ~5000  
- Classes:
  - Tumor  
  - Healthy  
- Data Type: MRI & CT images  

---

# ⚙️ Data Preparation

## 🧹 Data Cleaning & Preprocessing
- Resized images to 224×224  
- Normalized pixel values (0–1)  
- Converted labels into binary format  

## 🔄 Data Augmentation
- Rotation  
- Zoom  
- Horizontal flipping  

👉 Helps improve model generalization and reduce overfitting  

## 📊 Data Splitting
- Training set  
- Validation set  
- Test set  

---

# 🤖 Model Development

A Convolutional Neural Network (CNN) was built with:

- 3 Convolutional Layers (32, 64, 128 filters)  
- Batch Normalization  
- MaxPooling Layers  
- Dropout (to prevent overfitting)  
- Dense Layer (128 neurons)  
- Sigmoid Output Layer (binary classification)  

---

# 📈 Model Training

- Optimizer: Adam  
- Loss Function: Binary Cross Entropy  
- Metrics:
  - Accuracy  
  - Precision  
  - Recall  

Callbacks used:
- EarlyStopping  
- ReduceLROnPlateau  

---

# 📊 Results & Insights

## ✅ Model Performance
- Test Accuracy: **94.4%**
- Precision: ~0.94–0.95  
- Recall: ~0.92–0.96  

👉 The model shows strong and balanced performance across both classes.

---

# 📉 Key Findings

- CNN effectively learns tumor patterns from MRI images  
- Data augmentation significantly improved model performance  
- Model achieved high accuracy with minimal misclassification  
- Balanced precision and recall ensure reliable predictions  

---

# 📊 Confusion Matrix Summary

|                | Predicted Healthy | Predicted Tumor |
|----------------|------------------|-----------------|
| **Actual Healthy** | 367 (TN)         | 33 (FP)         |
| **Actual Tumor**   | 23 (FN)          | 577 (TP)        |

---

# 📸 Sample Predictions

Each prediction includes:
- True Label  
- Predicted Label  
- Confidence Score  

---

# 🛠️ Tools & Technologies Used

- Python  
- TensorFlow / Keras  
- OpenCV  
- NumPy, Pandas  
- Matplotlib  

---

# 📁 Project Structure

```bash
Brain_Tumor_Detection/
│
├── code/
├── data/
├── outputs/
├── model/
├── docs/
└── README.md
```

---

# ⚙️ How to Run

```bash
pip install -r requirements.txt
jupyter notebook code/brain_tumor_detection.ipynb
```

---
# 📄 Documentation

```bash
Detailed explanation of the project, methodology, and results can be found in:

docs/project_report.pdf
```

---
# 🧾 Conclusion

This project demonstrates the effectiveness of Convolutional Neural Networks (CNNs) in detecting brain tumors from MRI images. The model successfully learned complex visual patterns and achieved a strong test accuracy of 94.4%, with balanced precision and recall across both classes.

The results highlight that deep learning can significantly improve the speed and reliability of medical image analysis, reducing dependency on manual interpretation. Data preprocessing and augmentation techniques further enhanced the model’s ability to generalize to unseen data.

Overall, this project shows the potential of AI in supporting healthcare professionals by providing efficient and accurate diagnostic assistance.

---
# 📊 Insights Gained

Deep learning models like CNNs are highly effective for image classification tasks
Data preprocessing plays a critical role in improving model performance
Data augmentation helps reduce overfitting and improves generalization
Balanced evaluation metrics (precision & recall) are important in medical applications
Model performance depends heavily on data quality and distribution

---
# 🎓 What I Learned

End-to-end machine learning pipeline for image classification
Working with medical imaging datasets (MRI scans)
Building and training CNN models using TensorFlow/Keras
Importance of model evaluation metrics beyond accuracy
Techniques to handle overfitting (Dropout, Data Augmentation)
Structuring and presenting projects for real-world applications

---
# 🚀 Future Improvements

* Transfer Learning (ResNet, EfficientNet) for better performance
* Increase dataset size for improved generalization
* Implement model explainability (Grad-CAM)
* Deploy as a web application for real-world use
* Hyperparameter tuning using tools like Optuna

---
# 👨‍💻 Author

Master’s Student in Artificial Intelligence & Machine Learning
