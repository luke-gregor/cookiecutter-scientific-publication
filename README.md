# Cookiecutter Science Pub

_A logical, reasonably standardized, but flexible project structure for doing and sharing science toward writing a manuscript._


Heavily adapted from the [cookiecutter data science template](https://github.com/drivendata/cookiecutter-data-science). 


### Requirements to use the cookiecutter template:
-----------
 - Python 2.7 or 3.5
 - [Cookiecutter Python package](http://cookiecutter.readthedocs.org/en/latest/installation.html) >= 1.4.0: This can be installed with pip by or conda depending on how you manage your Python packages:

``` bash
$ pip install cookiecutter
```

or

``` bash
$ conda config --add channels conda-forge
$ conda install cookiecutter
```


### To start a new project, run:
------------

    cookiecutter https://github.com/lukegre/cookiecutter-science-pub


### The resulting directory structure
------------

The directory structure of your new project looks like this: 

```

├── LICENSE
├── Makefile           <- Makefile with commands like `make data` or `make train`
├── README.md          <- The top-level README for developers using this project.
├── data
│   ├── analysed       <- Output of scientific ana
│   ├── external       <- Data from third party sources.
│   ├── processed      <- The final, canonical data sets for modeling.
│   └── raw            <- The original, immutable data dump, can also link to server data (e.g. UPdata)
│
├── docs               <- A default `mkdocs` project; run `make website` from the base dir for more info
│
├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
│                         the creator's initials, and a short `-` delimited description, e.g.
│                         `1.0-jqp-initial-data-exploration`. Use git lfs to track these
│
├── references         <- Data dictionaries, manuals, and all other explanatory materials.
│                         Can also be journal articles (use git lfs to store these)
│
├── writing            <- Generated analysis md, PDF, LaTeX, etc.
│   ├── manuscript     <- Can be where you store your LaTeX manuscript and can also be a 
│   │                     subgit directory from Overleaf. First create the document on 
│   │                     overleaf and then clone to ./writing. Rename the folder to whatever 
│   │                     you like. 
│   └── markdown       <- Markdown files that will be used in the creation of docs
│
├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
│                         generated with `pip freeze > requirements.txt`
│
├── setup.py           <- makes project pip installable (pip install -e .) so scripts can be imported
├── scripts            <- Source code for use in this project.
│   ├── __init__.py    <- Makes src a Python module
│   │
│   ├── data           <- Scripts to download or generate data
│   │   ├── download_data.py
│   │   └── make_dataset.py
│   │
│   ├── docs           <- Scripts that are used to create documentation from markdown
│   │   └── sphinx_index.py
│   │
│   ├── analysis       <- Scripts to do your scientific analysis that is not visualization
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

```

## Contributing

We welcome contributions!

### Installing development requirements
------------

    pip install -r requirements.txt

### Running the tests
------------

    py.test tests
