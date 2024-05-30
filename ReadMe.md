# LungCNet: A CNN for Accurate Lung Cancer Detection from CT Scans

## Problem Statement

Lung cancer has been a major global health challenge and a leading cause of death worldwide. Detecting lung cancer is crucial for improving patient outcomes. Traditional methods, such as imaging techniques and biopsy procedures, while useful, come with challenges in detecting lung cancer. These methods often suffer from limited sensitivity, specificity, and inefficiencies when interpreting complex medical images such as CT scans. Due to these limitations, diagnosis can be delayed, and false positive/negative results can occur, leading to sub-optimal treatment planning for patients.

These challenges highlight the urgent need for advanced and reliable methods. Existing techniques struggle to accurately identify and characterize tumors due to variability in their appearance, location, and stage across different patients. The inefficient interpretation of large, multidimensional medical imaging data by human experts further compounds the problem.

This dissertation aims to address these challenges by developing and validating LungCNet, an innovative convolutional neural network (CNN) tailored for the accurate detection and classification of lung cancer from CT scans. The primary objectives are to design a CNN architecture specifically suited for the complexities of lung cancer imaging, incorporating advanced image processing algorithms and novel data augmentation techniques to effectively handle tumor variability. LungCNet will leverage its unique features to overcome the diagnostic limitations of current methods, improving sensitivity, specificity, and efficiency.

The research will rigorously evaluate LungCNet's performance using a comprehensive and diverse dataset of CT scans collected from the Iraq-Oncology Teaching Hospital/National Center for Cancer Diseases, including images across various stages of lung cancer and healthy controls. A comparative analysis will be conducted to assess LungCNet's diagnostic accuracy, sensitivity, and specificity against other state-of-the-art CNN models applied to the same dataset.

## Objectives

The main aim of this research is to develop and validate LungCNet, an innovative convolutional neural network (CNN) designed for the accurate detection and classification of lung cancer from CT scans, thereby improving the efficiency and reliability of lung cancer detection. To achieve this aim, the research has several key objectives:

1. Develop LungCNet by designing a tailored CNN architecture specifically crafted for the complexities of lung cancer imaging, incorporating advanced image processing algorithms and novel data augmentation techniques to effectively handle the variability in tumor appearance and location.
2. Leverage LungCNet's unique features to overcome the limitations of sensitivity, specificity, and diagnostic efficiency encountered with current lung cancer detection methods.
3. Evaluate LungCNet's performance using a comprehensive and diverse dataset of CT scans collected from the Iraq-Oncology Teaching Hospital/National Center for Cancer Diseases, which includes images across various stages of lung cancer as well as healthy controls.
4. Conduct a comparative analysis to assess LungCNet's diagnostic accuracy, sensitivity, and specificity against other state-of-the-art CNN models applied to the same dataset.
5. Open-source LungCNet's codebase and documentation on platforms like GitHub to facilitate knowledge transfer, foster collaboration, and further innovation in the application of AI to medical detection.

## Brief Literature Review

Cancer remains a predominant global health challenge, ranking as a leading cause of mortality worldwide (World Health Organization, 2022). Early detection improves patient outcomes and survival rates across various cancer types. Lung cancer is one of the most frequently diagnosed cancers, accounting for a significant portion of new cases and cancer-related deaths globally (Schabath & Cote, 2019).

Traditional diagnostic methods for lung cancer, such as imaging techniques and biopsies, often face limitations in sensitivity, specificity, and efficiency in interpreting complex medical images (Pulumati et al., 2023). These limitations can lead to delays in diagnosis, false positives/negatives, and suboptimal treatment planning, adversely affecting patient prognosis (Schlemmer et al., 2018; Liu et al., 2023).

In response to these challenges, researchers have explored applying machine learning (ML) and artificial intelligence (AI) techniques for lung cancer detection. Studies have demonstrated the potential of AI models to enhance the precision, consistency, and speed of various diagnostic tools, outperforming conventional methods in terms of accuracy, sensitivity, and specificity (Ardila et al., 2019; Gandhi et al., 2023).

Convolutional Neural Networks (CNNs), a deep learning model, have shown promise in lung cancer detection from medical imaging data. CNNs excel at extracting hierarchical features from raw data, making them well-suited for complex pattern recognition tasks (Yamashita et al., 2018). Several studies have developed CNN-based algorithms tailored for lung cancer detection and classification, utilizing various datasets and approaches (Pandian et al., 2022; Teramoto et al., 2017; Heuvelmans et al., 2021; Al-Huseiny & Sajit, 2021; Solyman & Schwenker, 2023).

Despite these advancements, challenges remain, particularly concerning the limitations of existing datasets, such as label inaccuracies, data imbalances, and the need for further improvements in model accuracy (Mahimkar, 2022). Ongoing research aims to address these gaps and further enhance the capabilities of AI-based lung cancer detection methods.

## Gaps in Current Research

The IQ-OTH/NCCD dataset used in this research suffers from limitations regarding accurate true labels, especially for the training images, posing a challenge in effectively training the model. There is no accompanying true label for each of the images during training. Additionally, the dataset exhibits a high degree of class imbalance, which can introduce bias and degrade the model's performance in accurately detecting underrepresented classes. Finally, existing research on this dataset often struggles with overfitting, where models perform well on the training data but fail to generalize effectively to unseen data.

This research is going to address these gaps.

## Contributions of the Research

This research makes significant strides in lung cancer detection by developing LungCNet, an innovative convolutional neural network tailored for this task. Key contributions include:

- Advanced preprocessing and data augmentation techniques to enhance the model's ability to handle tumor variability in appearance and location across CT scans.
- Introduction of novel convolutional layers and specialized training algorithms designed to boost diagnostic accuracy, achieving an impressive 99% classification accuracy.
- Promotion of knowledge transfer by making LungCNet's codebase openly available, fostering collaboration and further advancements in applying AI for medical applications.

Through these innovative approaches, the research overcomes challenges in lung cancer detection, represents a significant leap forward in accurate and efficient classification, and paves the way for improved patient outcomes through early detection.

## Data and Modelling

The research utilized a comprehensive dataset of 1,190 DICOM images collected from the Iraq-Oncology Teaching Hospital/National Center for Cancer Diseases (IQ-OTH/NCCD) over three months in 2019. This dataset encompassed CT scans from a diverse patient cohort, including images representing various stages of lung cancer as well as healthy controls.

Extensive data preparation was carried out, involving image resizing, normalization, and augmentation techniques. These preprocessing steps aimed to enhance the model's training process and overall performance.

The proposed model, LungCNet, features a tailored convolutional neural network (CNN) architecture specifically designed for lung cancer detection and classification from CT scans. The architecture incorporates convolutional, pooling, and fully connected layers, along with regularization techniques such as dropout. This design enables the extraction of hierarchical features from the CT scan images, facilitating precise predictions.

![LungCNet Architecture](path_to_image_1)

The model development followed the CRISP-DM (Cross-Industry Standard Process for Data Mining) framework, ensuring a systematic approach to data mining and model development. The training and evaluation processes employed various metrics, including accuracy, precision, recall, and F1-score, to comprehensively assess LungCNet's performance.

Notably, LungCNet outperformed other pre-trained models like VGG16, ResNet50, InceptionV3, and MobileNetV2, particularly in handling class imbalance and hyperparameter tuning. This superior performance highlights the efficacy of the proposed model architecture and the tailored approach adopted in this research.

![LungCNet Performance Comparison](path_to_image_2)

## Findings

This research successfully demonstrated that LungCNet, the proposed convolutional neural network, significantly improves lung cancer detection and classification accuracy compared to traditional methods and other CNN models. Key findings from the study include:

- LungCNet's high classification accuracy of 99%, outperforming other models that have utilized the same dataset for their research.
- The model exhibited robust performance across various evaluation metrics, effectively handling class imbalance and reducing overfitting issues often encountered by pre-trained models.
- LungCNet's strong and consistent performance highlights its potential for integration into clinical diagnostic workflows, offering a promising avenue for improving early lung cancer detection and enhancing patient outcomes through timely and accurate treatment.

The success of this tailored CNN architecture underscores the transformative potential of deep learning techniques in the realm of medical image analysis and lung cancer diagnosis.
