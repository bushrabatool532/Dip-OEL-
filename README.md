Lesion Detection and Segmentation Using Digital Image Processing

Open Ended Lab (OEL) – Digital Image Processing

Project Overview
This project implements an automated skin lesion detection and segmentation system using classical Digital Image Processing (DIP) techniques.
The system processes dermoscopic images from the PH2 Dataset to enhance image quality, remove artifacts such as hair, and accurately segment lesion regions.
The objective of this Open Ended Lab is to demonstrate the practical application of image preprocessing, morphological operations, and threshold-based segmentation for medical image analysis.

Dataset Description
PH2 Dataset is a publicly available dermoscopic image dataset used for skin lesion analysis.

Dataset Characteristics:
High-resolution RGB dermoscopic images
Includes benign and malignant skin lesions
Accompanied by ground truth labels
Widely used in academic research for melanoma detection

Dataset Structure Used:

PH2 Dataset images/
│── IMD001/
│   ├── IMD001.bmp
│── IMD002/
│   ├── IMD002.bmp
│── ...

System Architecture
The system follows a step-by-step image processing pipeline:
Data Loading from Google Drive
Image Enhancement using CLAHE
Hair Removal using Morphological Operations
Lesion Segmentation using Thresholding
Mask Generation and Storage
Performance Evaluation

Tools and Technologies
Python 3
Google Colab
OpenCV
NumPy
Matplotlib
Scikit-learn
Pandas
TQDM

Implementation Steps
Step 0: Environment Setup
Google Drive is mounted to access the dataset
Required libraries are imported

Step 1: Dataset Path Configuration
Paths are defined for:
Original PH2 images
Generated segmentation masks

Label text file

Step 2: Image Preprocessing
1. Image Enhancement (CLAHE)
Contrast Limited Adaptive Histogram Equalization (CLAHE) is applied in the LAB color space to enhance lesion visibility and improve contrast.

Purpose:
Improve clarity of lesion boundaries
Normalize illumination variations

2. Hair Removal
Hair artifacts are removed using:
Black-hat morphological operation
Image inpainting

Purpose:
Remove noise caused by hair
Improve segmentation accuracy

Step 3: Lesion Segmentation
Lesion segmentation is performed using:
Grayscale conversion
Gaussian blurring
Adaptive thresholding
Binary masks are generated where lesion areas are highlighted.

Step 4: Mask Saving
The generated lesion masks are saved in a dedicated directory for further analysis and evaluation.

Step 5: Performance Evaluation
Segmentation performance is evaluated using standard metrics:
Accuracy
Precision
Recall
F1-Score
Ground truth labels are compared with predicted masks.

Results
Enhanced image contrast using CLAHE
Successful removal of hair artifacts
Accurate lesion boundary segmentation
High segmentation accuracy on PH2 dataset
Sample Outputs

The notebook visualizes:
Original image
Enhanced image
Hair-removed image
Binary lesion mask


Learning Outcomes
Practical understanding of medical image preprocessing
Application of morphological operations
Hands-on experience with lesion segmentation
Understanding evaluation metrics in image analysis

Conclusion

This Open Ended Lab project successfully demonstrates a complete lesion detection pipeline using Digital Image Processing techniques. The system effectively enhances dermoscopic images, removes noise, and segments lesion regions, making it suitable for academic and research-based applications.

Author

Bushra Batool
Department of Software Engineering
Open Ended Lab – Digital Image Processing
