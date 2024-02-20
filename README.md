# SegFormer-for-Breast-Cancer-Tumor-Detection

## Members
Anuj Zore (https://www.linkedin.com/in/anuj-zore-806b3112a/)

Ketki Kinkar (https://www.linkedin.com/in/ketkikinkar/)

## Introduction

This repository contains the implementation of the SegFormer model adapted for the purpose of tumor detection in medical images. The SegFormer model, which is a transformer-based approach for semantic segmentation, has been fine-tuned to classify each pixel of an image into two categories: tumor and background. This project aims to contribute to medical imaging analysis by providing an efficient tool for early tumor detection, which is crucial for the timely and effective treatment of cancer.

## Model Overview

SegFormer combines a transformer-based encoder with a simple and efficient MLP decoder, enabling it to efficiently process images and perform segmentation tasks at scale. This model is particularly suited for the detailed and complex task of identifying tumors within medical images, thanks to its ability to capture a wide range of features at different scales.

## Dataset

The model is trained and evaluated on a custom dataset comprising medical images annotated with two classes: tumor and background. These images are pre-processed to fit the input requirements of the SegFormer model and are labeled to accurately represent the presence and location of tumors within the tissues.

## Installation

Follow these steps to set up the environment and run the project:

```bash
git clone https://github.com/<your-username>/segformer-tumor-detection.git
cd segformer-tumor-detection
pip install -r requirements.txt
```

## Tech Stack

This project leverages a comprehensive stack of technologies and libraries designed for high-performance deep learning and efficient image processing. Below are the key components of our tech stack:

### Python

- **Python 3.8+**: The core programming language for model development and data preprocessing.

### Deep Learning Framework

- **PyTorch**: Our primary framework for constructing and training the SegFormer model, chosen for its flexibility and dynamic computation graph.
- **Torchvision**: Utilized alongside PyTorch for image loading, pre-processing, and transformations.
- **mmsegmentation**: A powerful toolset for semantic segmentation, providing an implementation of the SegFormer and other segmentation models.

### Data Processing and Augmentation

- **OpenCV**: For advanced image processing tasks, enhancing the quality of our dataset through various transformations.
- **Albumentations**: A high-performance library for image augmentation, improving model robustness and accuracy.

### Evaluation and Visualization

- **Matplotlib** & **Seaborn**: For plotting training metrics and generating insightful visualizations of our model's performance.
- **TensorBoard**: Integrated for real-time tracking of the training process, including loss and accuracy metrics, and for visualizing model architectures.

### Miscellaneous

- **NumPy**: Essential for numerical computations and image data manipulation.
- **Pandas**: For efficient data analysis and manipulation, particularly useful during the dataset preparation phase.

### Development Tools

- **Git**: For version control, ensuring smooth collaboration and project tracking.
- **GitHub**: Hosts our project repository, facilitating code reviews, issue tracking, and project documentation.

## Reference

@article{segformer,
  title={SegFormer: Simple and Efficient Design for Semantic Segmentation with Transformers},
  author={Xie, Enze and Wang, Wenhai and Yu, Zhiding and Anandkumar, Anima and Alvarez, Jose M. and Luo, Ping},
  journal={NeurIPS},
  year={2021}
}
