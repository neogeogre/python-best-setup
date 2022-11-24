## python-best-setup


### pyenv

install required libraries: https://github.com/pyenv/pyenv/wiki#:~:text=zlib%20tcl%2Dtk-,Ubuntu/Debian/Mint%3A,-sudo%20apt%20update

install `pyenv` : https://github.com/pyenv/pyenv-installer#install

you may need also : 

```shell
sudo apt install python-is-python3
```

then setup python version like the one in the `.python-version` file.

```shell
pyenv install 3.9.15
pyenv local 3.9.15
```

### poetry

install poetry: https://github.com/python-poetry/poetry#installation

then do:

```shell
poetry config virtualenvs.in-project true

```

Now install dependencies with:

```shell
poetry install
```

if everything has been setup properly 

```shell
poetry run python -V
```

should return the version written in the `toml` file and the `.python-version`.

You can also update the dependencies with:

```shell
poetry update
```

Finaly execute your code with:

```shell
poetry run python main.py
```

please check: https://python-poetry.org/docs/basic-usage/
