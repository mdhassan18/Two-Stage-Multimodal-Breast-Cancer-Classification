# Models

This folder contains the trained deep learning models used in the proposed two-stage breast cancer analysis framework.  
The models are organized according to their role in the pipeline to ensure modularity, reproducibility, and clear separation of screening and diagnosis tasks.

---

## Stage-1: Screening Models

**Objective:** Binary classification (Normal vs Abnormal)

Stage-1 models are designed for **high-sensitivity screening** to identify potentially abnormal breast images.  
These models operate independently and are optimized to minimize false negatives.

Typical contents:
- Trained CNN weights
- Architecture-specific configurations
- Evaluation checkpoints

---

## Stage-2: Diagnosis Models

**Objective:** Binary classification (Benign vs Malignant)

Stage-2 performs **multimodal diagnosis** by integrating multiple data sources:
- Mammogram images (EfficientNet-B0)
- Ultrasound images (MobileNetV3)
- Clinical metadata (Age, BIRADS)

An **attention-based late fusion mechanism** is used to dynamically weight each modality during inference.

Typical contents:
- Individual modality models
- Fusion and attention module weights
- Final diagnostic model checkpoints

---

## Notes
- Large model weight files may be excluded from the repository and managed locally
- Model loading paths are configurable within the training and inference notebooks
- The folder structure supports future extensions and retraining

---

## Disclaimer
All models are developed for **academic and research purposes only** and are not intended for clinical deployment.
