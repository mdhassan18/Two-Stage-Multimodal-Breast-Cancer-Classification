# Datasets

This project uses two publicly available breast imaging datasets for multimodal diagnosis.  
All datasets were **cleaned, reorganized, and indexed manually**, and custom CSV files were created to make them fully training-ready and compatible with deep learning pipelines and Google Colab environments.  
Due to ethical and privacy constraints, the actual image data is not included in this repository.

---

## Dataset 1: CBIS-DDSM (Mammogram – Diagnosis)

### Folder Structure

CBIS-DDSM/  
├── jpeg/  
│ ├── SeriesInstanceUID  
│ │ ├── image1.jpg  
│ │ └── image2.jpg (optional)  
├── csv/    
│ │ ├── calc_case_description_test_set.csv  
│ │ ├── calc_case_description_train_set.csv   
│ │ ├── dicom_info.csv  
│ │ ├── mass_case_description_test_set.csv  
│ │ ├── mass_case_description_train_set.csv  
│ │ └──meta.csv  
└── train_ready.csv  


### CSV Format (`train_ready.csv`)  
image_path,label  
jpeg/<SeriesInstanceUID>/image.jpg,0  
jpeg/<SeriesInstanceUID>/image.jpg,1  


### Labels
- 0 → Benign  
- 1 → Malignant  

Each row represents a single mammogram image. Image paths are relative and Colab-compatible.

---

## Dataset 2: BUSI (Ultrasound – Diagnosis)

### Folder Structure

Dataset_BUSI_with_GT/  
├── normal/  
├── benign/  
└── malignant/  
busi_train_ready.csv  


### CSV Format (`busi_train_ready.csv`)  

image_path,mask_path,label  
Dataset_BUSI_with_GT/benign/benign (1).png,  
Dataset_BUSI_with_GT/benign/benign (1)_mask.png,1  


### Labels
- 0 → Normal  
- 1 → Benign  
- 2 → Malignant  

Segmentation masks are available but are not used in the current classification-based implementation.

---

## Ethical Notice
Medical imaging data is excluded from this repository. Users may obtain the datasets from official sources and follow the documented structure and CSV formats for reproducibility.


