# Before you do anything
type `brew options <what you are doing>`

ie.

`brew options python`

to see what's going on

# Protection
pip list
syspip list
syspip install virtualenv

brew install python


# Make a virtual environment
Use instructions in derek's bash_profile stuff

`virtualEnv -p python py2_sandbox`

# NEVER DO BREW INSTALL in a virtual environment but you must be in one with pip install

# Then do this in your environment:
make a file pip.conf
and put in:
```
[list]
format=columns
```
In [1]: import pandas as pd

In [2]: from pandas_datareader import data, wb

In [3]: import pandas_datareader as pdr
