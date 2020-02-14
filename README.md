# Introduction

A cookiecutter template to generate a simple python package, with the assumptions that the user is using:

* `pyenv` for Python version management
* `poetry` for package management
* (Gitbook)[gitbook.io] for long- and short-form documentation
* VSCode for IDE / text editor
* Python code quality tools:
    * `pytest` for unit tests
    * `black` for auto-formatting
    * `flake8` for linting
    * `isort` for import ordering

# Installation

Requires `cookiecutter`: `pipx install cookiecutter`

`cookiecutter gh:charraig/pyrepo-cookiecutter`