# Arabic Sign Language (ArSL) Recognition

**Computer Vision Project – University of Nebraska-Lincoln**

This project focuses on developing a preprocessing pipeline for Arabic Sign Language (ArSL) gesture recognition using computer vision techniques. The system leverages MediaPipe for efficient hand detection and image cropping, preparing high-quality hand images for further classification and real-time recognition.

---

## 📌 Abstract

This project aims to detect and recognize Arabic Sign Language (ArSL) gestures for the deaf and hard-of-hearing communities in Arabic-speaking regions. Using MediaPipe, a state-of-the-art hand-tracking framework, the system extracts hand regions from gesture images, enabling robust preprocessing for future gesture classification. The pipeline addresses challenges such as missed detections and noisy backgrounds, laying the foundation for inclusive assistive technology.

---

## 📖 Introduction

Arabic Sign Language (ArSL) is a vital communication tool for individuals with hearing and speech impairments in Arabic-speaking communities. This project leverages computer vision and machine learning to develop a system capable of detecting and preparing ArSL gestures for automated recognition. By focusing on accurate hand detection and cropping, the project enables the creation of robust models for ArSL gesture classification.

---

## 🛠️ Methodology

The project follows a two-step approach:

### 1. Hand Detection
- Utilizes **MediaPipe Hands** to detect hands and estimate bounding boxes around detected hands.
- MediaPipe’s pre-trained model ensures precise hand landmark detection.

### 2. Cropping with MediaPipe
- Implements a custom function (`detect_and_crop_hand_mediapipe`) to:
  - Read and convert images to RGB.
  - Detect hands using MediaPipe.
  - Compute bounding boxes with optional padding.
  - Crop hand regions and convert them back to RGB for visualization.

---

## 📊 Results

- **Total Images Processed:** 14,202
- **Hands Successfully Cropped:** 13,317 (92.57% success rate)
- **Hands Missed:** 885
- **Validation Accuracy:** 92.57%
- **Loss:** 0.2233

The system demonstrates strong performance in extracting high-quality hand regions, even in challenging scenarios with complex backgrounds or occlusions. Confusion matrix analysis highlights the model’s ability to distinguish between visually similar classes.

---

## 🔮 Future Work

- **Data Augmentation:** Enhance the dataset using techniques like rotation, scaling, and flipping.
- **Real-Time Applications:** Extend the system to recognize gestures in real-time using live video feeds.
- **Model Fine-Tuning:** Explore advanced models like YOLOv5 for improved performance.

---

## ✅ Conclusion

This project successfully developed a preprocessing pipeline for Arabic Sign Language recognition, focusing on efficient hand detection and image cropping. By leveraging MediaPipe, the system achieved over 92% accuracy in processing hand images, overcoming challenges such as missed detections and noisy backgrounds. This work underscores the importance of computer vision in creating inclusive solutions for diverse communities.

---

## 📚 References

- Kaggle Dataset: [Arabic Sign Language Dataset 2022](https://www.kaggle.com/datasets/ammarsayedtaha/arabic-sign-language-dataset-2022?resource=download)

---

## 🖼️ Visuals

- **Figure 1:** Arabic Sign Language Letter
- **Figure 2:** Confusion Matrix
- **Figure 3:** Evaluation Matrix
- **Figure 4:** Original vs Cropped Image
- **Figure 5:** Sample Missed Crop
- **Figure 6:** Sample Predictions

---

**Contributors:** University of Nebraska-Lincoln, Computer Vision Team  
**License:** MIT
