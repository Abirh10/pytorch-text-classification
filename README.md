# Image Classification

This project implements an image classification system using PyTorch to classify animal faces from the Animal Faces-HQ (AFHQ) dataset. It involves data preprocessing, convolutional neural network (CNN) model training, and performance evaluation using loss and accuracy metrics. The project also visualizes the training progress and allows for making predictions on new images after the model is trained.

## Key Features

*   **Animal Face Classification:** Specifically designed for classifying animal faces (cats, dogs, and wildlife) from the AFHQ dataset.
*   **Convolutional Neural Network (CNN):** Employs a CNN architecture built with PyTorch for feature extraction and classification.
*   **Data Preprocessing:** Includes image resizing, normalization, and conversion to PyTorch tensors.
*   **Training and Validation:**  The dataset is split into training, validation, and testing sets to properly train and evaluate the model's performance. Training progress is monitored and visualized.
*   **Performance Evaluation:**  The model's performance is evaluated using accuracy and loss metrics on both validation and test datasets.
*   **Prediction on New Images:** After training, the model can be used to predict the class of new, unseen animal face images.
*   **Uses GPU if avaliable:** The model training and inference is performed on available GPUs

## Technologies Used

*   Python
*   PyTorch
*   `opendatasets`
*   `torchvision` (transforms)
*   `sklearn` (LabelEncoder)
*   `matplotlib`
*   `PIL (Pillow)`
*   `pandas`
*   `torchsummary`

## Getting Started

1.  **Clone the repository:**
    ```bash
    git clone [repository_url]
    cd [repository_directory]
    ```

2.  **Install the required libraries:**
    ```bash
    pip install -r requirements.txt # Create requirements.txt file if there are any errors
    ```
    Alternatively, install the dependencies individually:
    ```bash
    pip install opendatasets torch torchvision scikit-learn matplotlib pandas torchsummary
    ```

3.  **Download the dataset:**
    The code automatically downloads the AFHQ dataset from Kaggle using `opendatasets`. You may need to provide your Kaggle API credentials.  Ensure you have a Kaggle account and have accepted the competition rules if necessary.

4.  **Run the main script:**
    ```bash
    python main.py # or the appropriate name of your python file
    ```

    This will train the model, evaluate its performance, and generate plots of the training progress.

## Future Enhancements

*   **Implement Data Augmentation:** Integrate more advanced data augmentation techniques (e.g., rotations, flips, zooms) to improve the model's generalization and robustness.
*   **Explore Different CNN Architectures:** Experiment with different pre-trained CNN architectures (e.g., ResNet, VGG) using transfer learning to potentially achieve higher accuracy.
*   **Interactive Prediction Interface:** Build a simple web interface or GUI to allow users to upload images and get real-time predictions from the trained model.

