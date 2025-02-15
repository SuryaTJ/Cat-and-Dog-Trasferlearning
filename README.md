<h1 align="left">Dog and Cat Classification using Transfer Learning with MobileNetV2</h1>

###

<p align="left">This repository contains code for a binary image classification task that distinguishes between images of dogs and cats using MobileNetV2 as the base model for transfer learning. MobileNetV2 is a lightweight and efficient convolutional neural network (CNN) architecture, making it ideal for tasks like this where computational resources may be limited.</p>

###

<h2 align="left">Project Overview</h2>

###

<p align="left">The goal of this project is to build a model that can classify images as either "dog" or "cat." We use MobileNetV2, a pre-trained CNN, as the base model and fine-tune it for this specific task. The model is trained on a dataset containing labeled images of dogs and cats.</p>

###

<h2 align="left">Dataset</h2>

###

<p align="left">The dataset used in this project is the Dogs vs. Cats dataset from Kaggle. It contains 25,000 images of dogs and cats, split into training and test sets.<br><br>Training set: 12,500 images of dogs and 12,500 images of cats.<br><br>Test set: 12,500 images (unlabeled).<br><br>You can download the dataset from Kaggle and place it in the data directory.</p>

###

<h2 align="left">Model Architecture</h2>

###

<p align="left">We use MobileNetV2 as the base model for transfer learning. MobileNetV2 is a lightweight and efficient architecture that is pre-trained on the ImageNet dataset. We add a few additional layers to fine-tune the model for the dog vs. cat classification task:<br><br>Base Model: MobileNetV2 with pre-trained weights (excluding the top classification layer).<br><br>Global Average Pooling Layer: To reduce the spatial dimensions of the feature maps.<br><br>Dense Layer: A fully connected layer with ReLU activation.<br><br>Output Layer: A single neuron with sigmoid activation for binary classification (dog or cat).<br><br>The model is compiled using the Adam optimizer and binary cross-entropy loss.</p>

###

<h2 align="left">Results</h2>

###

<p align="left">After training, the model achieves the following performance:<br><br>Training Accuracy: 96%<br><br>Training Loss: 0.1<br><br>Test Accuracy: 90%<br><br>Test Loss: 0.72<br><br>These results indicate that the model performs well on both the training and test datasets, demonstrating its ability to generalize to unseen data</p>

###
