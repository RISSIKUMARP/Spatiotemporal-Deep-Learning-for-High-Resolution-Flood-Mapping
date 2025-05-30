# Spatiotemporal-Deep-Learning-for-High-Resolution-Flood-Mapping

# 🌊 Urban Flood Prediction Using Hybrid Deep Learning Models

This repository contains the complete implementation and results for our project on flood prediction using deep learning, using **Houston, Texas** as a case study. We built and compared two hybrid architectures that fuse **temporal rainfall sequences** and **spatial environmental layers** to predict **binary flood masks**.

---

## 📌 Overview

Urban flooding poses significant risks, especially in hurricane-prone areas. Our approach uses a **hybrid deep learning framework** combining:
- **LSTM + DeepLabv3+**
- **GRU + U-Net++**

These models are enhanced by:
- An **attention-based feature fusion** mechanism
- **Bayesian hyperparameter tuning** using Optuna
- **Post-processing** with morphological operations for mask refinement

---

## 🧠 Model Architectures

Each model integrates:
- **Temporal Branch**: LSTM or GRU for 24-hour hourly rainfall sequences
- **Spatial Branch**: CNN encoder from 6 environmental raster layers (e.g., DEM, slope, LULC)
- **Fusion**: Attention-based fusion between temporal and spatial features
- **Decoder**: DeepLabv3+ or U-Net++ for mask generation

---

## 📂 Project Structure

