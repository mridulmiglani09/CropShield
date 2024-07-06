# Plant-Disease-Classification
Plant Disease Detection using GoogLeNet 

Project Overview

This project aims to develop a robust deep-learning model for detecting plant diseases using image data. Leveraging the power of GoogLeNet architecture, the model can classify images of plants into 38 different categories, including various diseases and healthy conditions.

Dataset

The dataset used for this project is the New Plant Diseases Dataset (Augmented), sourced from Kaggle. It consists of a diverse collection of plant images classified into 38 categories. The data is split into training, validation, and test sets to ensure effective model evaluation.

Data Preprocessing

Data Exploration

Performed an extensive data exploration to understand the distribution of different classes and the overall structure of the dataset. This involved visualizing the distribution of healthy vs. diseased plants and inspecting random samples from each class to gain insights into the variability and characteristics of the images.

Data Augmentation

To enhance the model's ability to generalize, data augmentation techniques such as random rotations, flips, and zooms were applied. This helps in artificially expanding the training dataset and allows the model to learn more robust features.

Model Architecture

GoogLeNet 

The core of our model is based on the GoogLeNet (Inception v1) architecture. This network is renowned for its depth and the use of Inception modules, which allow the network to capture spatial features at different scales. Key components of the architecture include:

Inception Modules: These modules perform convolutions with multiple filter sizes in parallel, capturing various features from the input images.
Auxiliary Classifiers: Two auxiliary classifiers are included to combat the vanishing gradient problem and provide additional regularization during training.
Batch Normalization: Applied to accelerate training and improve model stability.
Training
The model was trained using the Adam optimizer with a categorical cross-entropy loss function. Training was conducted over multiple epochs, with early stopping and learning rate reduction techniques employed to avoid overfitting and enhance convergence.

Evaluation

Performance Metrics

The performance of the model was evaluated using several key metrics:

Accuracy: Overall accuracy across the test set.
Confusion Matrix: Detailed breakdown of true positives, false positives, true negatives, and false negatives.
Precision, Recall, F1-Score: To provide a comprehensive understanding of the model's performance on each class.
ROC-AUC Score: To evaluate the model's capability in distinguishing between the different classes.

Results

The final model achieved an impressive accuracy of 97%, demonstrating high accuracy and robust performance across various plant disease categories. Detailed evaluation metrics and visualizations of the model's predictions can be found in the results section.

Visualization

We included visualizations to illustrate the data distribution and sample predictions from the model. This provides an intuitive understanding of the model's capabilities and the nature of the dataset.

Conclusion

This project showcases the effectiveness of deep learning models, particularly the GoogLeNet architecture, in tackling complex image classification tasks such as plant disease detection. The model's ability to accurately classify a wide range of plant diseases holds significant potential for applications in agriculture, enabling early and precise disease detection to improve crop management and yield.
