# PDM manual for tin200

This repository is based upon work done by Othelie Eliassen, Marius Vinorum, and
Aleksander Bo Tunheim from NMBU.

## Introduction

The source code uses the [scikit](https://scikit-learn.org/stable/),
[numpy](https://numpy.org/),
[pandas](https://pandas.pydata.org/), and
[tensorflow](https://tensorflow.org) libraries.

First, we read the data in the data repository with pandas. Then, the code is
processed with scikit and numpy, before it is used by Tensorflow. The tensorflow
library will use the processed data and train a machine learning model with the data.

## Getting started

To get started, make sure you have python 3 installed.
Install the required packaged either with conda, or with pip.

### Setup with Conda

Run the command:

```bash
conda env create -f environment.yml
```

### Setup with pip

Run the command:

```bash
python3 -m pip install -r requirements.txt
```

## Running the code

Enter the folder where you have downloaded the code, and open a terminal in the current folder. For a guide, take a look at the following guide: https://www.groovypost.com/howto/open-command-window-terminal-window-specific-folder-windows-mac-linux/

NOTE: In Windows, you might have to use the anaconda prompt instead of the
command prompt or powershell.

To run the streamlit version of the app, run the command:

If you used conda, you need to enter your environment by doing the following:

```bash
conda activate pdm-env
```

Now, we have to do multiple steps:

1. We have to first run the `Particle1.py` script to read the data, sort it and then normalize the data
2. Then we run the `Particle2.py` script to build our neural network, and train it.
3. Finally, to train our model, we run the `particle3.py` script to evaluate our model.

All scripts can be ran with the following code in your terminal:

```bash
python ./code/<Script name>.py
```
