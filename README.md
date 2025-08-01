# Swirl Correction

A specialized image processing system that identifies and corrects swirl distortions in images through deep learning.

## Overview

The Swirl Correction system addresses the problem of moderate swirl effects that can occur at variable centers, radii, and intensities within images . It combines coordinate space manipulations with machine learning to reverse swirl distortions through an interactive research-oriented architecture.

## Features

- **Synthetic Data Generation**: Creates swirl-distorted images for training using `skimage.transform.swirl()` 
- **Deep Learning Pipeline**: TensorFlow/Keras-based model training with data augmentation 
- **Interactive Development**: Jupyter notebook-based implementation for experimentation 
- **Flexible Deployment**: Support for CPU-only and GPU-accelerated processing 
- **Visualization Tools**: Before/after comparison using matplotlib 

## Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/enricoferraiolo/Swirl-Correction.git
   cd Swirl-Correction
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements_gpu.txt  # or requirements_cpu.txt
   ```
   
## System Architecture

The system processes images through several key stages:

1. **Data Loading**: Uses `tf_flowers` dataset or custom `.npy` image files 
2. **Preprocessing**: Resizes images to 128x128 and normalizes pixel values 
3. **Swirl Generation**: Creates synthetic distortions with configurable parameters 
4. **Data Augmentation**: Applies random transformations (flip, rotation, zoom, contrast) 
5. **Model Training**: TensorFlow/Keras pipeline for learning correction mappings 


## Project Structure

```
Swirl-Correction/
├── Swirl_correction.ipynb    # Core implementation
├── requirements.txt          # Base dependencies
├── requirements_cpu.txt      # CPU-only setup
├── requirements_gpu.txt      # GPU-accelerated setup
└── .gitignore               
```

## Usage

The system is designed for interactive research and experimentation . All functionality is contained within the `Swirl_correction.ipynb` notebook, which includes:

- Data preprocessing functions
- Swirl defect generation algorithms  
- Model training infrastructure
- Visualization and comparison tools
