# Introduction

A cookiecutter template to generate a simple python package, with the assumptions that the user is using:

* `pyenv` for Python version management
* `poetry` for package management
* [Gitbook](gitbook.io) for long- and short-form documentation
* VSCode for IDE / text editor
* Python code quality tools:
    * `pytest` for unit tests
    * `black` for auto-formatting
    * `flake8` for linting
    * `isort` for import ordering

# Installation

Requirements:
* `cookiecutter`: `pipx install cookiecutter`
* `poetry`: See [Poetry](python-poetry.org/docs) documentation -- use the `curl` method (not pipx), at least until [Issue #1888](https://github.com/python-poetry/poetry/issues/1888) is resolved.

```bash
cookiecutter gh:charraig/pyrepo-cookiecutter
cd <project_name>
poetry install
```