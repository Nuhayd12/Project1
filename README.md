# LSTM-NMT Model

This project implements a neural machine translation model that translates English sentences to Desired language using a sequence-to-sequence architecture with LSTM and attention mechanisms. The model is trained on a dataset containing English-Spanish sentence pairs.

## Table of Contents
- [Installation](#installation)
- [Requirements](#requirements)
- [Usage](#usage)
- [Training](#training)
- [Predicting Translations](#predicting-translations)
- [Contributing](#contributing)
- [License](#license)

## Installation

To set up this project, you need to create a conda virtual environment. Follow these steps:

1. **Install Anaconda**: If you haven't already, download and install Anaconda from [the Anaconda website](https://www.anaconda.com/products/distribution).

2. **Create a new environment**:
   
   ```bash
   conda create --name nmt_env python=3.8
   
3. **Activate the environment**:

  ```bash
  conda activate nmt_env
  ```


**Install the required packages: You can install the required libraries listed below using pip or conda.**

# Requirements

Below are the libraries required to run this project, along with their compatible versions:

Python >= 3.8
Pandas == 1.3.3
NumPy == 1.21.2
Keras == 2.6.0
TensorFlow == 2.6.0
pickleshare >= 0.7.5
You can also create a requirements.txt file by running:

```bash

pip freeze > requirements.txt
```

And install all required packages using pip:

```bash

pip install -r requirements.txt
```

If you prefer to use conda to install the libraries, you can first create a environment.yml file as follows:
```
yaml

name: nmt_env
channels:
  - defaults
dependencies:
  - python=3.8
  - pandas=1.3.3
  - numpy=1.21.2
  - keras=2.6.0
  - tensorflow=2.6.0
  - pickleshare=0.7.5
Then create the environment using:
```

```
bash
conda env create -f environment.yml
```

# Usage
After installing the required libraries, you can start using the translation model.

**Prepare your dataset**: Ensure you have your dataset in the correct format. The dataset should be a tab-separated file containing English sentences in one column and their corresponding Spanish translations in the second. (I have replaced the actual dataset with partial dummy data)

**Clean and preprocess the data**: Run the provided data cleaning script to prepare the dataset for training.

**Train the model**: Use the training script to train the sequence-to-sequence model for translation.

**Predict translations**: Once the model is trained, you can use the prediction script to translate English sentences.

# Training

To train the model, execute the training script:
```
bash

python train_model.py
```

# Predicting Translations

To predict translations using the trained model, run:
```
bash

python predict_translation.py
```

**Provide an English sentence as input when prompted, and the model will output the Spanish translation.**

# Contributing

Contributions are welcome! If you have suggestions for improvements, please create a pull request or open an issue in the repository.

# License

This project is licensed under the MIT License. See the LICENSE file for more details.


### Explanation of the README Sections

1. **Project Title**: Clearly states the purpose of the project.
2. **Installation**: Guides users on setting up a conda virtual environment and activating it.
3. **Requirements**: Lists the necessary libraries with specific versions for compatibility.
4. **Usage**: Provides instructions on how to use the project in stages.
5. **Training**: Instructions for training the model.
6. **Predicting Translations**: How to use the model for translating sentences post-training.
7. **Contributing**: Encourages community involvement.
8. **License**: Specifies the legal use of the project.

# Performance Graph


