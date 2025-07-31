# Absolute Localization through Vision Transformer Matching of Planetary Surface Perspective Imagery from a Digital Twin

![Summary Figure](docs/summary_fig.png)
*Figure 1: Overview of our absolute localization method using a simulated lunar environment as proxy. (a) Remote sensing data in the form of satellite and elevation maps is gathered, along with (b) rover-view surface images. A digital twin environment is created from the satellite and elevation maps, where (c) twin surface views can be generated through reprojections at known locations. (d) A DINOv2-powered vision transformer image similarity model is used to compare (b) with various candidates of (c). (e) Absolute localization is derived from a map of the closest matching locations.*

---

## Abstract

We present a novel machine learning framework and synthetic dataset for performing absolute localization on planetary surfaces where satellite navigation systems are unavailable. Current approaches involve manual surface-to-satellite image matching by human rover operators, limiting the rate of planetary exploration and scientific utilization. Our framework leverages deep neural networks to perform image similarity matching between a rover’s onboard cameras and corresponding ground-view images from a digital twin environment created from satellite and elevation maps. The rover views, satellite, and elevation maps are taken from a pho- torealistic lunar environment simulated in a 3D graphics engine (Unreal Engine 4). The synthetic ground-view reprojections are generated using an open-source 3D graphics software (Blender). In total, we generate a dataset of 1.68 million images at 210,000 locations. The images and corresponding metadata are then used to train a DINOv2 vision transformer image similarity model through supervised fine-tuning to determine matching locations between the rover views and candidate reprojections. Through this method, our model is able to determine the ground truth location within 5m using just 2.5% of the search space, outperforming other deep learning and classical image comparison benchmarks.

---

## 📂 Overview

Upon publication, this repository will contain a sample dataset, code, and documentation for our paper:

**[Title of Paper]**  
Accepted at [IROS 202X](https://iros.org/)  
[Author 1], [Author 2], [Author 3], ...

Link to preprint: [arXiv/Publisher link if available](#)

---

## 🚀 Getting Started

Clone the repo:

---

## 📊 Data

We provide a **sample dataset** for demonstration and testing.
- Download: [Link to sample/data_sample](data_sample/)
- To access the full dataset upon publication: [DOI/URL placeholder]

See `data_sample/README.md` for details about data format and usage.

---

## 🛠 Usage

Basic usage example:

---

## 💬 Citation

If you use our code or data, please cite:

**BibTeX**
```
@inproceedings{YOUR-KEY,
author = {Author 1 and Author 2 and Author 3},
title = {Title of Your Paper},
booktitle = {Proceedings of the IEEE/RSJ Int. Conf. on Intelligent Robots and Systems (IROS)},
year = {202X},
url = {https://arxiv.org/abs/XXX.XXXXX}
}
```

