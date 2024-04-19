# Comparative Analysis of CNN and Transformer Models for Medical Image Segmentation

This repository contains the research project "Comparative Analysis of CNN and Transformer Models for Medical Image Segmentation," conducted by Taehwan Park, Jiho Shinn, and Seo Won Yi. The project compares the performance of various models on Heart MRI data, including the use of various loss functions and transfer learning strategies.

## Dataset

The dataset used for this project is from the [Medical Segmentation Decathlon](http://medicaldecathlon.com/), which provides a comprehensive collection of medical imaging datasets for benchmarking segmentation algorithms.

## Models

The project evaluates the performance of the following models:

- **U-Net**: A CNN-based model implemented in Tensorflow. The source code can be found [here](https://github.com/shailensobhee/medical-decathlon).

- **FCN**: FCN (Fully Convolutional Network) with ResNet101 backbone and pre-trained weights provided by PyTorch.

- **LRASPP**: A lightweight segmentation model based on MobileNetV3 and provided by PyTorch.

- **MedT**: Medical Transformer model available on [GitHub](https://github.com/jeya-maria-jose/Medical-Transformer).

- **SegFormer**: A Transformer-based model from NVIDIA available on [Hugging Face](https://huggingface.co/nvidia/mit-b2).

- **Swin Transformer**: A vision Transformer model from Microsoft available on [Hugging Face](https://huggingface.co/microsoft/swinv2-large-patch4-window12-192-22k).

## Training Environment

Model training was carried out using Google Colab, utilizing A100, V100, and L4 GPUs for optimal performance.


