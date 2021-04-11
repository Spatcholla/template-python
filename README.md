# Spatcholla's Python Template

This is a [cookiecutter](https://github.com/audreyr/cookiecutter) template for a typical Python library following modern packaging conventions. It utilizes popular libraries alongside Make and Graphviz to fully automate all development and deployment tasks. Check out the live demo: [Spatcholla/template-python-demo](https://github.com/Spatcholla/template-python-demo)

[![Build Status](https://img.shields.io/travis/com/Spatcholla/template-python.svg)](https://travis-ci.com/Spatcholla/template-python)

## Features

* Preconfigured setup for [Travis CI](https://travis-ci.org/), [Coveralls](https://coveralls.io/), and [Scrutinizer](https://scrutinizer-ci.com/)
* `pyproject.toml` for managing dependencies and package metadata
* `Makefile` for automating common [development tasks](https://github.com/Spatcholla/template-python/blob/main/%7B%7Bcookiecutter.project_name%7D%7D/CONTRIBUTING.md):
    - Installing dependencies with `poetry`
    - Automatic formatting with `isort` and `black`
    - Static analysis with `pylint`
    - Type checking with `mypy`
    - Docstring styling with `pydocstyle`
    - Running tests with `pytest`
    - Building documentation with `mkdocs`
    - Publishing to PyPI using `poetry`
* Tooling to launch an IPython session with automatic reloading enabled
* Visual Studio Code settings for linting and formatting

## Usage

Install `cookiecutter` and generate a project:

```
$ pip install cookiecutter
$ cookiecutter gh:Spatcholla/template-python -f
```

Cookiecutter will ask you for some basic info (your name, project name, python package name, etc.) and generate a base Python project for you.

## Updates

Run the update tool, which is generated inside each project:

```
$ bin/update
```
