# Preparación de Entorno Python
**Cookiecutter Personal**

`preparacion-entorno-python` es un **template de Cookiecutter** que permite crear proyectos Python **estructurados y listos para desarrollo profesional**, incluyendo:

- Entorno virtual gestionado por **uv**.  
- Linting con **Ruff**.  
- Testing con **pytest**.  
- Documentación automática con **Sphinx**.  
- Soporte opcional para **Machine Learning** (`numpy`, `pandas`, `matplotlib`, `opencv-python`).  

Este template es ideal para iniciar proyectos de Python organizados y escalables, con buenas prácticas ya incorporadas.  

---

## Requiremientos

- [git](https://git-scm.com/) >= 2.x
- [Cookiecutter Python package](http://cookiecutter.readthedocs.org/en/latest/installation.html) >= 1.4.0:

``` bash
apt install cookiecutter
wget -qO- https://astral.sh/uv/install.sh | sh
apt install python3-sphinx
```

## Crear un nuevo proyecto

En el directorio en el que quieras guardar tu proyecto generado:

```bash
cookiecutter https://github.com/cacelass/preparacion-entorno-python.git
```
Instalar lo necesario para el proyecto...

```bash
cd <nombre_directorio_creado>
uv sync
uv run pytest
uvx ty check <documento>.py
sphinx-apidoc -o docs/source/ src/.
cd doc/ --> make html
```


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