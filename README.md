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
  - In the first experiment, used well known CNN models. In the second experiment, used the most recently developed CNN models.
  - Models experimented(1st): ["resnet18", "inception_v3", "densenet161", "alexnet", "mobilenet_v3_large", "vgg16", "mnasnet1_0"]</br>
  - Models experimented(2nd): ["efficientnet_b5", "convnext_base", "vit_b_16", "mnasnet1_0", "regnet_y_8gf"]</br>
  
## Results
![1stExp](/images/cifar10_study1_plot_slice.png)
In the first experiment with the traditional CNN models,
densenet161 performed the best.

!![2ndExp](/images/cifar10_study2_plot_slice.png)
In the second experiment with the recently developed CNN models,
mnasnet1_0 performed the best.

## Future Improvements
With the best and 2nd best model,
Change CNN structures to get better accuracy
