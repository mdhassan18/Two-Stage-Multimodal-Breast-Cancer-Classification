# Stage-2 Multimodal Diagnosis Model

This folder contains the deep learning models used for **Stage-2 breast cancer diagnosis** in the proposed two-stage framework.

---

## Objective
The Stage-2 model performs **diagnostic classification** to distinguish between:
- **Benign**
- **Malignant**

This stage focuses on improving diagnostic accuracy by leveraging **multiple complementary data modalities**.

---

## Multimodal Architecture
Stage-2 integrates the following inputs:
- **Mammogram images** processed using EfficientNet-B0
- **Ultrasound images** processed using MobileNetV3
- **Clinical metadata** (Age and BIRADS)

An **attention-based late fusion mechanism** is employed to dynamically weight each modality during inference.

---

## Role in the Pipeline
Stage-2 diagnosis is executed **independently of Stage-1 screening results** to enhance clinical safety and minimize false negatives.

---

## Contents
Typical files stored in this folder include:
- Trained modality-specific model weights
- Attention and fusion module weights
- Final diagnostic model checkpoints

---

## Notes
- Segmentation masks (if available) are not used in the current classification-based implementation
- Large model files may be excluded from version control
- Training and inference logic is implemented in the corresponding notebooks

---

## Disclaimer
This model is developed for **academic and research purposes only** and is not intended for clinical deployment.
