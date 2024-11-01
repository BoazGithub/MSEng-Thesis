 # CROSS-PROBABILISTIC WEAK SUPERVISION LEARNING FOR HIGH-RESOLUTION LAND COVER ENHANCEMENT 
This research focused on a weak supervision strategy for deep learning aimed at enhancing high-resolution (sub-meter) land cover from historical pseudo (noise) labels. The study involved developing a deep learning architecture that could be supervised
using unified noise or imbalanced datasets as a reasonable training set during the knowledge acquisition phase. The main concern was how to overcome the barriers of spatial resolution mismatch between pairs of
machine learning to train sets derived from high-resolution images representing complex urban features and rural image features, regardless of photogrammetric and heterogeneity in landforms.
# Dataset



# Requirements 



# C2FNet Architecture
The study introduced the Coarse-to-Fine Network (C2FNet) framework, which incorporates three key components: Edge Resolution Refinement Backbones (ERRB) for stable feature extraction, Unsupervised Dynamic Shuffle and Diagonal Annotation (UDSDA) for confident area selection and probability assignment based close spatial patterns within multiscale features, and a Contrasting Self-Supervised Loss Function (C2F-Loss) utilizing cosine similarity to guide model learning. The contributions of this study can be summarized as: a) improving the accuracy and robustness of land cover mapping, particularly in regions with complex features, achieving an overall accuracy of 80.01% and a kappa coefficient of 0.7567; and b) maximizing the utilization of available data sources for advanced high-resolution land cover mapping. 
![image](https://github.com/user-attachments/assets/3e163c08-adcd-47ed-9384-504fdadf38f7)

# Quantitative Results


# Qualitative Results

🔭 Baseline 

💬 Dataset Preparation


👉 Data Structure

🚚 Datasets



Contact Information
If you have any questions or would like to collaborate, please reach out to me at tamersaleh@whu.edu.cn or feel free to make issues.

License
The code and datasets are released for non-commercial and research purposes only. For commercial purposes, please contact the authors.

Acknowledgment
Appreciate the work from the following repositories:

wenhwu/awesome-remote-sensing-change-detection
SNUNet-CD
BIT-CD
Related resources
ASF-Dataset
Sentinel-Hub
SNAP Toolbox





