# Satellite-Based Economic Development Mapping with DeepLabV3+: A Case Study of Cairo

![Preview](https://img.shields.io/badge/DeepLearning-EconomicMapping-blue)

This project demonstrates how satellite imagery and deep learning can be combined to predict and visualize economic development in urban areas using Cairo, Egypt as a case study. We trained a DeepLabV3+ model on Landsat composites and VIIRS nighttime light data to generate pixel-level predictions of economic brightness from 2019 to 2025.

## 🌍 Project Overview

- **Region**: Cairo, Egypt
- **Satellite Inputs**: Landsat 8/9 (B1–B7), NDVI, NDWI, NDBI, POI & Road densities
- **Target**: VIIRS nighttime light radiance (µW/cm²/sr)
- **Model**: DeepLabV3+ with ResNet-34 backbone
- **Platform**: Google Colab (PyTorch)
- **Prediction Years**: 2019–2025

## 📦 Contents

| Folder/File | Description |
|-------------|-------------|
| `Final_Notebook.ipynb` | Full training, prediction, and evaluation pipeline |
| `model_weights/` | Trained model weights (`.pth`) |
| `paper/` | Final thesis PDF and visual notebook report |
| `data/LINK.txt` | Link to preprocessed TIFF data on Google Drive |

## 🔧 How to Use

1. Open the notebook in Google Colab
2. Mount Google Drive and link to the `Final Tif Files` folder
3. Run all cells to train or load the model and generate predictions
4. Export predicted maps as GeoTIFF

## 📊 Evaluation (Example: Cairo 2023)

- **MAE**: 8.13
- **RMSE**: 11.31
- **R²**: 0.8207
- Clear visual alignment between predicted and actual brightness

## 📁 Data Access

Raw and processed TIFF files (composites and VIIRS labels) are stored here:
🔗 [Google Drive Folder](https://drive.google.com/drive/folders/1QaxPqOtHD8GjBF7y9XG2YyjYNhcUhI5Z?usp=sharing)

> Folder includes composite rasters for 2019–2025 and ground truth VIIRS maps.

## 📜 Citation

If you use this work, please cite:

**Salma Al Emrany (2025)**  
*Satellite-Based Economic Development Mapping with DeepLabV3+: A Case Study of Cairo*  
Bachelor of Science in Data Science Thesis, The American University in Cairo  
[Download Thesis PDF](./paper/Satellite%20Based%20Economic%20Development%20Mapping%20with%20DeepLabV3%20A%20Case%20Study%20of%20Cairo.pdf)



## 👩‍🏫 Supervisor

This work was supervised by **Dr. Noha Youssef** at AUC, School of Sciences.
