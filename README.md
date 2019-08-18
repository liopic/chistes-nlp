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

You may only need to see these two:
* slides/ : slides of the introduction to NLP
* chistes-nlp.ipynb : notebook to be used in the workshop

Other files:
* chistes-nlp-all-executed.ipynb : notebook with all cells executed, in case you can't execute yourself
* data/ : 2k Spanish jokes dataset
* Pipfile, Pipfile.lock, requirements.txt : dependencies' files