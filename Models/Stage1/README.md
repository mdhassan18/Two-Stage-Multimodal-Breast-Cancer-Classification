# Stage-1 Screening Model

This folder contains the deep learning model used for **Stage-1 breast cancer screening** in the proposed two-stage framework.

---

## Objective
The Stage-1 model performs **binary classification** to distinguish between:
- **Normal**
- **Abnormal**

The primary goal of this stage is **high-sensitivity screening**, ensuring that potentially abnormal cases are not missed.

---

## Model Characteristics
- Convolutional Neural Network (CNN) based architecture
- Optimized for sensitivity rather than specificity
- Operates independently from Stage-2 diagnosis

---

## Role in the Pipeline
Stage-1 acts as an initial screening module.  
However, to enhance clinical safety, **Stage-2 diagnosis is executed regardless of the Stage-1 output**, reducing the risk of false negatives.

---

## Contents
Typical files stored in this folder include:
- Trained model weights
- Architecture definitions
- Checkpoints and evaluation artifacts

---

## Notes
- Large weight files may be excluded from version control
- Model loading and inference are handled within the corresponding notebooks

---

## Disclaimer
This model is developed strictly for **academic and research purposes** and is not intended for clinical use.
