# Thesis
## Overview

This thesis presents an automated framework for microstructural characterization of HDPE–HGM syntactic foams using micro-CT (µCT) imaging and machine learning.

Syntactic foams contain both engineered porosity (hollow glass microspheres) and manufacturing-induced defects (voids), which are difficult to distinguish but critically influence mechanical performance. This work develops an end-to-end pipeline to accurately segment, classify, and quantify these features in 3D.

# Tools and Technical Stack Documentation

## 1. Core Programming & Image Processing
- Python (v3.11 recommended)
- opencv-python (OpenCV)
- numpy
- scikit-learn (KMeans clustering)
- scikit-image (region properties, marching cubes)
- scipy (KDTree, stats)
- matplotlib (histograms, rose plots)

## 2. GUI & User Interface
- pillow (PIL)

## 3. 3D Visualization and Mesh Generation
- pyvista (PyVista)

## 4. Imaging Hardware & Software
- Bruker Skyscan 1172 Micro-CT Scanner
- NRecon (1.7.4.6) Reconstruction Software
- ImageJ
- Labkit

## 5. Manufacturing & Mechanical Testing
- Prusa i3 MK3 FFF 3D Printer
- Instron 5980 Series Universal Testing Machine
- Bluehill Universal Software
## Key Contributions

- Developed an **unsupervised segmentation pipeline** combining thresholding and K-means clustering for µCT data
- Achieved **F1-score of 0.92** for void detection compared to manual ground truth
- Classified voids into **manufacturing-induced defects vs. microsphere cavities** using shape descriptors
- Extracted morphological features: **void volume fraction, circularity, aspect ratio, nearest neighbour distance**
- Performed **structure–property correlation** with tensile properties (UTS, Young’s Modulus)
- Built a **custom GUI** for 3D visualization and segmented mesh export (digital twin generation)

## Methods

- Imaging: Micro-Computed Tomography (µCT)
- Techniques: K-means clustering, thresholding, morphological analysis
- Tools: Python, image processing, PyVista (3D visualization)
- Manufacturing: Fused Filament Fabrication (FFF) of HDPE-HGM composites

## Results

- Accurate multi-phase segmentation of **voids, matrix, and microspheres**
- Quantitative identification of **void morphology and spatial distribution**
- Demonstrated strong correlations between **microstructure and mechanical performance**
- Enabled scalable, non-destructive workflow for **quality control and design optimization**

## Repository Structure

- `thesis.pdf` – Full thesis document  
- `figures/` – Key visualizations and segmentation outputs  
- `code/` – Image processing and analysis scripts

## Author

Riya Vasan, Dr. Garrett Melenka, Dr. Reza Rizvi
MASc Mechanical Engineering, York University (2025)
