# MSAC-Net: A Context-Aware Multi-Stream Attentive Convolutional Neural Network for Surface Defect Segmentation

## Overview

**MSAC-Net** is a context-aware encoder-decoder CNN tailored for real-time industrial surface defect segmentation. It addresses the challenges of:
- Varying defect sizes, shapes, and low contrast
- Boundary imprecision and background ambiguity
- Real-time applicability in noisy environments

The architecture integrates:
- 🧠 **Multi-Stream Encoder**: Combines semantic and texture features via EfficientNetV2M and MSCC+SEDNet modules.
- 🎯 **SAEF + ERC**: Spatial attention enhanced fusion and residual convolution for detail preservation.
- 📐 **SS-MLP**: Spatially shifted MLP at the bottleneck for directional context modeling.
- 🧩 **EMSCA + CAG**: Multi-scale context aggregation and cross-attention gate for precise segmentation.

## Datasets

The model is evaluated on four benchmark datasets:
- **DAGM2007**
- **SD900**
- **KolektorSDD2**
- **Magnetic Tile**

All datasets are resized to `256×256` resolution and undergo extensive data augmentation using Albumentations.

## 🛠️ Installation
- git clone https://github.com/rayhan-ahmed91/MSAC-Net.git
- cd MSAC-Net
- pip install -r requirements.txt

## License
This project is released under the CC BY-NC-ND 4.0 License.
