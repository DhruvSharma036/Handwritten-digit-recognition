# Handwritten Digit Recognition with CNN and Gradio

This project implements a Convolutional Neural Network (CNN) to recognize handwritten digits using the MNIST dataset. The model is integrated with Gradio to provide a user-friendly web interface, allowing users to draw digits and get real-time predictions.

## Key Features

- **Data Loading and Preprocessing**: Efficiently loads and preprocesses the MNIST dataset, normalizing images to the [0, 1] range.
- **CNN Model Architecture**: Utilizes convolutional layers to capture image features and dense layers for classification.
- **Model Training**: Compiled with the Adam optimizer and categorical cross-entropy loss, trained for 10 epochs.
- **Real-time Predictions**: Provides a Gradio interface for drawing digits and displaying predictions.

## How It Works

1. **Data Preparation**: The MNIST dataset is split into training and testing sets, and images are reshaped to include a single channel (grayscale).
2. **CNN Model**: The model includes three Conv2D layers with ReLU activation, max-pooling layers, and dense layers with a softmax activation for classification.
3. **Training**: The model is trained on the MNIST dataset with validation data.
4. **Gradio Interface**: An interactive interface allows users to draw digits, which are then processed and classified by the trained model.

## Usage

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/DhruvSharma036/handwritten-digit-recognition.git
    cd handwritten-digit-recognition
    ```

2. **Install Dependencies**:
    ```bash
    pip install tensorflow gradio numpy
    ```

3. **Run the Script**:
    ```bash
    python digit_recognition.py
    ```

4. **Interact with the Model**:
    Launch the Gradio interface in your web browser, draw a digit (0-9) on the canvas, and click "Submit" to see the model's prediction and confidence score.

## Project Structure

- **`digit_recognition.py`**: Main script containing data loading, model definition, training, and Gradio interface setup.
- **`README.md`**: Provides an overview, installation instructions, and usage guide for the project.

## Future Enhancements

- **Improving Accuracy**: Experimenting with different architectures, hyperparameters, and data augmentation techniques.
- **Expanding Functionality**: Adding more advanced preprocessing steps, or supporting multi-digit recognition.
- **Deployment**: Deploying the model and interface as a web application for broader accessibility.

This project demonstrates the power of CNNs in image recognition and provides an engaging way to interact with machine learning models through a web interface.

