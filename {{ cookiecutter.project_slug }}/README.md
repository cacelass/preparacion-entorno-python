
{{ cookiecutter.project_module_name }} de {{ cookiecutter.project_author_name }}

## Descripcion
{{ cookiecutter.project_description }}

## Estructura de directorios y archivos resultantes

    .
    ├── ayuda
    ├── data
    ├── docs
    │   ├── build
    │   ├── make.bat
    │   ├── Makefile
    │   └── source
    │       ├── conf.py
    │       ├── index.rst
    │       └── _static
    ├── pyproject.toml
    ├── README.md
    └── src
        ├── {{ cookiecutter.project_module_name }}
        │   ├── __init__.py
        │   └── main.py
        └── test
            ├── __init__.py
            └── test_proba.py