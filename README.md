#### Project Status: Complete.


# Project Title: Cambridge-Driving Dataset Image Segmentation using DeepLabsV3 Model with Resnet50 Backbone.
## Project Description.
This Image segmentation project is served as an introduction to image segmentation using DeepLabsV3 through PyTorch for me. It was used to prepare for a much advanced project that can be found [here.](https://github.com/) The model trained achieved a Dice score of `0.9515` after just 35 epochs. There were no subsequent post-processing steps involved in this project.

## Notes about the dataset.
The dataset which can be found [here](https://www.kaggle.com/datasets/carlolepelaars/camvid) consists of 32 classes such as cars, animal, building, etc. Pre-processing steps used in this project include;   
* Normalizing: mean = [0.485, 0.456, 0.406], std = [0.229, 0.224, 0.225] (Because of backbone)
* Resizing
* RandomHorizontalFlip (50% probability)
* RandomVerticalFlip (50% probability)

## Other necessary Info.
* Loss Function: Cross Enthropy Loss
* Optimizer: ADAM with learning rate of 0.001

### Tools and Libraries used:
* PyTorch
* NumPy
* PIL
* matplotlib

## Snapshots of Prediction made by model.
![Screenshot (411)](https://github.com/munas-git/CamVid-PyTorch-DeepLabV3-resnet50/assets/78413685/9c6119c1-e2c1-492f-b6ef-a955b8494505)

> Extra Notes   
Potential improvements could be applied to this project such as extra data augmentation, learning rate scheduling, applying post-processing e.g conditional random fields, superpixel segmentation etc. or simply letting the model training run for more epochs.
