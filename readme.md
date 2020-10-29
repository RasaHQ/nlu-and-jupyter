# Evaluating Rasa NLU via Jupyter 

This project was made for Rasa version 2.0.2. 

This repository contains a jupyter notebook as well as a Rasa project. The
goal is to demonstrate that you can use whatever python tools you like to 
analyse the performance of trained NLU models. The notebook shows examples
using [pandas](https://pandas.pydata.org/), [scikit-learn](https://scikit-learn.org/stable/) 
and [altair](https://altair-viz.github.io/).

To get started with the project you'll want to install the requirements
and train a Rasa model. 

```bash
# First install all requirements
python -m pip install --upgrade pip
python -m pip install -r requirements 
# Next we train (just) a NLU model
rasa train nlu 
```

Once you've got a trained model you can select it from the `guide-to-jupyter.ipynb` notebook. 
We advice running the notebook via jupyter lab. 

```bash
python -m jupyter lab 
```

## Important 

The goal of this repository is just to demonstrate the jupyter notebook functionality. 
This project is missing some the Core components and the `config.yml` has a pipeline that
is meant for demonstration purposes only. In particular; the number of epochs is too low. 
The reason we've set it so low is to make the charts look prettier so it should not be seen
as a valid value. We recommend starting with 100 epochs instead. 
