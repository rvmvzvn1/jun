### Results 
<img width="1880" height="447" alt="image" src="https://github.com/user-attachments/assets/7ee1b3e6-002c-44d1-b908-6e74aed14d0e" />
## Google Earth Ore Detection Project

# Ore Zone Detection from Google Earth Images

This project uses a trained U-Net++ deep learning model to detect possible ore zones from Google Earth satellite images.

## Project Overview
The project loads satellite images from Google Drive, preprocesses them into 17 input channels, and applies a trained semantic segmentation model to predict potential ore zones.

The model generates probability maps, binary prediction masks, and visual markers showing detected areas on the original image.

## Technologies
- Python
- PyTorch
- segmentation_models_pytorch
- U-Net++
- EfficientNet-B3
- OpenCV
- NumPy
- Pandas
- Matplotlib
- Google Colab
- Google Drive

## Model
- Architecture: U-Net++
- Encoder: EfficientNet-B3
- Input channels: 17
- Output classes: 1
- Task: Binary semantic segmentation
- Threshold: 0.30

## Features
- Google Earth image processing
- Custom 17-channel feature generation
- Deep learning inference
- Probability map visualization
- Binary mask prediction
- Detected zone visualization
- Result table generation
- CSV export

## Results
- Probability maps for each image
- Predicted binary masks
- Detected ore zone markers
- Confidence score for each image
- Final results table saved as CSV

## Files
- `google_earth.ipynb` — Google Earth image inference and ore zone detection notebook

## Example Results
Add screenshots of:
- Original Google Earth image
- Probability map
- Predicted mask
- Detected zones
- Final results table

## How to Run
jupyter notebook
pip install segmentation-models-pytorch opencv-python matplotlib pandas
