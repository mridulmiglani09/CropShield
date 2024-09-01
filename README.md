# CropShield using GoogLeNet

## Project Overview
This project develops a deep learning model for detecting plant diseases using image data, leveraging the GoogLeNet (Inception v1) architecture to classify images into 38 categories, including various diseases and healthy conditions.

## Dataset
The dataset is the New Plant Diseases Dataset (Augmented) from Kaggle, with images classified into 38 categories. The data is split into training, validation, and test sets for effective model evaluation.

## Data Preprocessing

We visualized class distribution and inspected samples from each class to understand the dataset's structure and variability.
Data augmentation techniques such as rotations, flips, and zooms were applied to enhance the model's generalization capabilities.

## Model Architecture - GoogLeNet 

The model is based on GoogLeNet featuring:

Inception Modules: Parallel convolutions with multiple filter sizes to capture diverse features.
Auxiliary Classifiers: To combat the vanishing gradient problem and provide additional regularization.
Batch Normalization: To accelerate training and improve stability.
Training
The model was trained using the Adam optimizer with a categorical cross-entropy loss function. Techniques like early stopping and learning rate reduction were employed to prevent overfitting and enhance convergence.

## Evaluation
The model's performance was evaluated using:

- **Accuracy**: Achieved an impressive accuracy of 97%.
- **Confusion Matrix**: Detailed breakdown of prediction results.
- **Precision, Recall, F1-Score**: For a comprehensive performance understanding.
- **ROC-AUC Score**: To evaluate class distinction capability.

## Results
The model demonstrated robust performance across various plant disease categories, achieving a 97% accuracy. Detailed evaluation metrics and prediction visualizations are included in the results section.

## Conclusion
This project highlights the effectiveness of deep learning, particularly the GoogLeNet architecture, in complex image classification tasks like plant disease detection. The model's high accuracy holds significant potential for agricultural applications, enabling early and precise disease detection.
