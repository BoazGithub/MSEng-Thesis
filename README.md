 # CROSS-PROBABILISTIC WEAK SUPERVISION LEARNING FOR HIGH-RESOLUTION LAND COVER ENHANCEMENT 
This research focused on a weak supervision strategy for deep learning aimed at enhancing high-resolution (sub-meter) land cover from historical pseudo (noise) labels. The study involved developing a deep learning architecture that could be supervised
using unified noise or imbalanced datasets as a reasonable training set during the knowledge acquisition phase. The main concern was how to overcome the barriers of spatial resolution mismatch between pairs of
machine learning to train sets derived from high-resolution images representing complex urban features and rural image features, regardless of photogrammetric and heterogeneity in landforms.

## Description


| Image Ref. |      Site     | Image Acquisition Date  |   GT Date   |
| ---------- | ------------- | ----------- | ------------ | 
|   Img (1)  |   The City of Kigali  |  04-03-2023 |  27-06-2023 |
|   Img (2)  |      Bugesera        |  22-07-2023  |  25-08-2023  |  
|   Img (3)  |   Oklahoma State    |  26-08-2022  |  03-80-2022  |  


# Requirements 


[![Python 3.7+](https://img.shields.io/badge/Python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-376/) 
[![Pytorch 1.7.1](https://img.shields.io/badge/Pytorch-1.7.1-blue.svg)](https://pytorch.org/get-started/previous-versions/)
[![torchvision 0.8.2](https://img.shields.io/badge/torchvision-0.8.2-blue.svg)](https://pypi.org/project/torchvision/0.8.2/)
[![Opencv 4.5.5](https://img.shields.io/badge/Opencv-4.5.5-blue.svg)](https://opencv.org/opencv-4-5-5/)
[![CUDA Toolkit 10.1](https://img.shields.io/badge/CUDA-10.1-blue.svg)](https://developer.nvidia.com/cuda-10.1-download-archive-base)
[![Wandb 0.13.10](https://img.shields.io/badge/Wandb-0.13.10-blue.svg)](https://pypi.org/project/wandb/)


# C2FNet Architecture

The study introduced the Coarse-to-Fine Network (C2FNet) framework, which incorporates three key components: Edge Resolution Refinement Backbones (ERRB) for stable feature extraction, Unsupervised Dynamic Shuffle and Diagonal Annotation (UDSDA) for confident area selection and probability assignment based close spatial patterns within multiscale features, and a Contrasting Self-Supervised Loss Function (C2F-Loss) utilizing cosine similarity to guide model learning. The contributions of this study can be summarized as: a) improving the accuracy and robustness of land cover mapping, particularly in regions with complex features, achieving an overall accuracy of 80.01% and a kappa coefficient of 0.7567; and b) maximizing the utilization of available data sources for advanced high-resolution land cover mapping. 
![image](https://github.com/user-attachments/assets/3e163c08-adcd-47ed-9384-504fdadf38f7)

C2FNetwork components:
1. Unsupervised Dynamic Shuffle and Diagonal Annotation
   
![Unsupervised Dynamic Shuffle and Diagonal Annotation_design2_page-0001](https://github.com/user-attachments/assets/d5fcada2-69cc-4545-8aa4-332b9c762795)


# Quantitative Results

![image](https://github.com/user-attachments/assets/64e7d529-28c5-49df-9639-8c562fcab3f2)

# Qualitative Results
![image](https://github.com/user-attachments/assets/8b8f1148-e7b7-46ad-bf9b-31f2b3340ebd)

### 🔭 Baseline:

📖 📖 📖 
- :open_book:	:open_book:	 :open_book: DTCDSCN [[here](https://www.sciencedirect.com/science/article/abs/pii/S0924271622002180)]
- :open_book:	:open_book:	 :open_book: UNet [[here](https://www.int-arch-photogramm-remote-sens-spatial-inf-sci.net/XLIV-4-W3-2020/215/2020/)]
- :open_book:	:open_book:	 :open_book: ResNet50-IMP [[here](https://openaccess.thecvf.com/content_cvpr_2016/papers/He_Deep_Residual_Learning_CVPR_2016_paper.pdf)]
- :open_book:	:open_book:	 :open_book: ResNet50-RSP [[here](https://ieeexplore.ieee.org/abstract/document/9782149)]
- :open_book:	:open_book:	 :open_book: ViTAEv2 [[here](https://arxiv.org/pdf/2202.10108.pdf)]
📖 📖 📖


💬 Dataset Preparation


👉 Data Structure
### Dataset Overview
The sKwanda_V1_d dataset includes 256 × 256 pixel image patches collected from various regions. It is organized into three subsets: train, val, and test, each containing images and their corresponding ground truth labels. This dataset supports tasks such as supervised land cover classification and semantic segmentation.
### sKwanda_V1_d Dataset

The *sKwanda_V1_d* dataset is organized into training, validation, and testing sets, each containing images and ground truth (GT) labels for land cover mapping. The structure is as follows:

### Dataset Structure
import matplotlib.pyplot as plt
import matplotlib.patches as mpatches


### Define the dataset structure
🚚 Datasets


- [x] [sKwanda)V1_dataset_Bugesera][Google Drive Link]([https://drive.google.com/file/d/1W-gnUU-AaYbJ8KMdfnbrI7ySHkiKjOvo/view?usp=drive_link](https://drive.google.com/file/d/1X_Fz7LQIeix3rV3K29FBfKiU1WMdROe-/view?usp=drive_link)


###  Contact Information:


If you have any questions or would like to collaborate, please reach out to me at aiboaz1896@gmail.com or feel free to make issues.

### License: 


The code and datasets are released for non-commercial and research purposes only. For commercial purposes, please contact the authors.

### Acknowledgment:


Appreciate the work from the following repositories:


Planetary Science group at the State key laboratory of information engineering in surveying, mapping and remote sensing of the Wuhan University 

1. L2HNet

2. Related resources:


3. L2HNet dataset


4. Sentine2-Hub


5. ESRI 
