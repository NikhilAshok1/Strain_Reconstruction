# Strain Field Reconstruction using PCA and ANN
This repository contains code for reconstructing full-field strain measurements using a minimal set of strain sensors. The workflow combines Principal Component Analysis (PCA) for sensor selection and an Artificial Neural Network (ANN) for predicting strain at unmeasured locations.

## Features
- PCA-based sensor importance ranking
- ANN model for strain field reconstruction
- Visualization of reconstruction error per sensor
- Evaluation metric: Root Mean Squared Error (RMSE) per strain gauge

## Requirements
- Python 3.8+
- PyTorch
- scikit-learn
- pandas, numpy, matplotlib

## How to Use
1. Upload the experimental strain data (e.g., from Excel)
2. Run the notebook to perform PCA and select the most informative sensors
3. Train the ANN model using the selected sensors as inputs
4. Visualize prediction accuracy and evaluate reconstruction error

## Data
The Excel files used for the strain reconstruction experiments are uploaded to the [`Data/`](./Data/) folder. These include raw and processed strain datasets for symmetric and asymmetric bending cases.

## Important Note
This code is designed for strain datasets that follow a structure similar to our experimental setup (e.g., morphing wing data). If you're using a different dataset such as one with different sensor locations, coordinate systems, or loading conditions, you may need to modify the data preprocessing, PCA settings, or model input/output selection accordingly.

## License
MIT License

## Citation
If you use this code, please cite the following paper:  
*“Reconfigurable, Machine Learning-Based Sensor Networks for Real-Time, Adaptive Strain Field Reconstruction of Morphing Wings”, 2025.*
