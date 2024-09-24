
# Learning in Brain and Machine Exercise: Integration of VGG and ResNet Feature Extraction with SVM for Enhanced Image Classification

This project explores a novel approach to image classification by integrating feature extraction using two powerful convolutional neural network (CNN) architectures, **VGG** and **ResNet**, with a **Support Vector Machine (SVM)** classifier. The goal is to enhance image classification performance by leveraging the complementary strengths of these architectures.

## Project Overview

### Key Objectives:
- Combine the feature extraction capabilities of **VGG** and **ResNet** architectures to capture diverse image features.
- Use **SVM** as the classifier to effectively separate the images into their respective categories.
- Test the framework on a benchmark dataset and compare the results to assess the performance of each model.

## Methods

### 1. VGG Architecture
- **VGG16** and **VGG19** are employed for feature extraction. These architectures use deep convolutional layers with small receptive fields (3x3) and max-pooling layers to capture fine-grained features from the images.
- **Feature Extraction**: After passing the images through the VGG network, the extracted features are used as input to the SVM classifier.

### 2. ResNet Architecture
- **ResNet-101** is used as the second feature extractor. ResNet introduces **residual learning** blocks that help mitigate the vanishing gradient problem in deep networks.
- **Feature Extraction**: Similar to VGG, the output of ResNet is fed into the SVM classifier for final classification.

### 3. Support Vector Machine (SVM)
- **SVM** is employed as the classifier in this system. It works by finding a hyperplane that best separates the data into distinct classes, ensuring maximum margin between the support vectors (data points nearest to the hyperplane).

### 4. Dataset
- **"Cats and Dogs" Dataset**: The model was tested on the popular binary classification dataset, featuring labeled images of cats and dogs. The dataset is curated to provide a straightforward but effective test of classification performance.
  
## Results

| Model            | Accuracy (%) |
|------------------|--------------|
| **VGG + SVM**    | 97.3%        |
| **ResNet + SVM** | 98.9%        |

- **ResNet + SVM** outperformed **VGG + SVM**, demonstrating superior accuracy of **98.9%** on the dataset. The hierarchical feature extraction capabilities of ResNet were advantageous in recognizing intricate patterns in the images.
- Both approaches showed excellent performance, but ResNet’s ability to capture more complex visual structures provided a slight edge in classification accuracy.

### Key Insights:
- ResNet’s residual blocks allowed it to extract more detailed and complex features compared to VGG.
- Combining deep learning feature extraction with a traditional machine learning classifier (SVM) can lead to enhanced classification performance.

## Conclusion

This project highlights the benefits of integrating **deep learning feature extraction** with **traditional machine learning classifiers** like SVM for image classification tasks. The ResNet + SVM combination proved to be more effective in this study, but both architectures achieved high classification accuracy, underscoring the potential of hybrid approaches for improving image classification performance.

