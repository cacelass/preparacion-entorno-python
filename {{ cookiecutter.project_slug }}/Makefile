.PHONY: setup test docs lint clean

setup:
	uv sync --extra dev

test:
	uv run pytest

lint:
	uv run ruff check src tests

docs:
	sphinx-apidoc -o docs/source/ src/{{ cookiecutter.project_module_name }}
	cd docs && make html

clean:
	rm -rf .venv .pytest_cache docs/build
