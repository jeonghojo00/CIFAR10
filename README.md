# CIFAR10
CIFAR10 image classification

## Objective
Compare pre-defined CNN models for Image classification on CIFAR-10 dataset
Develop the the CNN model with the best accuracy and compare it with Transfer learning with various state-of-art CNN models

## Requirements
- Python 3
- torch(1.11.0+cu113) , torchvision(0.12.0+cu113) (For models and data import)
- optuna (for Experiment)

## Methodology
1. Download/Load CIFAR10 images with different size images by models due to lack of memory capacity in Colab pro
2. Use optuna to experiment each model with loaded CIFAR10 images </br>
  2_0. In the first experiment, used well known CNN models. In the second experiment, used the most recent CNN models with a model of the best accuracy in the first experiment </br>
  2_1. Models experimented(1st): ["resnet18", "inception_v3", "densenet161", "alexnet", "mobilenet_v3_large", "vgg16", "mnasnet1_0"]</br>
  2_2. Models experimented(2nd): ["efficientnet_b5", "convnext_base", "vit_b_16", "mnasnet1_0", "regnet_y_8gf"]</br>
  
## Results


## How to train and test(predict)

## Future Improvements
