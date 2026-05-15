# 🎓 Smart University Identity Recognition System

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Machine Learning](https://img.shields.io/badge/Machine_Learning-SVM_%7C_CNN_%7C_KNN-orange.svg)
![Computer Vision](https://img.shields.io/badge/Computer_Vision-PCA-green.svg)

## 📌 Project Overview
Many universities still rely on manual identification procedures, such as checking ID cards or matching faces visually. These procedures are often slow, ineffective, and susceptible to mistakes, adding to the workload of lecturers and creating opportunities for impersonation. 

This project introduces an innovative implementation of a **Smart University Identity Recognition System** utilizing the power of Computer Vision and Machine Learning. The system is capable of automatically recognizing university members using their facial images, providing a secure, robust, and fast alternative to manual identity verification.

## 🎯 Objectives
* Develop and test a system capable of identifying individuals from facial images.
* Achieve high accuracy and rapid processing speeds.
* Evaluate the feasibility of implementing this automated identification system in a real-world university environment.

## 📊 Dataset
This project uses the **Labeled Faces in the Wild (LFW)** dataset, one of the most widely recognized benchmarks for face recognition. 
* Contains images captured under various lighting conditions, poses, and facial expressions.
* A filtered subset of **7 distinct identities** was used to ensure a stable and balanced training set.

## ⚙️ System Pipeline
The architecture follows a standard, reproducible machine learning pipeline:
1. **Data Loading & Preprocessing:** Formatting images for uniform analysis.
2. **Exploratory Data Analysis (EDA):** Visualizing class distributions and sample images.
3. **Feature Extraction (PCA):** Principal Component Analysis (PCA) was applied to extract the most significant facial features (Eigenfaces), reducing dimensionality and filtering out noise.
4. **Model Training:** Training both classical and deep learning models.
5. **Model Evaluation:** Comparing accuracy, confusion matrices, and computational cost.

## 🧠 Models & Performance
This project serves as an apples-to-apples comparison between classical machine learning and deep learning methodologies:
* **K-Nearest Neighbors (KNN):** Performed poorly (~61%) due to high sensitivity to the curse of dimensionality.
* **Convolutional Neural Network (CNN):** Achieved strong accuracy (~81%), representing the deep learning approach.
* **Support Vector Machine (SVM):** Achieved strong accuracy (~82%), representing the classical approach when paired with PCA.

## 🏆 Conclusion & Best Model
The **SVM combined with PCA** was selected as the optimal model for this prototype. 

While both the CNN and SVM achieved approximately 81-82% accuracy, the SVM + PCA pipeline required significantly less computational power. This balance of high accuracy and high efficiency makes it the most realistic and deployable solution for a university system.

## 🚧 Limitations
* The prototype relies on a relatively small dataset (7 identities), which affects generalization.
* It currently processes static images and does not yet support real-time camera-based recognition.
* Extreme variations in lighting, pose, and background are not fully covered in the current scope.

## 🚀 Future Work
* **Real-Time Integration:** Implement live face recognition through a webcam/camera feed.
* **System Interface:** Connect the AI directly to the university's attendance and administrative databases.
* **Pipeline Expansion:** Incorporate robust face detection (e.g., Haar Cascades or MTCNN) and face tracking alongside a significantly larger university database.

---
**Author:** Maryam Fagbo 
*Computer Science Major | Aspiring AI & Machine Learning Engineer*
