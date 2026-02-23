# Handwritten Digit Recognition with Keras

This project demonstrates a simple neural network built using Keras for classifying handwritten digits from the MNIST dataset.


## Project Overview

This repository contains a Google Colab notebook that walks through the process of building, training, and evaluating a basic feedforward neural network to recognize handwritten digits. The goal is to classify images of digits (0-9) accurately.

The project utilizes the **MNIST (Modified National Institute of Standards and Technology) dataset**, a large database of handwritten digits that is commonly used for training various image processing systems. It consists of:

- 60,000 training images and labels
- 10,000 testing images and labels

Each image is a 28x28 pixel grayscale image.

The notebook is structured as follows:

   **Import Libraries:** Imports all necessary Python packages.
    
   **Load MNIST Data:** Downloads and loads the MNIST dataset.
    
   **Preprocessing:** Normalizes image pixel values and performs one-hot encoding on labels.
    
   **Build the Neural Network:** Defines the Keras sequential model architecture.
    
   **Compile:** Configures the model for training with an optimizer, loss function, and metrics.
    
   **Train the Model:** Trains the neural network on the training data.
    
   **Evaluation:** Evaluates the model's performance on the test set.
    
   **Make Prediction:** Demonstrates how to make predictions on individual images.
    
   **Visualization:** Includes code to visualize sample images, a confusion matrix, and a classification report.

## Model Architecture

The neural network consists of:

-   An `Input` layer for 28x28 grayscale images.
-   A `Flatten` layer to convert the 2D image data into a 1D vector.
-   A `Dense` hidden layer with 128 units and a 'relu' activation function.
-   A `Dense` output layer with 10 units (for 10 classes) and a 'softmax' activation function.

## Results

After training for 10 epochs, the model typically achieves a test accuracy of around **97% - 98%**.

The notebook includes:
-   Print statements for training and validation accuracy/loss per epoch.
-   An evaluation of the model on the `X_test` dataset, printing the final `Test Accuracy`.
-   A confusion matrix visualization showing the true vs. predicted labels for the test set.
-   A detailed classification report, providing precision, recall, and f1-score for each digit class.

## Contributing

Feel free to fork this repository, make improvements, and submit pull requests. Any contributions are welcome!

## License

This project is open-source and available under the MIT License.
