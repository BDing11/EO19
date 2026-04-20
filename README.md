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

The download link for the dataset is https://www.kaggle.com/datasets/dingbiao11/eo19-a-large-dataset-for-insect-identification

# Comprehensive Evaluation of EO19 Performance
Following a comprehensive evaluation of ten candidate models, YOLOv13n demonstrated superior overall performance. Building upon this result, we developed an interface tailored to practical application scenarios based on the YOLOv13 framework. Using this interface, we conducted an extensive assessment of the EO19 dataset across multiple classification categories, examining detailed parameter performance. The evaluation encompassed detection outcomes for both adult and larval classification images, including case studies of false negatives and false positives with corresponding cause analyses. In addition, video-based detection experiments were performed to illustrate the EO19 dataset’s capability in dynamic environments, thereby highlighting its feasibility for deployment in real-time monitoring contexts. Due to space limitations, the full details of these experiments are provided in https://github.com/BDing11/EO19_Test_Results_based_on_YOLOv13.
