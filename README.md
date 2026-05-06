# 🔢 MNIST Digit Classification: Advanced ML Pipeline
> A comprehensive machine learning project evolving from fundamental binary classification to a sophisticated multiclass system using **Ensemble Learning** and **Deep Feature Extraction**.

[![Python](https://img.shields.io/badge/Language-Python-blue?style=flat-square&logo=python)](https://www.python.org/)
[![Framework](https://img.shields.io/badge/Library-Scikit--Learn-orange?style=flat-square&logo=scikit-learn)](https://scikit-learn.org/)
[![Status](https://img.shields.io/badge/Phase-2--Optimized-green?style=flat-square)]()

## 📖 Project Overview
This project demonstrates an end-to-end machine learning pipeline for classifying handwritten digits from the **MNIST dataset**. The workflow transitioned through two distinct phases: establishing a baseline with binary classification and scaling to a high-performance multiclass solution using advanced optimization and feature engineering.

### 🧩 Core Pipeline Components
*   **Preprocessing:** Data normalization, feature scaling, and stratified splitting.
*   **Custom Algorithms:** From-scratch implementations of Softmax Regression, Linear SVM, and Random Forest.
*   **Optimization:** Stratified K-Fold Cross-Validation, L2 Regularization, and Bias-Variance diagnostic analysis.

---

## 🚀 Phase 1: Binary Classification (3 vs 8)
The initial phase focused on distinguishing between the digits "3" and "8", selected specifically for their high visual similarity and classification challenge.

### 🛠️ Strategic Implementation
*   **Problem Definition:** Supervised binary classification on $28 \times 28$ grayscale images.
*   **Feature Representations:** Comparative evaluation using **Raw Pixels**, **PCA** (50 dimensions), and **HOG** (Histogram of Oriented Gradients).
*   **Top Performer:** The **Linear SVM with HOG** features achieved the best performance with a validation F1-score of **0.9948**.

---

## 🖥️ Phase 2: Multiclass Optimization & Improvements
Phase 2 expanded the scope to all 10 digits (0–9) and introduced advanced architectural improvements to handle increased complexity and prevent overfitting[cite: 4].

### 🛠️ Advanced Model Enhancements
*   **Feature Engineering (CNN):** Leveraged a pretrained **MobileNetV2** model to extract high-level feature vectors, capturing complex spatial patterns that surpassed raw pixel representations.
*   **Ensemble Learning:** Implemented a **Random Forest** from scratch to capture non-linear relationships and reduce model variance.
*   **Hyperparameter Tuning:** Utilized **Stratified K-Fold Cross-Validation** to identify optimal learning rates and regularization strengths.
*   **Performance Diagnostics:** Plotted **Learning Curves** and conducted bias-variance analysis to ensure the final model was well-balanced.

---

## 📊 Performance Comparison
The hybrid approach combining Deep Learning for feature extraction and classical ML for classification proved most effective.

| Model Implementation | Feature Type | Optimization Strategy | Validation F1-Score |
| :--- | :--- | :--- | :--- |
| **Linear SVM** | **Pretrained CNN** | **Deep Feature Extraction** | **0.9392** |
| Softmax Regression | Raw Pixels | L2 Regularization + CV | 0.9163 |
| Linear SVM | Raw Pixels | Cross-Validation | 0.9056 |
| Random Forest | Raw Pixels | Ensemble Voting | 0.8305 |

---

## 🤝 The Team
This project was a collaborative effort by a team of 5 engineering students at **Ain Shams University (ASU)**:

*   **👨🏻‍💻 Omar Ahmed Abouraia**
*   **👨🏻‍💻 Hossam Osama Hussieny**
*   **👩🏻‍💻 Mariam Ibrahim Assr**
*   **👩🏻‍💻 Mariam Tarek Farouk**
*   **👩🏻‍💻 Lujain Mohamed**

---

## 🔗 Project Resources
*   📂 **[Full Phase 1 Technical Report](./Docs/MNIST_Phase1_Report.pdf)**
*   📂 **[Full Phase 2 Technical Report](./Docs/MNIST_Phase2_Report.pdf)**
*   📓 **[Phase 1 Implementation Notebook](./Phase1_MNIST_Binary_Classification.ipynb)**
*   📓 **[Phase 2 Optimization Notebook](./Phase2_Multiclass_Classification_Improvement.ipynb)**

---

## 🌟 Support & Feedback

⭐ **Give it a Star** to support the project!
💡 **Have suggestions or found a bug?**  
- 🐛 Open an issue for bugs
- Or reach out directly using the links below
 

## 📬 Contact

<p align="center">

<a href="mailto:omara862005@gmail.com?subject=TinyTelemetry%20Feedback&body=Hi%20Eng.%20Omar%20Abouraia,%0A%0AI%20would%20like%20to%20share%20some%20feedback...">
  <img src="https://img.shields.io/badge/Email-Contact%20Me-red?style=for-the-badge&logo=gmail&logoColor=white"/>
</a>

<a href="https://www.linkedin.com/in/omarabouraia/">
  <img src="https://img.shields.io/badge/LinkedIn-Omar%20Abouraia-blue?style=for-the-badge&logo=linkedin&logoColor=white"/>
</a>

---

*Developed as part of the Introduction to Machine Learning Course (CSE382), Junior Semester 5, 2026.*
