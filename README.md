# Cookiecutter Data Science Template with EDA Example

_A logical, reasonably standardized but flexible project structure for doing and sharing data science work._

This project provides a generic template for data science projects, designed to facilitate organization and scalability. It includes a template of an Exploratory Data Analysis (EDA) notebook named `1.0 EDA.ipynb` in the `notebooks/` directory, offering a starting point for your data exploration and analysis.

**Cookiecutter Data Science (CCDS)** is a tool for setting up a data science project template that incorporates best practices. This template aims to help you kickstart your project with a solid foundation.

> **Note**: This template is based on Cookiecutter Data Science v2. It requires the `cookiecutter-data-science` Python package, which extends the functionality of the [cookiecutter](https://cookiecutter.readthedocs.io/en/stable/README.html) templating utility. Use the provided `ccds` command-line program instead of `cookiecutter`.

## Installation

Cookiecutter Data Science v2 requires Python 3.8 or higher. It's recommended to install it using [pipx](https://pypa.github.io/pipx/):

```bash
# With pipx from PyPI (recommended)
pipx install cookiecutter-data-science

# Alternatively, with pip from PyPI
pip install cookiecutter-data-science
```

## Starting a New Project

To start a new project using this template, run:

```bash
ccds https://github.com/your_username/your_project_template.git
```

Replace `https://github.com/your_username/your_project_template.git` with the URL of this repository.

## Included EDA Template

This template includes an EDA notebook named `1.0 EDA.ipynb` located in the `notebooks/` directory. This notebook serves as a starting point for exploratory data analysis, helping you to:

- Understand the structure and content of your dataset.
- Identify patterns, anomalies, and relationships in the data.
- Prepare the data for modeling.

## Project Structure

The directory structure of your new project will look like this:

```
├── LICENSE            <- Open-source license if one is chosen.
├── Makefile           <- Makefile with commands like `make data` or `make train`.
├── README.md          <- The top-level README for developers using this project.
├── data
│   ├── external       <- Data from third-party sources.
│   ├── interim        <- Intermediate data that has been transformed.
│   ├── processed      <- The final, canonical datasets for modeling.
│   └── raw            <- The original, immutable data dump.
│
├── docs               <- A default mkdocs project; see www.mkdocs.org for details.
│
├── models             <- Trained and serialized models, model predictions, or model summaries.
│
├── notebooks          <- Jupyter notebooks.
│   └── 1.0 EDA.ipynb  <- Template notebook for exploratory data analysis.
│
├── pyproject.toml     <- Project configuration file with package metadata and tool settings.
│
├── references         <- Data dictionaries, manuals, and other explanatory materials.
│
├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
│   └── figures        <- Generated graphics and figures to be used in reporting.
│
├── requirements.txt   <- The requirements file for reproducing the analysis environment.
│
├── setup.cfg          <- Configuration file for tools like flake8.
│
└── src                <- Source code for use in this project.
    ├── __init__.py    <- Makes src a Python module.
    ├── config.py      <- Stores useful variables and configurations.
    ├── dataset.py     <- Scripts to download or generate data.
    ├── features.py    <- Code to create features for modeling.
    ├── modeling
    │   ├── __init__.py
    │   ├── predict.py <- Code to run model inference with trained models.
    │   └── train.py   <- Code to train models.
    └── plots.py       <- Code to create visualizations.
```

## Usage

After generating your project, you can begin working with the EDA notebook:

1. **Navigate to the project directory**:

   ```bash
   cd your_project_name
   ```

2. **Create a virtual environment and activate it**:

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. **Install the dependencies**:

   ```bash
   pip install -r requirements.txt
   ```

4. **Run the EDA notebook**:

   ```bash
   jupyter notebook notebooks/1.0\ EDA.ipynb
   ```

   This will open the EDA template notebook, where you can start exploring your data.

## Contributing

We welcome contributions! If you have suggestions or improvements, please open an issue or submit a pull request.

### Installing Development Requirements

```bash
pip install -r dev-requirements.txt
```

### Running the Tests

```bash
pytest tests
```

## License

This project is distributed under the MIT License. See the [LICENSE](LICENSE) file for more details.
