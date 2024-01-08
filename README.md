# 🌟 Image Enhancement Techniques on Mammogram for Breast Cancer Detection

## Table of Contents
1. [Background](#background)
2. [Introduction](#introduction)
3. [Methodology](#methodology)
    - [Dataset](#dataset)
    - [Code and Algorithm](#code-and-algorithm)
4. [Future Works](#future-works)
5. [Conclusion](#conclusion)
6. [References](#references)

---

## 🌐 Background
Cancer refers to the uncontrolled multiplication of cells in particular locations of the body. The cells may form  a lump, microcalcifications, or distortions referred to as tumors. Breast cancers develop from breast cells, the cells may spread through the breast to the lymph  nodes of the body. According to the American Cancer Society, breast cancer contributes to about 30% of all new female cancers each year, and estimated that in 2023, 43700 women will die from breast cancer. 

One of the leading methods of diagnosing breast cancer (BC) is through mammography. This is a method that helps in the early detection of clinically unsuspecting breast cancer among women who are yet to show  signs of breast cancer (asymptomatic). Mammograms employ low-energy X-rays for breast examination and screening and they are sensitive to calcifications. Important signs to look out for in mammograms are clusters of microcalcifications, masses, and architectural distortions. There are two types of mammography, Screening which is the first step, and Diagnosing. Following the results of a screening mammogram, a follow-up diagnostic mammography  is done based on the level of suspicion by the radiologist. 

The human factor involved in the screening process, and detection of suspicious abnormalities is prone to a high degree of error. According to Karthikeyan et al.,  In screening studies, radiologists have an error rate of 10%-30% for detection of cancer. Misinterpretation of breast cancer signs results in 52% of the errors and 43% of the errors are caused due to overlooking signs in abnormal scans. Problems caused by the error rate include biopsies being performed on benign lesions, and false negatives (with its repercussions for the patient, late diagnosis implies lowered chances of survival, and higher treatment costs). A major contributor to these errors is that radiologists depend on visual inspection. In a hospital environment when there is a large number of mammograms, the radiologist may miss out on vital signs while studying the scans due to exhaustion. There are several ways research seeks to improve diagnostic procedures including improved image processing techniques as well as leveraging computer-aided diagnosis (CAD).

Yassir et al., in their work, Image Enhancement Module for Analysis of Mammogram Images for Diagnosis of Breast Cancer, mention that mammography images suffer from low contrast, background noise, and non-coherency among the regions. Leveraging image enhancement techniques, we can circumvent these problems. Image enhancement, by MatLab, is the process of adjusting digital images so that the results are more suitable for display or further image analysis.

## 📝 Introduction
The goal of image enhancement is to increase the radiologists’ confidence in mammogram breast cancer interpretation. Histogram equalization transforms the pixel values in an image, creating a more uniform distribution across the entire range. This process alters pixel values, distributing them between 0 and 255, leading to an increased diversity. While histogram equalization readies a brighter scene for radiologists, caution is necessary as heightened brightness can obscure abnormalities in the image. When employing this technique, it is crucial to carefully consider its application and determine the optimal level of brightness.

## 🛠️ Methodology
a.	Dataset: The dataset was obtained from Kaggle. The images were originally acquired at a breast center located in a university hospital (Centro Hospitalar de S. Joao [CHSJ], Breast Center, Porto) with the permission of the Portuguese National Committee of Data Protection and Hospital's Ethics Committee. The database-INBreast has a total of 115 cases (410 images) from which 90 cases are from women with both breasts affected (four images per case) and 25 cases are from mastectomy patients (two images per case). Several types of lesions (masses, calcifications, asymmetries, and distortions) were included. Accurate contours made by specialists are also provided in XML format. 

b.	Code and Algorithm

     1. Image Enhancement and Segmentation: The image enhancement technique used is histogram equalization, the user uploads a mammogram and the image is enhanced for easy prediction. The segmentation part of the system uses a U-Net convolution network, accepts a mammogram image and its mask, and predicts the location of the tumor. 
     
     2. GUI: The Graphical User Interface was designed in a simple way to display the results of the algorithm. It mainly contains the following widgets:
     
     - Select Button: allows the user to choose an image from the computer and display it.
     - Enhance Button: displays the enhancement results on the chosen image.
     - Segment Button: Displays the Segmentation results on the chosen image.

## 📁 Repository Composition
The repository consists of the following files:
- **README.md:** Overview of the project and its components.
- **gui_code:** Contains the code for the Graphical User Interface.
- **mammogram-project-training:** Includes code and algorithms for image enhancement techniques.
- **GUI-video:** A video demonstrating how the code runs and displays results in the GUI.

## 🔮 Future Works
The future scope involves further refining enhancement techniques and exploring additional algorithms to improve diagnostic accuracy.

## 🎓 Conclusion
Efforts in employing image enhancement techniques aim to augment radiologists' interpretations, enhancing early detection and treatment of breast cancer.

## 🔖 References
- Almalki YE, Soomro TA, Irfan M, Alduraibi SK, Ali A. [Impact of Image Enhancement Module for Analysis of Mammogram Images for Diagnostics of Breast Cancer.](https://www.mdpi.com/1424-8220/22/5/1868) Sensors (Basel). 2022 Feb 26;22(5):1868.
- Ganesan, K., Acharya, U. R., Chua, C. K., Min, L. C., Abraham, K. T., & Ng, K. H. (2013). [Computer-aided breast cancer detection using mammograms: A review.](https://doi.org/10.1109/RBME.2012.2232289) IEEE Reviews in Biomedical Engineering, 6, 77–98.

## 📌 Note
This project was made possible by the contributions of:
- [Mohamad El Zein]
- [Luna Bitar]
- [Joana Owusu-Appiah]
- [Habtamu Yihun]
- [Karim Sleiman]
