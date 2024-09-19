# Data Preparation
The data is organized into separate folders for training, validation, and testing. The following steps were taken to load and preprocess the data:

- Load images from the specified directory structure.
- Convert the labels into one-hot encoded vectors.
- Normalize image pixel values to a range of [0, 1].

# Model Architecture
Two models were built for comparison:

## CNN Model
- A custom CNN architecture with multiple convolutional and pooling layers.
- Dense layers followed by dropout for regularization.

## MobileNetV2 Model
- A pre-trained MobileNetV2 model with a custom classification head added.

# Training
Both models were trained using early stopping to prevent overfitting. The models were saved after training for future inference.

# Evaluation
The models were evaluated on a test set, and their accuracies were reported. Additionally, confusion matrices were generated for a visual representation of the classification performance.

# Example Predictions
You can make predictions on a sample image using the provided `readable_prediction` function, which displays the predicted class and confidence level for the given image.

# Results
- CNN Model Accuracy on Test Set: **95.65%**
- MobileNetV2 Model Accuracy on Test Set: **94.79%**
