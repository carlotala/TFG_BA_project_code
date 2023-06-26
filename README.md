# TFG Business Analytics:

This repository contains the code for the undergraduate thesis project of Carlota López Argote: **Implementation of a warning system for the prevention of car accidents through fatigue detection in drivers**.

### Data:
The data used for this project was a self-made dataset consisting on video recordings of a person driving under 4 different levels of drowsiness: alert, slightly drowsy, moderately drowsy and very drowsy.

### Requirements:
There is a **requirements.txt** file that lists all the dependencies needed to run the project. To install them, run:

```python
pip install -r requirements.txt
```

### Code Structure:
The code is organized into the following Jupyter notebooks:

1. **data_preprocess.ipynb**: This notebook loads and preprocesses the data for use in the classification models. It reads data from the directory `/data` and saves the processed image files in the directory `/data/images/sample` and the table with the extracted features in the directory `/data/features/processed`.
2. **model_workflow.ipynb**: This notebook implements and trains the computer vision model for classification of levels of drowsiness, and provides analysis of the results.

Please run the notebooks in the order specified above.

### Using the trained model:
The trained model is available in the `/models` directory in the form of a .h5 file. To use it for inference, you can load it using the following code snippet in Python:

```python
import tensorflow as tf

# Load the model
model = tf.keras.models.load_model('models/model_16.h5')
```

### Usage:
To use this code, simply clone this repository to your local machine and open the desired Jupyter notebook(s) in a Python environment with the required libraries installed. Follow the instructions in each notebook to load the data, train the model(s), and analyze the results.

Please note that the data must be downloaded and prepared separately before running the code.
