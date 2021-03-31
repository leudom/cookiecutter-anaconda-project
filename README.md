# Cookiecutter for Data Science with Anaconda Project

Adapted project structure for doing and sharing data science work with anaconda-project. The objectiv of this repo is to provide a **lean** and **flexible** project structure to organize your work. Therefore, I removed a whole bunch of artifacts from the original repo (e.g. make files, requirements.txt, etc.) in order to stay lean with dependencies and project structure. This repo is based on 
#### (http://drivendata.github.io/cookiecutter-data-science/)

### Requirements to use the cookiecutter template:
-----------
 - Python 2.7 or 3.5+
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

    cookiecutter https://github.com/leudom/cookiecutter-anaconda-project


[![asciicast](https://asciinema.org/a/v0DEGD0waKMizEKrgRflxV4wj.svg)](https://asciinema.org/a/v0DEGD0waKMizEKrgRflxV4wj)

### The resulting directory structure
------------

The directory structure of your new project looks like this: 

```
├── LICENSE
├── README.md               <- The top-level README for developers using this project.
├── anaconda-project.yml    <- Anaconda project file
├── bin                     <- Trained and serialized models, model predictions, or model summaries.
├── data
│   ├── external            <- Data from third party
│   ├── interim             <- Intermediate data that has been transformed.
│   ├── processed           <- The final, canonical data sets for modeling.
│   └── raw                 <- The original, immutable data dump.
├── notebooks               <- Jupyter notebooks. Naming convention is a number (for ordering),
│                              the creator's initials, and a short `-` delimited description, e.g.
│                              `1.0-jqp-initial-data-exploration`.
├── references              <- Data dictionaries, manuals, and all other explanatory materials.
├── reports                 <- Generated analysis as HTML, PDF, LaTeX, etc.
│   └── figures             <- Generated graphics and figures to be used in reporting
└── src                     <- Source code for use in this project.
    ├── __init__.py         <- Makes src a Python module
    ├── data                <- Scripts to download or generate data
    │   ├── __init__.py     
    │   └── make_dataset.py
    ├── features            <- Scripts to turn raw data into features for modeling
    │   ├── __init__.py
    │   └── build_features.py
    ├── models              <- Scripts to train models and then use trained models to make predictions
    │   ├── __init__.py
    │   ├── predict_model.py
    │   └── train_model.py
    └── visualization       <- Scripts to create exploratory and results oriented visualizations
        ├── __init__.py
        └── visualize.py
```

## Contributing

We welcome contributions!
1. Fork it (<https://github.com/yourname/yourproject/fork>)
2. Create your feature branch (`git checkout -b feature/fooBar`)
3. Commit your changes (`git commit -am 'Add some fooBar'`)
4. Push to the branch (`git push origin feature/fooBar`)
5. Create a new Pull Request

### Installing development requirements
------------

    pip install -r requirements.txt

### Running the tests
------------

    py.test tests
