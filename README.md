# utils

## Install depdencies
```shell
pip install build
pip install twine
```

## Build Package
Change to the directory that contains the `project.toml` and `setup.cfg` files and then run the `build` package.

```shell
cd cprint
python -m build
```

## Upload to PyPI
Change to the directory that contains the `dist` directory that was created as a result of running `build` and then run `twine`.

```shell
cd cprint
twine upload -u $PYPI_USER -p $PYPI_PASSWORD dist/*
```