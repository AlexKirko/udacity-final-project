# Project

This project is written in support to the article published [here](). It is 
created as a part of the Udacity Data Scientist course, but it can be used as
an example of user identification through session data analysis.

The goal of the project is to differentiate Alice (an attacker) from Bob (all the
other users) by analysing what sites and when she visits. The analysis is performed
The task itself and the data used are taken from this [Kaggle competition](https://www.kaggle.com/c/catch-me-if-you-can-intruder-detection-through-webpage-session-tracking2).
While this is not the final version I used to submit my solution to the competition,
it incorporates the most important tools to be used in user identification. It is
also enough to beat the first baseline: ROC AUC 0.95343.

I hope you find the project and it's accompanying article useful in learning about
bag-of-sites and time series cross-validation. 

# Requirements

1. A full Anaconda installation
2. hyperopt module - install via `pip install hyperopt`

*Important:* at the moment of writing this README, hyperopt has issues with one
of the packages it depends upon. If you see this error:

`model 'bson' has no attribute 'BSON'`

Then you can circumvent the error:


    from hyperopt import base
    base.have_bson = False


When the issue is fixed, this will no longer be necessary.

# Installation and usage

No installation is necessary. Just launch Jupyter Notebook from the root folder.
You can run the explarotory data analysis by running `visual_exploration.ipynb`.
You can run the mechine learning algorithm by running `main.ipynb`.

# License and data permissions

The data for this repo, stored in the `data` folder, is included as per the terms
of the license for [this](https://www.kaggle.com/c/catch-me-if-you-can-intruder-detection-through-webpage-session-tracking2/overview/description) Kaggle competition.
The project itself is licensed under the GNU Public License (included).