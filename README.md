# AI-FashionRecognizer
Deep learning project for classifying clothing images using the Fashion MNIST dataset — built with TensorFlow and fully ready for custom image prediction.

# Fashion MNIST Classifier

This repository contains a simple neural network for classifying images from the **Fashion MNIST** dataset (T-shirt, Trouser, Pullover, Dress, Coat, Sandal, Shirt, Sneaker, Bag, Ankle boot).

The model is implemented using **TensorFlow / Keras** in a Jupyter Notebook.

---

## Project Structure

- `Fashion MNIST Classifier.ipynb`  
  Main Jupyter Notebook containing:
  - Loading the Fashion MNIST dataset from `tf.keras.datasets.fashion_mnist`
  - Visualizing sample images
  - Building and training a fully connected neural network
  - Making predictions on test images and on a custom image (`test.png`)

- `Neural-Networks.png`  
  Visualization of the network architecture generated with `keras_visualizer`.

- `test.png` (optional)  
  Custom image used for prediction. The notebook expects a single-channel (grayscale) image of size **28x28** pixels.

---

## Model Architecture

The neural network is a simple feed-forward model:

```text
Input: 28 x 28 grayscale image
↓ Flatten
Dense(128, activation='relu')
↓
Dense(10, activation='linear' / logits)
