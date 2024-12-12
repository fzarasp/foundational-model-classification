Image Classification using CNN on MNIST and CIFAR-10 Datasets

# Image Classification using CNN on MNIST and CIFAR-10

This project explores image classification using Convolutional Neural Networks (CNNs) on two widely-used datasets: MNIST and CIFAR-10. The project aims to demonstrate the superior performance of CNNs compared to traditional and other deep learning architectures for image-based tasks.

## Table of Contents
1. [Introduction](#introduction)
2. [Datasets](#datasets)
3. [Methodology](#methodology)
4. [Experiments and Results](#experiments-and-results)
5. [References](#references)

## Introduction
Traditional machine learning models struggle with complex, high-dimensional data and often fail to generalize well. CNNs overcome these limitations by automatically extracting hierarchical features from input data, making them ideal for image classification tasks. This project implements a CNN-based approach and compares it against various alternative architectures to highlight its effectiveness.

## Datasets
### MNIST
- **Description**: Grayscale images of handwritten digits (0-9).
- **Size**: 60,000 training images and 10,000 testing images.
- **Resolution**: 28x28 pixels, converted to 32x32 RGB for compatibility.

### CIFAR-10
- **Description**: Color images across 10 classes, including airplanes, cats, and ships.
- **Size**: 50,000 training images and 10,000 testing images.
- **Resolution**: 32x32 pixels with RGB color channels.

## Methodology
1. **Preprocessing**:
   - Normalized pixel values to the range [0, 1].
   - Resized MNIST images to match CIFAR-10 dimensions.

2. **CNN Architecture**:
   - **Input Layer**: Handles 32x32x3 input dimensions.
   - **Convolutional Layers**:
     - Layer 1: 32 filters, 3x3 kernel, ReLU activation, max pooling (2x2).
     - Layer 2: 64 filters, 3x3 kernel, ReLU activation, max pooling (2x2).
   - **Fully Connected Layers**:
     - Dense layer with 64 neurons and ReLU activation.
     - Output layer with 10 neurons and softmax activation.
   - **Optimization**:
     - Optimizer: Adam.
     - Loss Function: Categorical Crossentropy.

## Experiments and Results
### Comparison with CNN-Based Models
Our CNN model significantly outperformed the Shallow CNN and Diluted CNN in training accuracy, validation accuracy, training loss, and validation loss.

### Comparison with Non-CNN Models
Compared to Linear Neural Networks, Fully Connected Networks, Multilayer Perceptrons, LSTMs, and Transformers, our CNN achieved superior performance due to its ability to effectively extract spatial features from image data.

| Model            | Accuracy | Precision | Recall | F1 Score |
|-------------------|----------|-----------|--------|----------|
| Our CNN          | 83.67%   | 84.04%    | 83.67% | 83.74%   |
| Shallow CNN      | 77.36%   | 77.43%    | 77.36% | 77.31%   |
| Diluted CNN      | 75.99%   | 76.87%    | 75.99% | 75.83%   |
| Linear NN        | 70.71%   | 72.06%    | 70.71% | 70.82%   |
| FCNN             | 72.55%   | 72.89%    | 72.55% | 72.44%   |
| MLP              | 71.26%   | 71.69%    | 71.26% | 71.18%   |
| LSTM             | 77.78%   | 77.91%    | 77.78% | 77.73%   |
| Transformer       | 69.27%   | 70.47%    | 69.27% | 69.15%   |

![image](https://github.com/user-attachments/assets/99a9fd4f-48e5-43b2-9e7f-23622f3e1abc)

![image](https://github.com/user-attachments/assets/4832a17a-e63a-4a97-9f25-afd02198b34e)

![image](https://github.com/user-attachments/assets/fef07811-e5a1-4a3f-aeca-12289540012e)

![image](https://github.com/user-attachments/assets/6a974a57-8593-41c9-b169-d2212b712d99)

![image](https://github.com/user-attachments/assets/3472935c-651b-4bf5-88e9-c3049884b64b)
## References
1. Xin, M. & Wang, Y., *Research on image classification model based on deep convolution neural network*. EURASIP Journal on Image and Video Processing, 2019.
2. Chen, L. et al., *Review of image classification algorithms based on convolutional neural networks*. Remote Sensing, 2021.
3. Alzubaidi, L. et al., *Review of deep learning: concepts, CNN architectures, challenges, applications, future directions*. Journal of Big Data, 2021.
4. Bhatt, D. et al., *CNN variants for computer vision: History, architecture, application, challenges and future scope*. Electronics, 2021.

---

Feel free to explore the repository and contribute!



