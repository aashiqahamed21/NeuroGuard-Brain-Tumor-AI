# 🏥 NeuroGuard-MRI-Diagnosis

![Python](https://img.shields.io/badge/Python-3.9%2B-blue)
![PyTorch](https://img.shields.io/badge/PyTorch-Medical%20AI-orange)
![Streamlit](https://img.shields.io/badge/Streamlit-Clinical%20Dashboard-red)
![License](https://img.shields.io/badge/License-MIT-green)

**NeuroGuard-MRI-Diagnosis** is an enterprise-grade AI workstation designed for the automated detection and classification of brain tumors from **T1-Weighted MRI scans**. 

By leveraging **Deep Learning (ResNet18)** and **Explainable AI (Grad-CAM)**, this system provides radiologists with a "second opinion" on complex cases, classifying scans into four diagnostic categories: **Glioma, Meningioma, Pituitary Tumor, and No Tumor**.

---

## 📋 Clinical Capabilities

### 1. 🧠 Automated Tumor Classification
* **Multi-Class Detection:** Instantly identifies Glioma, Meningioma, and Pituitary anomalies.
* **High Sensitivity:** Optimized for **T1-Weighted Contrast Enhanced** images.
* **Real-Time Inference:** Delivers diagnostic predictions in <2 seconds.

### 2. 🔬 Explainable AI (XAI) Layer
* **Grad-CAM Visualization:** Generates a heatmap overlay to show *exactly* which region of the brain triggered the diagnosis.
* **Trust & Transparency:** Moves beyond "Black Box" predictions by visually justifying the AI's reasoning to the clinician.

### 3. 🛠️ Image Enhancement Engine
* **Quality Control:** Integrated brightness and contrast calibration tools to normalize poor-quality scans from older MRI machines.
* **Pre-Processing:** Automatic resizing and normalization of DICOM/JPG inputs.

### 4. 📄 Professional Reporting System
* **Automated PDF Generation:** Compiles a full "referral-ready" medical report.
* **Electronic Signature:** Includes the digital signature of the attending physician (Dr. Aashiq Ahamed N).
* **Patient History Mock-up:** Simulates an Electronic Health Record (EHR) environment for demonstration.

---

## ⚙️ Technical Architecture

* **Model Architecture:** ResNet18 (Pre-trained on ImageNet, Fine-tuned on Brain Tumor MRI Dataset)
* **Frontend:** Streamlit (Custom CSS for Dark/Light Medical Themes)
* **Backend:** PyTorch & Torchvision
* **Report Engine:** FPDF (Python PDF Generation)

---

## 🚀 Installation & Usage

To run this diagnostic suite locally:

1.  **Clone the Repository**
    ```bash
    git clone [https://github.com/YourUsername/NeuroGuard-MRI-Diagnosis.git](https://github.com/YourUsername/NeuroGuard-MRI-Diagnosis.git)
    cd NeuroGuard-MRI-Diagnosis
    ```

2.  **Install Dependencies**
    ```bash
    pip install -r requirements.txt
    ```

3.  **Launch the Dashboard**
    ```bash
    streamlit run app.py
    ```

---

## 📂 Repository Structure

```bash
NeuroGuard-MRI-Diagnosis/
├── app.py                  # Main Clinical Dashboard Application
├── neuroguard_model.pth    # Trained PyTorch Weights (ResNet18)
├── requirements.txt        # Python Dependencies
├── Demo_Images/            # Reference MRI Scans (T1-Weighted)
└── README.md               # System Documentation
