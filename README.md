# Deep Neural Networks in Diagnosing Pneumonia from Chest X-Ray Images

## Overview
This project investigates the application of deep neural networks in diagnosing pneumonia using chest X-ray images. The study utilizes various deep learning architectures, including DenseNet201, ResNet-18, EfficientNetB0, and a custom CNN model, to classify chest X-ray images into two categories: Normal and Pneumonia.

## Features
- Utilizes multiple deep learning architectures for pneumonia classification.
- Employs data augmentation techniques to improve model accuracy.
- Implements transfer learning with pre-trained models to enhance performance.
- Evaluates models using accuracy, precision, recall, and F1-score.
- Provides insights into the effectiveness of AI in medical diagnostics.

## Dataset
The dataset used in this project is sourced from Kaggle and consists of 5,863 chest X-ray images collected from the Guangzhou Women and Children Medical Center. The dataset is split into three subsets:
- **Training Set**
- **Validation Set**
- **Test Set**
Each subset includes two classes: Normal (0) and Pneumonia (1). Preprocessing techniques such as grayscale conversion, normalization, and augmentation (rotation, zooming, and shifting) were applied to improve model performance.

## Methodology
Four deep learning models were evaluated:
1. **DenseNet201**: Pre-trained model with fine-tuning and data augmentation.
2. **EfficientNetB0**: Optimized for feature extraction and classification.
3. **ResNet-18**: Standardized deep residual network.
4. **Custom CNN**: A convolutional neural network designed specifically for this dataset.

### Preprocessing Steps
- Resized images to 196×196 or 224×224 for consistency.
- Normalized pixel values to [0,1] range.
- Applied data augmentation (rotation, flipping, zooming, shifting) to address class imbalance.
- Utilized early stopping to prevent overfitting.

## Results
- **DenseNet201** achieved **88% accuracy** after fine-tuning.
- **EfficientNetB0** demonstrated the best performance with **95.94% accuracy**, excelling in pneumonia detection with a recall of **0.99**.
- **ResNet-18** struggled with noisy data and had an overall accuracy of **50%**.
- **Custom CNN** achieved **91% accuracy** with robust performance across all evaluation metrics.

## Discussion
- Data augmentation and transfer learning significantly improved model performance.
- EfficientNetB0 emerged as the most reliable model for pneumonia classification.
- Future work should focus on expanding the dataset, handling noisy images more effectively, and integrating explainability techniques such as Grad-CAM for better interpretability.

## Conclusion
Deep learning models, particularly EfficientNetB0 and DenseNet201, show great promise in automating pneumonia diagnosis from chest X-ray images. These models can aid radiologists by improving diagnostic accuracy and reducing workload. Further enhancements in data preprocessing and model optimization will make AI-driven diagnostics more effective and applicable in real-world clinical settings.

## Authors
- Nehal Hamed Alzhrani
- Reham Faisal Alsubhi
- Lamar Waleed Fattah
