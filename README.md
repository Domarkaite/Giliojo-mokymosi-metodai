# Giliojo mokymosi metodai - Deep learning labs

This repository contains a series of labs focusing on deep learning applications in image classification, segmentation, and video-to-text recipe generation.

---

## 📁 Lab 1 – Classification with ResNet50

Image classification using transfer learning on OpenImages data.

### Overview
- Fine-tuned a pretrained ResNet50 model to classify bananas, oranges, and strawberries.

### Highlights
- Collected custom dataset via OpenImages  
- Applied data augmentation and preprocessing  
- Evaluated precision, recall, and F1-scores per class  
- Optimized thresholds for improved multi-class accuracy  

### Metrics
- Banana – 0.64 F1  
- Orange – 0.79 F1  
- Strawberry – 0.84 F1  

---

## 📁 Lab 2 – CNN Classifier with Upload UI

Training a custom convolutional neural network for fruit classification.

### Overview
- Built a deep learning pipeline from data collection to evaluation using a custom CNN.

### Highlights
- Downloaded and split 1500+ OpenImages samples across three fruit classes  
- Implemented data augmentation and train/test pipeline  
- Developed UI for image upload and real-time classification  

### Results
- Accuracy – 0.77  
- F1 Score – 0.77  

---

## 📁 Lab 3 – Image Segmentation with U-Net

Semantic segmentation of roses, oranges, and cars using a custom U-Net model.

### Overview
- Full segmentation pipeline from dataset preparation to Flask deployment.

### Highlights
- Downloaded OpenImages dataset with per-pixel masks using fiftyone  
- Implemented multi-class PyTorch dataset with on-the-fly augmentation  
- Trained custom U-Net with cross-entropy loss, saved best model  
- Evaluated with Dice and F1 scores (excluding background)  
- Deployed UI for real-time image uploads and mask visualization  

### Metrics
- Mean Dice – 0.47  
- Micro F1 – 0.62  
- Macro F1 – 0.62  

---

## 📁 Recipe Generation from Video

Automated generation of cooking recipes from video recordings using video and audio recognition models.

### Overview
- Developed an end-to-end pipeline combining video frame captioning, speech recognition, and recipe generation with GPT-3.5.

### Highlights
- Extracted visual captions using BLIP, GIT, and KOSMOS-2  
- Performed audio transcription with Whisper speech recognition  
- Generated structured recipes by passing captions to GPT-3.5-turbo  
- Evaluated recipe accuracy and content similarity using HuggingFaceFV/finevideo dataset  
- Implemented pipeline in Google Colab with a user-friendly video processing interface  

---

### Setup & Usage

All projects were developed and tested in Google Colab environments. Instructions for running each lab, including dataset download, model training, and inference, are available within respective notebooks.

---

### Technologies Used

- PyTorch  
- OpenImages Dataset  
- Transformers (BLIP, GIT, KOSMOS-2, Whisper)  
- OpenAI GPT-3.5-turbo  
- Flask (for UI deployment)  
- FiftyOne (dataset management and visualization)  

---

### Contact

For questions or collaboration, feel free to reach out!
