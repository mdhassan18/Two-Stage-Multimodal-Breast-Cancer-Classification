# Notebooks

This folder contains the Jupyter notebooks used to implement, train, evaluate, and demonstrate the proposed **two-stage breast cancer analysis system**.

Each notebook is self-contained and corresponds to a specific functional stage of the pipeline.

---

## Notebook List and Description

### 1. Stage1_Screening_Normal_vs_Abnormal.ipynb
- Implements **Stage-1 screening**
- Performs binary classification: **Normal vs Abnormal**
- Designed for high-sensitivity screening
- Uses EfficientNet-B0 as the backbone
- Combines mammogram and ultrasound data using unified screening labels
- Outputs a trained screening model

---

### 2. Stage2_Multimodal_Diagnosis.ipynb
- Implements **Stage-2 diagnostic classification**
- Performs binary classification: **Benign vs Malignant**
- Uses multimodal inputs:
  - Mammogram images (EfficientNet-B0)
  - Ultrasound images (MobileNetV3-Small)
  - Clinical metadata (Age and BIRADS)
- Employs **attention-based late fusion** to weight modality contributions
- Outputs a trained multimodal diagnostic model

---

### 3. Demo_GradCAM_Gradio.ipynb
- Demonstrates the complete two-stage pipeline
- Integrates trained Stage-1 and Stage-2 models
- Provides an interactive **Gradio web interface**
- Visualizes spatial model attention using **Grad-CAM++**
- Displays modality importance through attention weights
- Generates human-readable explanations of model focus

---

## Execution Notes
- Notebooks are designed to run on **Google Colab**
- GPU acceleration is used when available
- File paths assume a consistent project directory structure

---

## Disclaimer
These notebooks are developed for **academic and research purposes only** and are not intended for clinical use.

