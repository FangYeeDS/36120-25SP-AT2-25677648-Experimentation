# 36120-25SP-AT2-25677648-Experimentation

<a target="_blank" href="https://cookiecutter-data-science.drivendata.org/">
    <img src="https://img.shields.io/badge/CCDS-Project%20template-328F97?logo=cookiecutter" />
</a>

**Project Description:**  
As part of Open Meteo’s AI integration initiative, two machine learning models will be developed to improve weather forecasting for Sydney. The first model is a binary classifier designed to predict whether rain will occur exactly 7 days from a given date. The second model is a regression model aimed at forecasting the cumulative volume of precipitation (in mm) over the next 3 days. Both models will be deployed as APIs on Render to enable easy integration with Open Meteo’s existing services.

## Project Organization


```
├── LICENSE            <- Open-source license if one is chosen
├── Makefile           <- Makefile with convenience commands like `make data` or `make train`
├── README.md          <- The top-level README for developers using this project.
├── data
│   ├── external       <- Data from third party sources.
│   ├── interim        <- Intermediate data that has been transformed.
│   ├── processed      <- The final, canonical data sets for modeling.
│   └── raw            <- The original, immutable data dump.
│
├── docs               <- A default mkdocs project; see www.mkdocs.org for details
│
├── models             <- Trained and serialized models, model predictions, or model summaries
│
├── notebooks          <- Jupyter notebooks. Following naming convention '36120-25SP-<student_id>-AT2-experiment_<number>'
│
├── pyproject.toml     <- Project configuration file with package metadata for 
│                         36120_25sp_at2_25677648_experimentation and configuration for tools like black
│
├── references         <- Data dictionaries, manuals, and all other explanatory materials.
│
├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
│   └── figures        <- Generated graphics and figures to be used in reporting
│
├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
│                         generated with `pip freeze > requirements.txt`
│
├── setup.cfg          <- Configuration file for flake8
│
└── 36120_25sp_at2_25677648_experimentation   <- Source code for use in this project.
    │
    ├── __init__.py             <- Makes 36120_25sp_at2_25677648_experimentation a Python module
    │
    ├── config.py               <- Store useful variables and configuration
    │
    ├── dataset.py              <- Scripts to download or generate data
    │
    ├── features.py             <- Code to create features for modeling
    │
    ├── modeling                
    │   ├── __init__.py 
    │   ├── predict.py          <- Code to run model inference with trained models          
    │   └── train.py            <- Code to train models
    │
    └── plots.py                <- Code to create visualizations
```

## Environment Set Up

### Prerequisites

- Make sure you have **Python 3.12.4** installed.
- Install the **Poetry** package manager. If you don’t have it yet, install it with:

```bash
curl -sSL https://install.python-poetry.org | python3 -
```

### Libraries and Dependencies

This project uses **Python 3.12.4** and manages dependencies via the Poetry package manager. The key packages required are:

- pip
- python-dotenv
- ruff
- pandas (2.2.2)
- scikit-learn (1.5.1)
- ipykernel (>=6.30.0,<7.0.0)
- numpy (>=2.3.2,<3.0.0)
- matplotlib (>=3.10.5,<4.0.0)
- seaborn (>=0.13.2,<0.14.0)
- scipy (>=1.11.0,<2.0.0)
- xgboost (2.1.0)
- my-krml-25677648 (custom package from TestPyPI)

The `pyproject.toml` also configures the supplemental package source **TestPyPI** to install the custom package.

## Running the Project

### Activate the Environment and Run Jupyter Notebooks

1. **Install dependencies**
```bash
poetry install
```

2. **Activate the virtual environment**
```bash
poetry shell
```

3. **Start Jupyter Notebook**
```bash
jupyter notebook
```

4. **Open and run notebooks from the /notebooks directory inside Jupyter**

---

