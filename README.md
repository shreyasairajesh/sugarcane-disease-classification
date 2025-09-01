# Sugarcane Disease Classification (Brown Spot & Rust) using DSANet

This repository showcases our **accepted research paper** on automated sugarcane disease detection, focusing on **Brown Spot** and **Brown Rust** classification using a lightweight deep learning model – **Depthwise Separable Attention Network (DSANet)**.



## Problem
Sugarcane contributes heavily to the agricultural economy, but leaf diseases like **Brown Spot** and **Brown Rust** cause up to **20% yield loss annually**.  
Manual inspection is slow, error-prone, and impractical for large farms. We address this by building an automated, lightweight, and highly accurate classification system.



## Approach
- **Baseline CNN**: Conventional CNN trained on raw + augmented data.  
- **DSANet (Proposed)**: Combines  
  - Depthwise Separable Convolutions (40–60% parameter reduction)  
  - Dual Attention (Channel + Spatial) for disease lesion focus  
  - Ghost Modules for efficient feature extraction  

This makes DSANet both **accurate** and **edge-device deployable**.



## Results
| Model                  | Test Accuracy | Parameters |
|-------------------------|--------------:|-----------:|
| Baseline CNN (no aug)  | 75.3%         | High       |
| Baseline CNN (aug)     | 89.2%         | High       |
| **DSANet (aug)**       | **98.8%**     | Low        |

- Data augmentation improved generalization significantly.  
- DSANet achieved state-of-the-art accuracy while being lightweight enough to run on CPU devices.  



## Dataset
- **Categories**: Healthy, Brown Spot, Brown Rust  
- **Class distribution**: 45% Healthy, 30% Brown Spot, 15% Brown Rust  
- **Preprocessing**: Images resized (224×224), normalized, augmented (rotations, flips, zooms, brightness changes).  
- Dataset not publicly released due to research/IP restrictions.



## Publication
This work has been **accepted to the 17th IEEE International Conference on Computational Intelligence and Communication Networks (CICN 2025), NIT Goa, India (20–21 December 2025).**

**Paper Title:** *Brown Spot and Rust Classification of Sugarcane: Why DSANet with Augmentation Beats Conventional CNNs*  
**Authors:** Sowmyashree Mukunda, Shreya Sai Rajesh, Shruthi M L J  
**Affiliation:** Department of Electronics and Communication, PES University, Bengaluru, India  



## Citation
```bibtex
@inproceedings{rajesh2025dsanet,
  title={Brown Spot and Rust Classification of Sugarcane: Why DSANet with Augmentation Beats Conventional CNNs},
  author={Mukunda, Sowmyashree and Rajesh, Shreya Sai and Shruthi, M L J},
  booktitle={Proceedings of the 17th IEEE International Conference on Computational Intelligence and Communication Networks (CICN)},
  year={2025},
  address={NIT Goa, India},
  month={December 20–21}
}
