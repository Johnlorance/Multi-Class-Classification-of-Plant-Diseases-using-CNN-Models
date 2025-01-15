# Multi-Class-Classification-of-Plant-Diseases-using-CNN-Models
## 🌟 Overview
This project aims to create and compare two distinct CNN models for classifying
plant images across 38 disease categories. These models trained to
categorize images based on diseases for each class.

## Model A: Scratch-built CNN
One CNN model designed and trained from scratch. This model comprise multiple convolutional layers, pooling layers, 
and fully connected layers. It will learn to extract relevant features directly from the plant images and 
serve as a baseline for performance comparison.
This architecture is designed to handle the complexities of classifying plant diseases within 
the provided image dataset.
            Model Parameters:
            Total params: 26,225,126
            Trainable params: 26,222,630
            Non-trainable params: 2,496

## Model B: VGG-16 Fine-Tuned CNN
The second CNN model based on the VGG-16 architecture, a renowned pre-trained model. Convolutional layers will be initialized
with pre-trained weights from the ImageNet dataset. The final layers will be retrained using the plant disease dataset,
adapting the model to the specific classification task with 38 classes.

## Dataset:
The dataset consists of labeled images of plants, each associated with one of the 38 disease categories. 
The dataset divided into training, validation, and testing subsets to ensure unbiased model evaluation.
Images sourced from a Git-Hub Repo is forked to my Git-Hub account. 
