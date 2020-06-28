# vtools
Bash functions for managing python virtual environments.

## Prerequisite
vtools uses `virtualenv` to create python virtual environment.

## Setup
Add the .bash_vtool file beside your .bashrc file.

Edit .bashrc to load the added file.
```bash
[...]
# vtools additions
if [ -f ~/.bash_vtools ]; then
    . ~/.bash_vtools
fi
```
Edit .bash_vtools to set the 2 variables:
* `VENVSROOTPATH=~/venvs` is the path of the existing folder that will contain your virtual environment. 
* `VENVPYTHON_PATH=/usr/bin/pythonX.X` is the version of python you'll use as interpreter. 
## Commands
* `mkenv [name]`:   create a new environment.
* `listenv`:        Display existing environments.
* `vact [name]`:    Activate environment.
* `rmenv [name]`:   delete an environment.
