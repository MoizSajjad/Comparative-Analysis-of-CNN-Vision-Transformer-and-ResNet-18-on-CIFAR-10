# Comparative Analysis of CNN, Vision Transformer, and ResNet-18 on CIFAR-10

This repository contains the implementation and experimental evaluation of three deep learning architectures for image classification on the CIFAR-10 dataset:
- A custom Convolutional Neural Network (CNN)
- A Vision Transformer (ViT) trained from scratch
- A ResNet-18 model using transfer learning from ImageNet

The goal is to analyze performance trade-offs in terms of accuracy, parameter efficiency, inference speed, and class-wise behavior.

---

## 📊 Models Implemented

### 1. CNN Baseline
- Lightweight architecture with ~620K parameters  
- Achieves the best overall performance  
- Test Accuracy: **71.13%**  
- Fastest inference time

### 2. Vision Transformer (ViT)
- Patch-based transformer architecture  
- ~3.2M parameters  
- Test Accuracy: **64.63%**  
- Shows strong potential but requires more training

### 3. ResNet-18 (Transfer Learning)
- Pretrained on ImageNet  
- Only final layer fine-tuned (~5K parameters)  
- Test Accuracy: **40.30%**  
- Performance limited due to aggressive layer freezing

---

## 📁 Dataset
- **CIFAR-10**
- 60,000 RGB images (32×32) across 10 classes  
- Train / Validation / Test split: 45k / 5k / 10k  
- Standard normalization and data augmentation applied

---

## 🧪 Evaluation Metrics
- Accuracy  
- Macro Precision  
- Macro Recall  
- Macro F1-Score  
- Confusion Matrices  
- Inference Time per Image

---

## ⚙️ Experimental Setup
- Framework: PyTorch  
- Optimizers: Adam, AdamW  
- Training Epochs: 5  
- Batch Size: 128  
- Environment: Google Colab (GPU)

---

## 🚀 Interactive Demo
A Gradio-based web interface allows real-time image classification using all three models, enabling easy comparison of predictions.

---

## 📌 Key Findings
- CNN offers the best accuracy-to-parameter and speed trade-off  
- ViT performs competitively but needs longer training or stronger augmentation  
- Transfer learning requires careful fine-tuning for small-resolution datasets

---

## 🔮 Future Work
- Train models for more epochs  
- Apply advanced augmentation (MixUp, CutMix)  
- Fine-tune deeper layers of ResNet-18  
- Explore pretrained or hybrid CNN–Transformer models

---

## 👤 Author
**Moiz Sajjad**  
Department of Data Science  
FAST NUCES, Islamabad
