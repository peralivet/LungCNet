A detailed summary of this research is below but this project contains three files that were used for the experiment as well as the dataset.

The dataset for this project can be find here: ![Project Dataset Link](https://www.kaggle.com/datasets/adityamahimkar/iqothnccd-lung-cancer- dataset/data).

While there are three files for the project because three different experiment were run for the project. All three files are included in this project as well as a detailed report on how everything was achieved.

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

![LungCNet Architecture](https://github.com/peralivet/LungCNet/blob/71d40c801d9415532083ba9e4f7769e26cbd6e57/Screenshot%202024-05-30%20at%201.26.31%20PM.png)

The model development followed the CRISP-DM (Cross-Industry Standard Process for Data Mining) framework, ensuring a systematic approach to data mining and model development. The training and evaluation processes employed various metrics, including accuracy, precision, recall, and F1-score, to comprehensively assess LungCNet's performance.

Notably, LungCNet outperformed other pre-trained models like VGG16, ResNet50, InceptionV3, and MobileNetV2, particularly in handling class imbalance and hyperparameter tuning. This superior performance highlights the efficacy of the proposed model architecture and the tailored approach adopted in this research.

![LungCNet Performance Comparison](https://github.com/peralivet/LungCNet/blob/71d40c801d9415532083ba9e4f7769e26cbd6e57/Screenshot%202024-05-30%20at%202.34.19%20PM.png)

## Findings

This research successfully demonstrated that LungCNet, the proposed convolutional neural network, significantly improves lung cancer detection and classification accuracy compared to traditional methods and other CNN models. Key findings from the study include:

- LungCNet's high classification accuracy of 99%, outperforming other models that have utilized the same dataset for their research.
- The model exhibited robust performance across various evaluation metrics, effectively handling class imbalance and reducing overfitting issues often encountered by pre-trained models.
- LungCNet's strong and consistent performance highlights its potential for integration into clinical diagnostic workflows, offering a promising avenue for improving early lung cancer detection and enhancing patient outcomes through timely and accurate treatment.

The success of this tailored CNN architecture underscores the transformative potential of deep learning techniques in the realm of medical image analysis and lung cancer diagnosis.

## References

1. World Health Organization. (2023, June 26). Lung cancer. World Health Organization. https://www.who.int/news-room/fact-sheets/detail/lung-cancer.
2. Schabath, M. B., & Cote, M. L. (2019). Cancer progress and priorities: Lung cancer. Cancer Epidemiology, Biomarkers & Prevention, 28(10), 1563–1579. https://doi.org/10.1158/1055-9965.EPI-19-0221.
3. Pulumati, A., Vattikonda, N. A., Nagalla, R. K., Samyuktha, K., & Savanur, A. (2023). Technological advancements in cancer detection: Improvements and limitations. Cancer Reports, 6(2), Article e1764. https://doi.org/10.1002/cnr2.1764.
4. Schlemmer, H.-P., Bittencourt, L. K., D'Anastasi, M., Domingues, R., Khong, P.- L., Lockhat, Z., Muellner, A., Reiser, M. F., Schilsky, R. L., & Hricak, H. (2018). Global challenges for cancer imaging. Journal of Global Oncology, 4, 1-10. https://doi.org/10.1200/JGO.17.00036.
5. Ardila, D., Kiraly, A. P., Bharadwaj, S., Choi, B., Reicher, J. J., Peng, L., Tse, D., Etemadi, M., Ye, W., Corrado, G., Naidich, D. P., & Shetty, S. (2019). End-to-end lung cancer screening with three-dimensional deep learning on low-dose chest computed tomography. Nature Medicine, 25(6), 954–961. https://doi.org/10.1038/s41591-019-0447-x.
6. Yamashita, R., Nishio, M., Do, R. K. G., & Togashi, K. (2018). Convolutional neural networks: An overview and application in radiology. Insights into Imaging, 9(4), 611–629. https://doi.org/10.1007/s13244-018-0639-9.
7. Pandian, R., Christofer, S. A., Karthick, R., Dhanalakshmi, A., Mohamed Uvaze Ahamed, A., & Somasundaram, S. (2022). Detection and classification of lung cancer using CNN and Google Net. Measurement: Sensors, 24, Article 100588. https://doi.org/10.1016/j.measen.2022.100588.
8. Heuvelmans, M. A., Van Ooijen, P. M. A., Ather, S., Silva, C. F., Han, D., Heußel, C. P., Hickes, W., Kauczor, H., Novotný, P., Peschl, H., Rook, M., Rubtsov, R. V., Von Stackelberg, O., Tsakok, M., Arteta, C., Declerck, J., Kadir, T., Pickup, L. C., Gleeson, F., & Oudkerk, M. (2021). Lung cancer prediction by Deep Learning to identify benign lung nodules. Lung Cancer, 154, 1–4. https://doi.org/10.1016/j.lungcan.2021.01.027.
9. Teramoto, A., Tsukamoto, T., Kiriyama, Y., & Fujita, H. (2017). Automated classification of lung cancer types from cytological images using deep convolutional neural networks. BioMed Research International, 2017, Article 4067832. https://doi.org/10.1155/2017/4067832.
10. Al-Huseiny, M. S., & Sajit, A. S. (2021). Transfer learning with GoogLeNet for the detection of lung cancer. Indonesian Journal of Electrical Engineering and Computer Science, 22(2), 1078-1086. https://doi.org/10.11591/ijeecs.v22.i2.pp1078-1086.
11. Solyman, S., & Schwenker, F. (2023). Lung tumor detection and recognition using deep convolutional neural networks. In E. Klyuev & V. Evdokimova (Eds.), Computational science and its applications – ICCSA 2022 workshops (pp. 79–91). Springer International Publishing. https://doi.org/10.1007/978-3-031-31327-1_5.
12. Mahimkar, A. (2022). IQ-OTH/NCCD - Lung Cancer Dataset. Www.kaggle.com. https://www.kaggle.com/datasets/adityamahimkar/iqothnccd-lung-cancer- dataset/data.
13. Kareem, H. F., AL-Husieny, M. S., Mohsen, F. Y., Khalil, E. A., & Hassan, Z. S. (2021). Evaluation of SVM performance in the detection of lung cancer in marked CT scan dataset. Indonesian Journal of Electrical Engineering and Computer Science, 21(3), 1731-1738. https://doi.org/10.11591/ijeecs.v21.i3.pp1731-1738.
14. Al-Yasriy, H. F., AL-Husieny, M. S., Mohsen, F. Y., Khalil, E. A., & Hassan, Z. S. (2020). Diagnosis of lung cancer based on CT scans using CNN. IOP Conference Series: Materials Science and Engineering, 928, Article 022035. https://doi.org/10.1088/1757-899X/928/2/022035.
15. NARİN, D., & ONUR, T. Ö. (2022). The Effect of Hyper Parameters on the Classification of Lung Cancer Images Using Deep Learning Methods. Erzincan Üniversitesi Fen Bilimleri Enstitüsü Dergisi, 15(1), 258–268. https://doi.org/10.18185/erzifbed.1006560.
16. Mohamed, T. I. A. (2022). Optimized deep learning model for early detection and classification of lung cancer on CT images. Researchspace.ukzn.ac.za. https://researchspace.ukzn.ac.za/items/709e7d7a-d095-4b90-982c- 43c384a41f17.
