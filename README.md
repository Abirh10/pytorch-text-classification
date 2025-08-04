# Image Classification

## Project Description

This project implements an image classification model using PyTorch to identify animal faces. It downloads a dataset of animal faces from Kaggle, preprocesses the images, builds a convolutional neural network (CNN), trains the model, and evaluates its performance. The model is trained to classify images into different animal categories. This README provides details on the project's key features, technologies used, setup instructions, and potential future enhancements.

## Key Features

*   **Image Dataset Download:** Automatically downloads the animal faces dataset from Kaggle using the `opendatasets` library.
*   **Data Preprocessing:** Resizes images to a uniform size (128x128), converts them to PyTorch tensors, and normalizes pixel values.
*   **Custom Dataset:** Utilizes a custom `Dataset` class for efficient loading and preprocessing of images.
*   **Data Splitting:** Splits the dataset into training (70%), validation (15%), and testing (15%) sets.
*   **Convolutional Neural Network (CNN):** Implements a CNN architecture with convolutional layers, pooling layers, and ReLU activation functions.
*   **Training and Validation:** Trains the model using the Adam optimizer and CrossEntropyLoss, monitoring training and validation loss and accuracy.
*   **Performance Evaluation:** Evaluates the trained model on the test dataset and reports the final accuracy and loss.
*   **Image Prediction:** Includes a function to predict the class of a single image.
*   **Visualizations:** Plots training and validation loss and accuracy over epochs.

## Technologies Used

*   Python
*   TensorFlow (although the primary framework is PyTorch)
*   PyTorch
*   `opendatasets`
*   `torch`
*   `torch.nn`
*   `torch.optim`
*   `torchvision.transforms`
*   `torch.utils.data`
*   `sklearn.preprocessing`
*   `matplotlib.pyplot`
*   `PIL (Pillow)`
*   `pandas`
*   `torchsummary`

## Getting Started

1.  **Clone the repository:**
    ```bash
    git clone <repository_url>
    cd <repository_directory>
    ```

2.  **Install the required libraries:**
    ```bash
    pip install -r requirements.txt
    ```
    *Note*: A `requirements.txt` file has to be created, containing the dependencies: 
    ```
    opendatasets
    torch
    torchvision
    scikit-learn
    matplotlib
    Pillow
    pandas
    torchsummary
    ```

3.  **Download the dataset:**
    The script downloads the Kaggle dataset directly. Ensure you have a Kaggle API key and it is properly configured.

4.  **Run the main script:**
    ```bash
    python main.py # Or the name of your main script
    ```

## Future Enhancements

*   **Implement Data Augmentation:** Incorporate data augmentation techniques (e.g., random rotations, flips, zooms) to improve model generalization.
*   **Explore Different CNN Architectures:** Experiment with different CNN architectures (e.g., ResNet, DenseNet) to potentially achieve higher accuracy.
*   **Add a User Interface:** Develop a simple web or desktop application to allow users to upload images and get predictions from the trained model.
