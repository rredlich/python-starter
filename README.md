# Python Starter
This is the base code to start a basic project with Pyhton.

## Quick start
```
# Confirm Python version
python --version

# Run code
python main.py
```

## Set up the environment
```
# Create a new virtual environment
python -m venv venv

# Activate a virtual environment
source venv/bin/activate

# To deactivate a virtual environment
deactivate
```

## Run the requirements file
```
# Set up Python environment
pip install -r requirements.txt

# Generate a requirements file
pip freeze > requirements.txt 
```

## Install the dependencies of your package
```
# Perform an editable install
pip install -e .

# Install the extra dependencies
pip install -e .[extra_feature]
```

## Use consistent naming
Try to follow https://pep8.org/ convention, like:
* Using underscores for variables and functions
* Using capital letters for classes
* Using macro case for constants

Here are some examples:
```
import os   # STD lib imports first
import sys  # alphabetical

import some_third_party_lib  # 3rd party stuff next
import some_third_party_other_lib  # alphabetical

import local_stuff  # local stuff last
import more_local_stuff


_a_global_var = 2
_b_global_var = 3

A_CONSTANT = 3.14


# 2 empty lines between top-level funcs + classes
def naming_convention():


class NamingConvention(object):
```

## Check your code for consistency
```
# Install Ruff
pip install ruff

# Run Ruff as a linter
ruff check .                  # Lint all files in the current directory and subdirectories
ruff check path/to/code/*.py  # Lint all `.py` files in `/path/to/code`

# Run Ruff as a formatter
ruff format .                 # Format all files in the current directory and subdirectories
ruff format path/to/code/*.py # Format all `.py` files in `/path/to/code`
```
