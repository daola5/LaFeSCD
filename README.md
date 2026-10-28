# LaFeSCD
This repository provides the code for the method in our paper 'LaFeSCD: Joint Learning of Language Priors and Frequency-Aware Representations for Semantic Change Detection in Remote Sensing Images'.

## Overview
<img width="1476" height="744" alt="image" src="https://github.com/user-attachments/assets/d8984502-34f5-4582-b95f-8708ab21f942" />

LaFeSCD is a multi-domain joint learning of language, frequency, and spatial for semantic change detection. It works through three modules:
- **LPR** (Language Priors Representation)
- **LPTFA** (Language Priors and Temporal Feature Alignment)
- **AFDL** (Adaptive Frequency Domain Learning)

## Requirements

- Python 3
- PyTorch
- torchvision
- numpy
- scipy
- scikit-image
- opencv-python
- matplotlib
- tensorboardX
- timm
- einops

The model was trained on an NVIDIA A100 GPU.

## Pretrained Models

Download the [RemoteCLIP ViT-B/32 checkpoint](https://huggingface.co/chendelong/RemoteCLIP/blob/main/RemoteCLIP-ViT-B-32.pt) before training.

## Datasets
- **SECOND**
- **Landsat-SCD**

## Training
```bash
# Train on SECOND dataset
python train_SECOND.py

# Train on Landsat-SCD dataset
python train_Landsat.py
```

## Inference

```bash
python pred_SCD.py
```
