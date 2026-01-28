
{{ cookiecutter.project_module_name }} de {{ cookiecutter.project_author_name }}

## Descripcion
{{ cookiecutter.project_description }}

## Estructura de directorios y archivos resultantes

    .
    ├── {{ cookiecutter.project_slug }}
    │   ├── ayuda
    │   ├── data
    │   ├── docs
    │   │   ├── build
    │   │   ├── make.bat
    │   │   ├── Makefile
    │   │   └── source
    │   │       ├── conf.py
    │   │       ├── index.rst
    │   │       └── _static
    │   ├── Makefile
    │   ├── pyproject.toml
    │   ├── README.md
    │   ├── src
    │   │   └── {{ cookiecutter.project_module_name }}
    │   │       ├── __init__.py
    │   │       ├── __main__.py
    │   │       └── main.py
    │   └── tests
    │       ├── __init__.py
    │       └── test_proba.py
    ├── cookiecutter.json
    └── README.md