# 🐄 Multi-View Cattle Biometric System with Open-Set Recognition

Deep Metric Learning for Livestock Identification using Face and Muzzle Biometrics.

---

## 📌 Overview

This project presents a multi-view biometric identification system for cattle using deep metric learning.  
The system leverages both **face** and **muzzle** images to build robust identity embeddings and supports **open-set recognition**, enabling reliable rejection of unknown cattle.

The architecture combines convolutional feature extraction with transformer-based contextual modeling and is trained using margin-based metric learning for enhanced class separation.

---

## 🧠 System Architecture

### 🔹 1. Deep Learning Pipeline

- **Backbone:** Pretrained ResNet50
- **Context Modeling:** Transformer encoder with multi-head attention
- **Loss Function:** ArcFace (angular margin loss)
- **Embedding Learning:** Metric learning framework for discriminative identity representation

The model is trained to maximize inter-class separation while maintaining compact intra-class clustering in embedding space.

---

### 🔹 2. Multi-Modal Fusion

The system processes:

- 🐮 Cattle Face Images  
- 🐮 Cattle Muzzle Images  

Each modality generates an embedding vector.  
Final identity verification is performed using:

- Weighted cosine similarity fusion  
- Gallery-based comparison  
- Validation-driven threshold tuning  

This improves robustness compared to single-view biometric systems.

---

### 🔹 3. Open-Set Recognition

Unlike closed-set classifiers, this system can:

- ✅ Accept known cattle  
- ❌ Reject unknown cattle  
- ⚠️ Flag low-confidence cases  

A conservative decision mechanism is implemented to minimize false acceptance rates, making the system practical for real-world farm deployment.

---

## 📦 Pretrained Models

Due to GitHub file size limits, pretrained models are hosted on Google Drive.

### 🔹 Face Model  
Download here:  
https://drive.google.com/uc?export=download&id=16zn0njzq5QPAzQho_XHI9HcXtKRSvK5l

### 🔹 Muzzle Model  
Download here:  
https://drive.google.com/uc?export=download&id=1tMqKbR_8-B9Lw_hgzaxohRXLxRVG6WEk

After downloading, place the models inside:
/models/


---

## 🚀 Installation

```bash
git clone https://github.com/your-username/Multi-View-Cattle-Biometric-System-with-Open-Set-Recognition.git
cd Multi-View-Cattle-Biometric-System-with-Open-Set-Recognition

pip install -r requirements.txt

▶️ Usage

1.Download pretrained models (see above).

2.Place them in the models/ directory.

3.Run inference:
python inference.py
4.For training:

🧪 Methodology Summary

Transfer learning using ImageNet-pretrained backbone

Transformer-enhanced feature aggregation

ArcFace-based metric learning

Cosine similarity verification

Threshold optimization for open-set decisioning
🛠️ Technologies Used

Python

PyTorch

ResNet50

Transformer Encoder

ArcFace Loss

Metric Learning

Transfer Learning
📊 Key Contributions

Multi-view biometric fusion for livestock identification

Transformer-enhanced metric learning pipeline

Open-set recognition framework for unknown cattle detection

Practical decision threshold calibration
📄 License

This project is intended for research and academic use.
🤝 Acknowledgements

This work explores the application of deep metric learning to agricultural biometric systems, contributing toward scalable and automated livestock management solutions.

---

### Why this looks authentic and natural:
- Clear technical explanation without buzzword stuffing  
- Professional but not over-polished  
- Structured like real ML research repos  
- Clean formatting and realistic sectioning  
- No exaggerated claims  

---
