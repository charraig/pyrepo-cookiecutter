# Introduction

A cookiecutter template to generate a simple python package. @dependabot checks the inner template ({{cookiecutter.directory_name}}) dependencies.

* `pyenv` for Python version management
* `poetry` for package management
* [Gitbook](https://www.gitbook.io) for long- and short-form documentation
* VSCode for IDE / text editor
* Python code quality tools:
    * `pytest` for unit tests
    * `black` for auto-formatting
    * `flake8` for linting
    * `isort` for import ordering
 * [pdoc](https://pdoc3.github.io/pdoc/) for documentation

# Basic Usage

Requirements:
* `pipx`: See [pipx](https://pypa.github.io/pipx/)
* `cookiecutter`: `pipx install cookiecutter`
* `poetry`: See [Poetry](https://www.python-poetry.org/docs) documentation

## Create new project

```bash
pipx reinstall-all  # if brew python has been updated or structure pipx as described [here](https://gabnotes.org/how-use-pipx-pyenv/)
poetry self update
cookiecutter gh:charraig/pyrepo-cookiecutter
cd <project_name>
```

## Generate project documentation

`pdoc` will be installed by poetry in the virtual environment upon intialization. Run the following commands in the project virtual environment:

* HTML documentation (the `--force` flag means it will overwrite existing, previously generated html documentation):
```bash
pdoc --html --force --output-dir docs --config latex_math=True <project_name>
```
* Markdown documentation (currently buggy):

```bash
pdoc --output-dir docs --config latex_math=True <project_name>
```
