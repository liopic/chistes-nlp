# chistes-nlp

## Introduction
In this workshop **different NLP techniques** are explored to solve a supervised categorization problem: given a collection of Spanish jokes and their tagged categories, use a ML model to predict the category of a new joke.

**This workshop is intended to show** the following:
- Classical and modern NLP techniques.
- Python libraries used to work with natural language.
- The specific problems working with Spanish language.
- The difficulties using a confusing domain: jokes.

This workshop takes part in:
- PyDay BCN 2018, November 24th; Barcelona
- PyConEs 2019, October 4rd-6th; Alicante

## Installation
It is recommended to install the requested libraries before attending the workshop, so you don't need to rely in conference's WiFi. There are 2 recommended ways: using `pipenv` or just using `pip` to install the requirements.

### Using pipenv
Just do the following:
```
pipenv install
pipenv shell
python -m spacy download es
jupyter notebook
```
First command is used to install the dependencies; 2nd, opens a shell in the generated virtual environment; 3rd, downloads Spanish data needed by spacy; 4th, opens jupyter in your navigator.

If there was no problems 🤞, you should see jupyter on your browser: just open chistes-nlp.ipynb file.

### Using pip
You can install the required libraries directly in your computer, using the following commands:
```
pip install -r requirements.txt
python3 -m spacy download es
```
But it should be better to use a virtual environment, like `virtualenv`. Refer to its documentation for more information, or just use pipenv (previous section).

## Contents

* slides/ : slides of the introduction to NLP
* chistes-nlp.ipynb : notebook to be used in the workshop
* data/ : 2k Spanish jokes dataset


# NLP applied to Spanish jokes

In this notebook we will be applying different Natural Language Processing techniques to a corpus of jokes in Spanish.
The **objective** is to **train a Machine Learning model to classify jokes in categories**.

In order to execute smoothly the code, you should've installed the requirements using `pipenv` or `pip` (refer to the README.md for details).

Actually we will be using **pandas** to do a first exploration of the dataset, **spacy (with Spanish package installed)** to extract Natural Language information from the jokes, and **sklearn** to vectorize the jokes and train a Machine Learning model to classify jokes.