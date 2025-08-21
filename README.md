# 🧠 Brain Tumor Segmentation using CNN (U-Net)

This project implements a **U-Net Convolutional Neural Network (CNN)** for **brain tumor segmentation** using **MRI scans**.  
The model classifies each pixel of an MRI image as **tumor** or **non-tumor**, providing an automated assistive tool for medical professionals.

---

## 📌 Project Overview
Brain tumor diagnosis through MRI imaging is crucial but manual segmentation is time-consuming and error-prone.  
This project leverages **deep learning with U-Net architecture** to automate the segmentation process.

- **Architecture:** U-Net (encoder-decoder with skip connections)  
- **Dataset:** MRI brain tumor images with corresponding masks  
- **Frameworks:** TensorFlow / Keras, OpenCV, NumPy, Scikit-learn  
- **Results:**
  - Precision: **83.5%**
  - Recall: **77.8%**
  - Dice Coefficient: **80.6%**

---

## 📊 Dataset
- Source: [Kaggle – Brain Tumor Segmentation](https://www.kaggle.com/datasets/nikhilroxtomar/brain-tumor-segmentation)  
- **Total Images:** 3,064  
- **Format:**  
  - MRI scan (`.jpg` / `.png`)  
  - Binary mask (annotated tumor regions)  

**Preprocessing Steps:**
- Resize all images to **256 × 256**
- Normalize pixel values
- Convert masks to **binary (0/1)**
- Train/Test split (e.g., 80/20)

---

## 🏗️ Model Architecture
The U-Net model consists of:
- **Encoder (Contracting path):** Extracts features with Conv2D + ReLU + MaxPooling layers  
- **Bridge:** Bottleneck convolution layers  
- **Decoder (Expansive path):** Upsampling + skip connections to recover spatial details  
- **Output Layer:** 1×1 convolution with **sigmoid** activation for binary segmentation  

📌 Techniques used:
- Dropout layers (to prevent overfitting)  
- Adam optimizer (lr=0.001)  
- Early stopping with patience = 3  

---

## **👨‍💻 Author**
### ***Bhargavkumar Panchal***

GitHub: @bbhargavpanchal

LinkedIn: https://www.linkedin.com/in/bhargavpanchall/




📞 Support

Email: bhargavpanchal5151@gmail.com


⭐ If you find this project useful, please consider giving it a star!
