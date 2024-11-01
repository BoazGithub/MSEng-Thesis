 # CROSS-PROBABILISTIC WEAK SUPERVISION LEARNING FOR HIGH-RESOLUTION LAND COVER ENHANCEMENT 
This research focused on a weak supervision strategy for deep learning aimed at enhancing high-resolution (sub-meter) land cover from historical pseudo (noise) labels. The study involved developing a deep learning architecture that could be supervised
using unified noise or imbalanced datasets as a reasonable training set during the knowledge acquisition phase. The main concern was how to overcome the barriers of spatial resolution mismatch between pairs of
machine learning to train sets derived from high-resolution images representing complex urban features and rural image features, regardless of photogrammetric and heterogeneity in landforms.
# Dataset

- [x] [sKwanda)V1_dataset_Bugesera][Google Drive Link]([https://drive.google.com/file/d/1W-gnUU-AaYbJ8KMdfnbrI7ySHkiKjOvo/view?usp=drive_link](https://drive.google.com/file/d/1X_Fz7LQIeix3rV3K29FBfKiU1WMdROe-/view?usp=drive_link)

# Requirements 




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
- :open_book:	:open_book:	 :open_book: DTCDSCN [[here](https://ieeexplore.ieee.org/abstract/document/9311793)]
- :open_book:	:open_book:	 :open_book: UNet [[here](https://www.int-arch-photogramm-remote-sens-spatial-inf-sci.net/XLIV-4-W3-2020/215/2020/)]
- :open_book:	:open_book:	 :open_book: FC-Siam [[here](https://ieeexplore.ieee.org/abstract/document/8451652)]
- :open_book:	:open_book:	 :open_book: SNUNet–ECAM [[here](https://ieeexplore.ieee.org/abstract/document/9355573)]
- :open_book:	:open_book:	 :open_book: Siam-Nested-UNet [[here](https://dl.acm.org/doi/abs/10.1145/3437802.3437810)]
- :open_book:	:open_book:	 :open_book: ResNet50-IMP [[here](https://openaccess.thecvf.com/content_cvpr_2016/papers/He_Deep_Residual_Learning_CVPR_2016_paper.pdf)]
- :open_book:	:open_book:	 :open_book: ResNet50-RSP [[here](https://ieeexplore.ieee.org/abstract/document/9782149)]
- :open_book:	:open_book:	 :open_book: Swin–T-RSP [[here](https://ieeexplore.ieee.org/abstract/document/9782149)]
- :open_book:	:open_book:	 :open_book: Swin-T-IMP [[here](https://ieeexplore.ieee.org/abstract/document/9736956)]
- :open_book:	:open_book:	 :open_book: ViTAEv2 [[here](https://arxiv.org/pdf/2202.10108.pdf)]
📖 📖 📖


💬 Dataset Preparation


👉 Data Structure



```yaml
For S1GFloods dataset, clip the images to 256 × 256 patches. Please, respect the following structure: 
├————train/
|      ├———Pre/                                  Images of Time 1 before the flood event
            ├———<region><year><XY>.png
            ...
            ├———<region><year><XY>.png
|      ├———Post/                                 Images of Time 2 after the flood event
            ├———<region><year><XY>.png
            ...
            ├———<region><year><XY>.png            
|      ├———GT/                                   Ground truth labels
            ├———<region><year><XY>.png 
            ...
            ├———<region><year><XY>.png 
|
├————val/
|      ├———Pre/  
            ├———<region><year><XY>.png 
            ...
            ├———<region><year><XY>.png 
|      ├———Post/
            ├———<region><year><XY>.png 
            ...
            ├———<region><year><XY>.png 
|      ├———GT/
            ├———<region><year><XY>.png 
            ...
            ├———<region><year><XY>.png 
|
├————test/
|      ├———Pre/  
            ├———<region><year><XY>.png 
            ...
            ├———<region><year><XY>.png 
|      ├———Post/
            ├———<region><year><XY>.png 
            ...
            ├———<region><year><XY>.png 
|      ├———GT/
            ├———<region><year><XY>.png 
            ...
            ├———<region><year><XY>.png 
```


🚚 Datasets



Contact Information:


If you have any questions or would like to collaborate, please reach out to me at aiboaz1896@gmail.com or feel free to make issues.

License: 


The code and datasets are released for non-commercial and research purposes only. For commercial purposes, please contact the authors.

Acknowledgment:


Appreciate the work from the following repositories:


Planetary Science group at the State key laboratory of information engineering in surveying, mapping and remote sensing of the Wuhan University 

L2HNet

Related resources:


L2HNet dataset


Sentine2-Hub


ESRI 





