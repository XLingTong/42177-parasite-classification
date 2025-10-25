# 42177-parasite-classification
Group project for UTS 42177 Image Processing and Pattern Recognition. Implements medical image classification for parasite detection using microscopy data. Includes shared preprocessing, classical ML (SVM, kNN, trees, boosting, logistic) and deep learning CNN models for robustness evaluation.
# 42177 Image Processing and Pattern Recognition
## Project: Medical Image Classification for Parasite Detection

### Team Members
Ling Tong (CNN)  
Muhib Al Muquit (Logistic Regression)  
Sheikh Wasif (kNN)  
Shuntian Shi (Decision Trees & Random Forests)  
Xinyi Dai (Boosting Methods)  
Zhengjie Chen (SVM)

### Overview
This repository contains all code, manifests, and artifacts for the 42177 group project.
Raw data is **not included**. See below for instructions to obtain and preprocess it.

### Dataset
Microscopic Images of Parasites Species (Mendeley Data v3)  
https://doi.org/10.17632/38jtn4nzs6.3

Place dataset at:  
`/data/raw/MendeleyParasiteDataSet/`  
or update the path in `config.json`.

### Reproducing preprocessing
```bash
python src/preprocess/build_manifest.py
python src/preprocess/preprocess_images.py
python src/preprocess/degrade_sets.py
