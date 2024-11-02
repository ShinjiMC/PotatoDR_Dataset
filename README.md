# PotatoDR Dataset

**By Braulio Nayap Maldonado Casilla and Paul Antony Parizaca Mozo**

The PotatoDR dataset comprises several resources aimed at identifying and classifying various potato leaf diseases. This dataset is crucial for agricultural research and the development of effective solutions to combat plant diseases, particularly for potato crops.

This document summarizes the datasets used in our research, detailing the number of images available for each disease type, and outlines the process of eliminating duplicate and low-quality images to ensure the dataset's integrity.

## Dataset Potato Leaft Status

### Summary of Datasets

| Dataset Name                                            | Source                                                                                  | Number of Images in Healthy | Number of Images in Early Blight | Number of Images in Late Blight |
| ------------------------------------------------------- | --------------------------------------------------------------------------------------- | --------------------------- | -------------------------------- | ------------------------------- |
| Potato Leaf (Healthy and Late Blight)                   | [Mendeley](https://data.mendeley.com/datasets/v4w72bsts5/2)                             | 363                         | -                                | 67                              |
| PlantDoc                                                | [Kaggle](https://www.kaggle.com/datasets/abdulhasibuddin/plant-doc-dataset)             | -                           | 109                              | 97                              |
| Potato Leaf Disease Dataset in Uncontrolled Environment | [Mendeley](https://data.mendeley.com/datasets/ptz377bwb8/1)                             | 201                         | -                                | -                               |
| Potato Leaf Disease Dataset                             | [Kaggle](https://www.kaggle.com/datasets/muhammadardiputra/potato-leaf-disease-dataset) | 400                         | 400                              | 400                             |
| PlantVillage                                            | [Kaggle](https://www.kaggle.com/datasets/emmarex/plantdisease)                          | 152                         | 1000                             | 1000                            |

After aggregating and organizing these datasets, we proceeded to clean the dataset by removing duplicate images and low-quality data to create a refined dataset, yielding:

- Early Blight: 1000 images
- Healthy: 1000 images
- Late Blight: 1000 images

### Process of Duplicate Removal

During the dataset preparation, we implemented a process to identify and eliminate duplicate images. This was accomplished using perceptual hashing techniques to compare images visually and programmatically. The steps included:

1. **Hashing**: Each image was processed to generate a unique hash based on its visual content.
2. **Grouping**: Images with matching hashes were grouped together as duplicates.
3. **Removal**: From each group of duplicates, we retained only one image and removed the others to ensure a clean dataset.

This process not only streamlined our dataset but also ensured that it contained high-quality images that represent the different potato leaf diseases effectively.

## Potato Leaf Types of Disease

The Potato Leaf Disease Dataset in Uncontrolled Environment contains various images representing different types of potato leaf diseases. It is essential for training models that can accurately classify and detect these diseases in agricultural settings. The dataset includes:

| Disease Type | Number of Images |
| ------------ | ---------------- |
| Bacteria     | 569              |
| Fungi        | 748              |
| Nematode     | 68               |
| Pest         | 611              |
| Phytophthora | 347              |
| Virus        | 532              |

These images are critical for developing machine learning models that can assist farmers and agricultural specialists in identifying diseases early and accurately, thus improving crop yields and food security.

## References

1. [Tilahun, Natnael (2022), “Potato Leaf (Healthy and Late Blight)”, Mendeley Data, V2, doi: 10.17632/v4w72bsts5.2](https://data.mendeley.com/datasets/v4w72bsts5/2)
2. [Singh, D., Jain, N., Jain, P., Kayal, P., Kumawat, S., & Batra, N. (2020). “Plantdoc: A dataset for visual plant disease detection,” in Proceedings of the 7th ACM IKDD CoDS and 25th COMAD doi: 10.1145/3371158.3371196](https://www.kaggle.com/datasets/abdulhasibuddin/plant-doc-dataset)
3. [Shabrina, Nabila Husna; Indarti, Siwi; Maharani, Rina; Kristiyanti, Dinar Ajeng; Irmawati, Irmawati; Prastomo, Niki; M, Tika Adillah (2023), “Potato Leaf Disease Dataset in Uncontrolled Environment”, Mendeley Data, V1, doi: 10.17632/ptz377bwb8.1](https://data.mendeley.com/datasets/ptz377bwb8/1)
4. [A. Muhammad (2021), “Potato leaf disease dataset,”](https://www.kaggle.com/datasets/muhammadardiputra/potato-leaf-disease-dataset)
5. [J. D. Michalewicz, R. Malekzadeh, and J. D. Brantley (2021), “Plantvillage dataset”](https://www.kaggle.com/datasets/emmarex/plantdisease)
