# makemore-3

# Name Generator Neural Network
This repository contains a character-level neural network built from scratch using PyTorch. The model is designed to generate realistic names by learning patterns in a dataset of names. The project focuses on implementing core neural network components and training workflows without relying on pretrained models.

Features
Custom implementation of layers, including BatchNorm and embeddings.
Contextual windowing to capture character dependencies.
Designed for fundamental understanding of neural networks.
Trains on a dataset of names to generate realistic outputs.
Requirements
Python 3.7+
PyTorch 1.13+
NumPy
Install the required packages via pip:

bash
Copy code
pip install torch numpy  
Dataset
The project uses a dataset of names (e.g., names.txt) as input for training. Ensure that each name is on a new line in the file.

Usage
Clone the repository:

bash
Copy code
git clone https://github.com/yourusername/name-generator-nn.git  
cd name-generator-nn  
Place your dataset in the project directory (e.g., names.txt).

Train the model:

bash
Copy code
python train.py  
Generate names after training:

bash
Copy code
python generate.py  
How It Works
Training: The model learns character patterns using embeddings and contextual windows. Batch normalization is used to stabilize training.
Generation: Starts with a context of empty characters, predicting the next character until a termination condition (e.g., .) is met.
Customizations
Modify the hyperparameters (e.g., learning rate, context size, batch size) in the configuration section of train.py.
Update the dataset with your own names or text data.
Example Outputs
After training on a dataset, the model generates names like:

Alvara
Marianella
Benedictus
Learning Focus
This project emphasizes building from scratch to deepen understanding of:

Embedding layers and how they encode categorical data.
Batch normalization and its role in training stability.
Character-level modeling and sequence generation.
