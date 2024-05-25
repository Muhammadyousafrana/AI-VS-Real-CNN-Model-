# AI-VS-Real-CNN-Model-
# CNN Model for Image Authenticity Detection

This repository contains a Convolutional Neural Network (CNN) model designed to predict whether a given image is real or fake. The model is deployed and integrated using Streamlit, providing an interactive web application for users to upload images and receive predictions in real-time.

## Table of Contents

- [Overview](#overview)
- [Installation](#installation)
- [Usage](#usage)
- [Model Architecture](#model-architecture)
- [Dataset](#dataset)
- [Training](#training)
- [Deployment](#deployment)
- [Contributing](#contributing)
- [License](#license)

## Overview

With the increasing prevalence of doctored and synthetic images, there is a growing need for automated tools to assess the authenticity of visual content. This project leverages the power of CNNs to classify images as real or fake. The model is deployed via Streamlit, enabling a user-friendly interface for making predictions.

## Installation

To run this project locally, follow these steps:

1. **Clone the repository:**

    ```bash
    git clone https://github.com/Muhammadyousafrana/AI-VS-Real-CNN-Model-.git
    ```

2. **Create and activate a virtual environment:**

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3. **Install the required packages:**

    ```bash
    pip install -r requirements.txt
    ```

## Usage

To use the Streamlit application:

1. **Run the Streamlit app:**

    ```bash
    streamlit run app.py
    ```

2. **Open your web browser** and go to `http://localhost:8501` to interact with the application.

3. **Upload an image** through the provided interface, and the model will predict whether the image is real or fake.

## Model Architecture

The CNN model is built using TensorFlow and Keras. The architecture consists of several convolutional layers followed by max-pooling and fully connected layers. The model is trained to distinguish between real and fake images using a labeled dataset.

## Dataset

The dataset used for training and testing the model consists of labeled images categorized as real or fake. For details on how the dataset is prepared and preprocessed, refer to the `data_preparation.ipynb` notebook in the repository.

## Training

To train the model, follow these steps:

1. **Prepare the dataset** by running the data preparation script:

    ```bash
    python prepare_data.py
    ```

2. **Train the model** by executing the training script:

    ```bash
    python train_model.py
    ```

3. **Evaluate the model** using the evaluation script:

    ```bash
    python evaluate_model.py
    ```

## Deployment

The deployment is handled using Streamlit. The `app.py` script sets up the Streamlit interface and loads the trained model for real-time predictions.

## Contributing

Contributions are welcome! If you have any ideas, suggestions, or bug reports, please open an issue or submit a pull request. For major changes, please discuss them in an issue first to ensure they align with the project goals.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.

---

Feel free to modify this `README.md` to better fit your project's specific details and requirements.