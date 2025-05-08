Indian Currency Detection Dataset

This repository contains a curated dataset for detecting Indian currency notes using object detection models like YOLOv5. It includes images of various denominations, annotated with bounding boxes to highlight important features such as denomination numbers, watermark areas, and security threads.

Dataset Structure

-Images: Stored in `.jpg` and `.png` formats.
-Annotations: YOLO format (plain text).
-Data Splits:
  - Training: 70% (~3500 images)
  - Validation: 20% (~1000 images)
  - Test: 10% (~500 images)

Dataset Features

-Image Format: JPEG, PNG
-Dimensions: Standardized to 640x640 pixels
-Labels: Bounding boxes for:
  - Denomination
  - Watermark
  - Security thread
-Scaling: Pixel values normalized between 0 and 1

Preprocessing

- Verified and cleaned corrupted images
- Standardized file names
- Annotations converted using LabelImg
- Augmentation with Albumentations: flips, rotations, lighting changes

Annotations

- Format: YOLOv5 (x_center, y_center, width, height)
- Classes: Defined in `data.yaml`
- Tags: Each bounding box is labeled with class tags such as `Denomination`, `Watermark`, `Security Thread`

Tools Used

- LabelImg (for annotation)
- Albumentations (for augmentation)
- Python + YOLOv5 (for model training/testing)

Privacy & Security

- No PII included
- Dataset is public and non-sensitive, so no encryption applied

Version Control

- Managed with Git for reproducibility
- Logs maintained for dataset evolution

Visualization & Analysis

- Histograms of class distribution
- Scatter plots of bounding box dimensions
- Sample images with overlayed annotations for inspection

Licensing & Usage

- License: Subject to open-source or proprietary terms as defined by the dataset owner
- Owner: Vijay S P
- Source: GitHub (https://github.com/Vijay-Ponnusamy/Indian-Currency-Detection.git)

Contact
For queries or contributions, please contact the dataset owner or raise an issue in this repository.

