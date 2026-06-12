# Link :
https://pavan190602.github.io/BrainTDDL/


# BrainTDDL
CNN Deep Learning
# 🧠 Brain Tumor Detection Using CNN

> A hybrid deep learning approach combining **Morphological Filtering** and **Convolutional Neural Networks** for accurate, efficient brain tumor diagnosis from MRI scans.

---

## 📌 Overview

Brain tumor detection is a critical and challenging task in medical imaging that directly impacts patient outcomes. This project proposes a **hybrid detection system** that merges morphological filtering with a multi-layer CNN to preprocess, extract features from, and classify brain MRI images — achieving improved accuracy and faster diagnosis over conventional approaches.

The interactive web demo allows users to upload MRI scans and watch the full CNN pipeline execute step-by-step: preprocessing → feature extraction → classification → diagnostic report.

---

## 🎯 Key Features

- **Interactive Demo** — Upload 1–5 MRI images and visualize each pipeline stage in real time
- **3-Step CNN Pipeline** — Morphological preprocessing, deep feature extraction, and Softmax classification
- **Multiclass Output** — Detects and classifies multiple tumor types (not just binary detection)
- **Tumor Localization** — Annotates detected regions directly on scan images
- **Diagnosis Report** — Confidence scores and brain region identification per image
- **Dark / Light Mode** — Full theme toggle with CSS variable-based design
- **Responsive UI** — Works across desktop and mobile screen sizes

---

## 🔬 Research Abstract

Brain tumors have continued to increase over the last decade across several countries. Interpretation of MRI images is challenging due to the complexity of the brain's anatomy and variability in tumor characteristics.

This study proposes an approach combining **morphological filtering** and **Convolutional Neural Networks (CNNs)**. Images are first preprocessed using morphological filtering to enhance contrast and remove noise from brain MRI scans, then the CNN model classifies extracted features using backpropagation and gradient descent to minimize classification error on labeled images.

---

## 🧩 CNN Architecture

| Layer | Details |
|---|---|
| **Input** | Brain MRI scan image |
| **Conv Layer 1** | 32 filters — low-level edge & structure features |
| **Max Pooling** | Spatial dimension reduction |
| **Conv Layer 2** | 64 filters — mid-level texture features |
| **Conv Layer 3** | 128 filters — complex tumor pattern recognition |
| **Flatten** | Feature map → vector |
| **FC Layer 1** | Dense 512 units |
| **Dropout** | Rate 0.5 — regularization to prevent overfitting |
| **FC Layer 2** | Dense 256 units |
| **Output** | Softmax multiclass classification |

---

## 🔄 Processing Pipeline

```
MRI Input → Morphological Filtering → Feature Extraction → Classification → Diagnosis Output
   (01)              (02)                    (03)               (04)             (05)
```

1. **MRI Input** — Raw brain MRI scans loaded into the system
2. **Morphological Filtering** — Contrast enhancement, noise removal, tumor region extraction
3. **Feature Extraction** — CNN convolutional layers extract texture and spatial features
4. **Classification** — Fully connected layers with Softmax classify tumor type
5. **Diagnosis Output** — Tumor presence, type, confidence score, and brain region reported

---

## 🦠 Tumor Types Detected

- **Gliomas** — tumors of glial cells (most common type)
- **Meningiomas** — arise from the meninges (brain lining)
- **Pituitary Adenomas** — affecting hormone regulation
- **Metastatic Tumors** — spread from other body organs
- **Astrocytomas** — from astrocyte star-shaped cells
- **Ependymomas** — lining of the brain ventricles

---

## 🗂️ Tech Stack

| Category | Tools |
|---|---|
| **Deep Learning** | TensorFlow / Keras |
| **Language** | Python 3.x |
| **Image Processing** | OpenCV (morphological filtering) |
| **Data Handling** | NumPy, Pandas |
| **Visualization** | Matplotlib, Seaborn |
| **Evaluation** | Scikit-learn |
| **Frontend Demo** | HTML5, CSS3, Vanilla JavaScript |

---

## 📚 Datasets

- [Brain MRI Images Dataset — Kaggle](https://www.kaggle.com/navoneel/brain-mri-images-for-brain-tumor-detection)
- [BRATS — Brain Tumor Segmentation Challenge Dataset](https://www.med.upenn.edu/cbica/brats/)
- Labeled tumor / no-tumor MRI training images
- Medical imaging research literature (IEEE, PubMed)

---

## 🛠️ Techniques & Patterns

- Encoder-Decoder pattern for feature compression
- Sliding Window for tumor localization
- Multi-scale Feature Extraction
- Morphological Opening / Closing operations
- Transfer Learning (pre-trained weights)
- Data Augmentation (flip, rotate, zoom)
- Batch Normalization for training stability
- Adam Optimizer with categorical cross-entropy loss

---

## 🚀 Getting Started

### Prerequisites

```bash
Python 3.8+
pip
```

### Installation

```bash
# Clone the repository
git clone https://github.com/your-username/brain-tumor-detection-cnn.git
cd brain-tumor-detection-cnn

# Install dependencies
pip install -r requirements.txt
```

### Run the Web Demo

Simply open `index.html` in any modern browser — no server required.

### Train the Model

```bash
python train.py --dataset ./data/mri_images --epochs 50 --batch_size 32
```

### Run Inference

```bash
python predict.py --image path/to/mri_scan.jpg
```

---

## 📁 Project Structure

```
brain-tumor-detection-cnn/
│
├── index.html              # Interactive web demo (frontend)
├── train.py                # Model training script
├── predict.py              # Inference / prediction script
├── model/
│   └── cnn_model.h5        # Trained Keras model weights
├── data/
│   ├── tumor/              # Tumor-positive MRI images
│   └── no_tumor/           # Tumor-negative MRI images
├── notebooks/
│   └── brain_tumor_cnn.ipynb   # Jupyter notebook with full walkthrough
├── utils/
│   ├── preprocessing.py    # Morphological filtering functions
│   └── evaluation.py       # Metrics and report generation
├── requirements.txt
└── README.md
```

---

## 📊 Model Performance

| Metric | Value |
|---|---|
| **Accuracy** | ~95%+ (on validation set) |
| **Loss Function** | Categorical Cross-Entropy |
| **Optimizer** | Adam |
| **Regularization** | Dropout (0.5) |
| **Augmentation** | Rotation, Flip, Zoom |

---

## 👥 Research Team

**Pavan Kumar**
B.Tech CSE – Internet of Things, Malla Reddy College of Engineering & Technology
🎓 MSCS · University of Central Missouri, USA
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?logo=linkedin)](https://www.linkedin.com/in/yvpavankumar/)

**Sahith Reddy**
B.Tech CSE – Internet of Things, Malla Reddy College of Engineering & Technology
🎓 MSCS · Texas A&M University – Corpus Christi
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?logo=linkedin)](https://www.linkedin.com/in/sahith-reddy-013a87219/)

**Katta Shivani**
B.Tech CSE – Internet of Things, Malla Reddy College of Engineering & Technology
🎓 MS in Data Science · University of Arkansas at Little Rock
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?logo=linkedin)](https://www.linkedin.com/in/shivani-reddy-katta/)

---

## 🏫 Institution

**Malla Reddy College of Engineering & Technology (MRCET)**
Affiliated with Jawaharlal Nehru Technological University Hyderabad (JNTUH)

---

## 🔑 Keywords

`Brain Tumor Detection` `Convolutional Neural Networks` `Morphological Filtering` `Medical Imaging` `MRI Images` `Feature Extraction` `Deep Learning` `Multiclass Segmentation` `Computer-Aided Diagnosis` `Backpropagation` `Image Preprocessing` `Classification`

---

## 📄 License

This project is intended for **academic and research purposes only**. It is not a certified medical diagnostic tool. Always consult a qualified medical professional for clinical decisions.

---

## ⚠️ Disclaimer

> This system is a research prototype and should **not** be used as a substitute for professional medical diagnosis. All results are for educational and demonstration purposes only.
