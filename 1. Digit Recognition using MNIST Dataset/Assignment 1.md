# MNIST CNN Project: Output Summary & README

This project implements a Convolutional Neural Network (CNN) to classify handwritten digits from the MNIST dataset. This document outlines the key visualizations and outputs generated during the evaluation phase of the model.

## 1. Key Visualizations

### Model Loss Development
<img width="855" height="547" alt="Traning Loss" src="https://github.com/user-attachments/assets/91ad3b99-678b-457b-85bf-81a71d531594" />

* **Description:** This plot tracks the **Training Loss vs. Validation Loss** over 20 epochs.
* **Purpose:** It is used to monitor how well the model is learning (convergence) and to identify if the model is beginning to overfit the training data (where training loss continues to drop while validation loss rises).

### Confusion Matrix
<img width="797" height="701" alt="Confusion Matrix" src="https://github.com/user-attachments/assets/0d6810af-2eff-4202-ae4a-513d5a2ca15f" />

* **Description:** A heatmap visualization generated using `seaborn` and `sklearn.metrics`.
* **Purpose:** It provides a detailed breakdown of classification accuracy per digit. It highlights specific "confusions"—for instance, showing if the model frequently mistakes the digit **4** for a **9** or a **7** for a **1**.

### 10x10 Prediction Grid
<img width="1955" height="1990" alt="Predictions" src="https://github.com/user-attachments/assets/0967e4fb-601b-4ad6-bc99-ec1daeafc8b4" />

* **Description:** A grid displaying the first 100 images from the test set alongside their predicted labels.
* **Color Coding:**
    * **<span style="color:blue">Blue Labels</span>**: Correct predictions.
    * **<span style="color:red">Red Labels</span>**: Incorrect predictions (formatted as `Predicted label (True label)`).
* **Purpose:** To provide a visual qualitative assessment of the model's performance on individual samples.

## 2. Model Export

The final trained state of the network is exported for deployment, further testing, or future inference.

* **Filename:** `mnist_cnn_model.keras`
* **Format:** Keras HDF5/Native format
