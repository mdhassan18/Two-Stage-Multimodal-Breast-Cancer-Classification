# Notebooks

This folder contains the Jupyter notebooks used for development, training, evaluation, and demonstration of the proposed two-stage breast cancer analysis framework.

Each notebook is modular and corresponds to a specific stage or function within the pipeline.

---

## Notebook Overview

### Stage-1 Screening
- Implements the screening model for Normal vs Abnormal classification
- Includes data loading, preprocessing, training, and evaluation
- Designed for high-sensitivity screening

### Stage-2 Multimodal Diagnosis
- Implements the diagnostic model for Benign vs Malignant classification
- Integrates mammogram images, ultrasound images, and clinical metadata
- Uses attention-based late fusion for multimodal learning

### Gradio Demo
- Deploys the complete system using a web-based interface
- Supports image upload and real-time inference
- Visualizes predictions and model attention outputs

---

## Notes
- Notebooks are structured for execution in Google Colab
- File paths are relative and configurable
- Model weights are loaded from the `models` directory

---

## Usage
Notebooks may be executed independently or sequentially depending on the experimental requirements.

---

## Disclaimer
These notebooks are intended for **academic and research purposes only** and are not designed for clinical deployment.
