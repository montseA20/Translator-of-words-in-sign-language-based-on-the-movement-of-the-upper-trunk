Sign Language Recognition System
This project implements a sign language recognition system that translates hand gestures from videos into text. It utilizes Mediapipe for hand keypoint detection and an Artificial Neural Network (ANN) for classification.

This project requires Python 3.8 or higher.

Ensure the training.json file contains the correct mapping between video IDs and corresponding glosses (words).

This script trains the model using the data in dataset.json and saves the trained model as model2.pth. It also displays training progress, including loss and evaluation metrics, and generates plots for visualization.

Inference: (Currently integrated with training) The main.py script currently performs inference on the training data after each training epoch.

Model
The model used is an Artificial Neural Network (ANN) implemented with PyTorch.
It consists of linear layers, ReLU activation functions, and Dropout layers for regularization.
The model takes a sequence of 30 frames, each containing 42 hand keypoints (21 per hand), as input.
The output is a probability distribution over the set of possible sign language glosses (words).
Pending
🟨 Try other model architectures (CNN etc.): Explore more advanced model architectures, such as Convolutional Neural Networks (CNNs), to potentially improve accuracy and capture spatial relationships in the hand gesture data.
🟨 LIVE parsing of frames for live translation: Implement real-time processing of video frames to enable live translation of sign language gestures. This would involve capturing video input, extracting hand keypoints, and feeding them to the trained model for prediction.
🟨 Setup infer pipeline: Develop a dedicated inference pipeline for efficient and streamlined prediction using the trained model. This could involve optimizing the model for inference, creating an API for accessing the model, and building a user interface for real-time translation or interaction.



Fuentes y contenido relacionado
