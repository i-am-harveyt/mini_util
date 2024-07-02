# mini\_util

## Introduction

This is a simple example that construct a PyPI package with poetry.

## Project Setup

Commands and steps:

```sh
# init project
poetry new <package-name>

cd <package-name>

# you can init your git, and do something with it here

# if ready to release
poetry version  # this will display version
poetry version 0.1.2  # this will set version to 0.1.2
poetry publish --build  # this will publish to pypi and build to `dist/`, you may need to wait around 2 mins to update

# after publish, you may just use pip install <my-package> to install
# or you can also build this using local file
poetry build  # files will store in `dist/`
pip install dist/mini_util-0.1.2-py3-none-any.whl --force-reinstall
# and you can use the cli now
```

## Cli Usage

```sh
mutil -s="Hello World"
# or
mutil --string="Hello World"

```
