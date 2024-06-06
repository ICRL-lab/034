# Plant Disease Classification
<p align="center">
  <img src="pic.jpg" alt="Plant Disease Classification" width="200" height="200">
</p>

## Introduction:
It’s a plant disease classification in which we use different models and calculate their results on the same dataset. We used the ANN, CNN, and Transfer Learning using MobileNet.

## Dataset:
It’s a dataset of images with train and test folders in it, containing four classes (Common_rust, Blight, Grey-leaf-spot, Healthy). There are about 840 images in each train and test folder.

### Some information about the dataset is given below:
- **Name:** Plant disease
- **Mode:** Image Data
- **Number of Samples:** 840
- **Type:** Classification
- **Modality:** Color images
- **Number of Classes:** 4
- **Classes Names:** Common-rust, Blight, Grey-leaf-spot, Healthy

## Preprocessing:
There are some following preprocessing techniques used in this code:
- Rescaling
- Shear Range
- Zoom Range
- Horizontal Flip

## Models:
1. CNN (Convolutional Neural Network) Model
2. ANN (Artificial Neural Network) Model
3. Transfer Learning Using MobileNet

## RESULTS


| Model       | Architecture | Preprocessing Steps   | Optimizer | Learning Rate | Epochs | Test Accuracy | Notes                                      |
|-------------|--------------|-----------------------|-----------|---------------|--------|---------------|--------------------------------------------|
| CNN         | Conv2D + Dense Layers | Rescaling, Shear Range, Zoom Range, Horizontal Flip | Adam      | 0.001         | 25     | 0.8765 | Custom CNN model with data augmentation   |
| ANN         | Dense Layers  | Rescaling              | Adam      | 0.001         | 25     | 0.5563  | Simple ANN model with flattened inputs      |
| MobileNet   | Pre-trained MobileNet + Custom Dense Layers | Rescaling, Shear Range, Zoom Range, Horizontal Flip | Adam      | 0.001         | 25     | 0.9286  | Transfer learning using pre-trained MobileNet |
