# EO19
A Large Dataset Construction for Insect Identification and Multi-Model Performance Assessment

We provide six types of datasets in this GitHub repository:

1. Raw images and labels without train/val/test splits.  
This package contains the original images along with both VOC‑format and YOLO‑format annotations. It is intended for users who wish to create their own customized dataset splits based on specific experimental needs.

2. Pre‑split datasets in VOC, YOLO, and JSON formats (8:1:1).  
These datasets follow an 8:1:1 train/validation/test division and correspond exactly to the versions used in our paper, ensuring full reproducibility of our experiments.

3. Augmented and randomly reduced datasets (YOLO format).  
These datasets are generated through data augmentation and random down‑sampling. Each category contains 1000 images with corresponding YOLO‑format labels, providing a controlled environment for studying data‑scale effects.

4. Traditional classification‑style dataset (YOLO format).  
This dataset serves as a control group in our study. It follows a conventional classification scheme where adult and larval stages are not treated as separate categories. Users aiming to reproduce our comparative experiments or requiring a simplified taxonomy may use this version.
