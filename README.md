# Traffic Sign Recognition using TensorFlow

## Overview

The Traffic Sign Recognition project aims to develop a neural network model using TensorFlow to classify road signs based on input images. With the advancement of self-driving cars, computer vision plays a crucial role in enabling vehicles to understand their environment, including recognizing and distinguishing various road signs such as stop signs, speed limit signs, yield signs, and more.

## Dataset

For this project, we utilize the German Traffic Sign Recognition Benchmark (GTSRB) dataset. This dataset consists of thousands of images depicting 43 different kinds of road signs, each labeled with the corresponding sign category.

## Neural Network Model

The neural network model is built using TensorFlow, a popular deep learning framework. The model architecture typically involves convolutional neural networks (CNNs) to effectively extract features from input images and classify them into different road sign categories.

## Project Workflow

1. **Data Preparation:** Preprocess the GTSRB dataset, including image resizing, normalization, and splitting into training and testing sets.
2. **Model Development:** Design and train the neural network model using TensorFlow, experimenting with different architectures, hyperparameters, and optimization techniques.
3. **Model Evaluation:** Evaluate the trained model's performance on the testing dataset, measuring metrics such as accuracy, precision, recall, and F1-score.
4. **Model Deployment:** Deploy the trained model for real-time road sign recognition, potentially integrating it with self-driving car systems or traffic management applications.

## Future Enhancements

- Explore advanced techniques such as transfer learning and fine-tuning pretrained models to improve classification accuracy.
- Extend the model to recognize additional types of road signs or adapt it for specific use cases or environments.
- Enhance the model's robustness to variations in lighting conditions, weather, and camera perspectives.


I conducted a comparison between two neural networks that are identical except for the presence of a convolutional layer. In the model containing the convolutional layer, we achieved an accuracy of 0.9687 after 10 epochs. Conversely, the model without the convolutional layer only reached an accuracy of 0.0581 in the same timeframe. This discrepancy is logical because convolutional layers are specifically designed to extract intricate features and analyze spatial patterns, making them particularly effective for tasks involving the recognition of complex shapes in traffic-related data.

Additionally, elevating the number of filters in the convolutional layer from 32 to 40 resulted in enhanced accuracy for both the training and testing datasets.(for example in testing data : accuracy = 0.9245 improving to -> 0.9329 ) This improvement is coherent since increasing the number of filters allows the neural network to learn a broader range of features, thereby enhancing its ability to understand and represent the underlying patterns in the data .
Raising the number of filters from 40 to 70 resulted in a decrease in accuracy for the testing data, dropping from 0.9329 to 0.9298. This decline can be attributed to overfitting, where the model becomes too tailored to the training data, making it less adept at generalizing to new, unseen data.










