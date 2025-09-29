# python_code_reference

A Python project for code reference and examples.

## Project Setup

This project uses `uv` as the package manager and Python version manager. Follow these steps to set up the development environment:

### Python Version Management

```bash
# Install specific Python version (if not already installed)
uv python install 3.12.7

# Create virtual environment with specific Python version and name
uv venv --python 3.12.7 python_code_reference

# Initialize project with specific Python version
uv init --python 3.12.7
```

### Package Management

```bash
# Add packages to the active virtual environment
uv add <package_name> --active

# Add development packages
uv add --dev pytest ruff
```

### Dependencies

Current project dependencies are managed through `pyproject.toml` and locked in `uv.lock`.

To install all dependencies:
```bash
uv sync
```

### Running the Project

```bash
python main.py
```