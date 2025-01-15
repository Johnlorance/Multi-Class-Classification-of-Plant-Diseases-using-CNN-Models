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
**Model Summary:**
<div style="display: inline-block;">
            Total params: 26,225,126 <br>
            Trainable params: 26,222,630 <br>
            Non-trainable params: 2,496
</div>

## Model B: VGG-16 Fine-Tuned CNN
The second CNN model based on the VGG-16 architecture, a renowned pre-trained model. Convolutional layers will be initialized
with pre-trained weights from the ImageNet dataset. The final layers will be retrained using the plant disease dataset,
adapting the model to the specific classification task with 38 classes.
**Model Summary:**
<div style="display: inline-block;">
    Total params: 14,714,688 <br>  
    Trainable params: 14,714,688 <br>
    Non-trainable params: 0  
</div>

## Dataset:
The dataset consists of labeled images of plants, each associated with one of the 38 disease categories. 
The dataset divided into training, validation, and testing subsets to ensure unbiased model evaluation.
Images sourced from a Git-Hub Repo is forked to my Git-Hub account. 

## Experimental Results

### Model A: Scratch-built CNN

| Number of Epochs | Training Accuracy | Testing Accuracy |
|-------------------|-------------------|------------------|
| 5                 | 83%              | 74.36%          |
| 7                 | 89.7%            | 80.4%           |
| 10                | 91.5%            | 91.06%          |
| 12                | 92.77%           | 91.91%          |
| 15                | 93.80%           | 85.36%          |

**Best Accuracy with 12 epochs:**  
The final model was trained on 12 epochs.

### Model B: VGG-16 Fine-Tuned CNN

| Number of Epochs | Training Accuracy | Testing Accuracy |
|-------------------|-------------------|------------------|
| 5                 | 97.68%           | 97.2%           |

So there is no for more fine-tuning epochs and we stoped in this
