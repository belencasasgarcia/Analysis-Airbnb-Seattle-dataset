Airbnb_Seattle_data_analysis
==============================

Analysis of Seattle Airbnb Kaggle dataset

# Airbnb Seattle data analysis

- [Repository Contents](#repository-contents)
- [File descriptions](#file-descriptions)
- [System requirements](#system-requirements)
- [Installation guide](#installation-guide)
- [Demo](#demo)

## Repository Contents:

The files include data and codes to analyse the Seattle Airbnb dataset from Kaggle. These data can be found [here][kaggle airbnb].

The structure of the repository is as follows (note that this corresponds to a cookiecutter strcuture and not all folders/files are applicable):
------------

    ├── LICENSE
    ├── Makefile           <- Makefile with commands like `make data` or `make train`
    ├── README.md          <- The top-level README for developers using this project.
    ├── data
    │   ├── external       <- Data from third party sources.
    │   ├── interim        <- Intermediate data that has been transformed.
    │   └── raw            <- The original, immutable data dump.
    │
    ├── docs               <- A default Sphinx project; see sphinx-doc.org for details
    │
    ├── models             <- Trained and serialized models, model predictions, or model summaries
    │
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures        <- Generated graphics and figures to be used in reporting
    │
    ├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
    │                         generated with `pip freeze > requirements.txt`
    │
    ├── setup.py           <- makes project pip installable (pip install -e .) so src can be imported
    ├── src                <- Source code for use in this project.
    │   ├── __init__.py    <- Makes src a Python module
    │   │
    │   ├── data           <- Scripts to download or generate data
    │   │   └── make_dataset.py
    │   │
    │   ├── features       <- Scripts to turn raw data into features for modeling
    │   │   └── build_features.py
    │   │
    │   ├── models         <- Scripts to train models and then use trained models to make
    │   │   │                 predictions
    │   │   ├── predict_model.py
    │   │   └── train_model.py
    │   │
    │   └── visualization  <- Scripts to create exploratory and results oriented visualizations
    │       └── visualize.py
    │
    └── tox.ini            <- tox file with settings for running tox; see tox.readthedocs.io


--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>

### File descriptions
Input data files can be found in `data/raw` and include the following:

- `calendar.csv` : csv file containing listing id and the price and availability for a given day
- `listings.csv` : csv file containing several properties for each listing, such as price, number of guests, type of property, etc.., and review scores
- `reviews.csv` : csv file containing reviewer id and review comments. This dataset was not used in the analysis

### System requirements
We have tested in Python 3.11.5 and conda 22.9.0 on OSX Big Sur (on MacBook Air with M1 Chip and 16 GB RAM).

### Installation guide
The installation guide below assume that:

1. The repository has been cloned
2. [Anaconda][conda] is installed for package and environment management

Reproduce the environment used for visualizations with the following command:

````
conda env create -f environment/environment.yml
````
This creates a new environment named `udacity_env`. This environment can be activated by executing the following command in the terminal:

````
conda activate udacity_env
````

### Demo
To generate the results and plots, run the `01-data-analysis.ipynb` notebook.

[conda]: https://docs.conda.io/en/latest/
[kaggle airbnb]: https://www.kaggle.com/datasets/airbnb/seattle/data

