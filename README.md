# IDS-706 Week 1: Python Template Project

## Overview

This repository contains a Python template project for **Data Engineering Systems (IDS 706)** Week 1 assignment. The template demonstrates best practices for Python development including virtual environments, testing, linting, formatting, and continuous integration using GitHub Actions.

## Features

- **Python 3.11** environment setup
- **Virtual environment** management
- **Makefile** for automated tasks
- **Unit testing** with pytest
- **Code formatting** with black
- **Code linting** with flake8
- **GitHub Actions** for CI/CD
- **Dev Container** support for GitHub Codespaces
- **Test coverage** reporting

## Project Structure

```
IDS-706-week-1-template/
├── .devcontainer/          # Dev container configuration
├── .github/
│   └── workflows/          # GitHub Actions workflows
├── Makefile               # Automated build tasks
├── hello.py              # Main Python module
├── test_hello.py         # Unit tests
├── requirements.txt      # Python dependencies
└── README.md            # This file
```

## Getting Started

### Option 1: Local Development

1. **Clone the repository:**
   ```bash
   git clone https://github.com/zhongyuan-duke/IDS-706-week-1-template.git
   cd IDS-706-week-1-template
   ```

2. **Set up virtual environment:**
   ```bash
   python3 -m venv ~/.IDS706_python_template
   source ~/.IDS706_python_template/bin/activate
   ```

3. **Install dependencies:**
   ```bash
   make install
   ```

### Option 2: GitHub Codespaces

1. Navigate to the repository on GitHub
2. Click the **Code** button
3. Select **Codespaces** tab
4. Click **Create codespace on main**
5. The environment will be automatically configured

## Usage

The template includes several make commands for common development tasks:

### Available Make Commands

- `make install` - Install and upgrade dependencies
- `make test` - Run unit tests with coverage
- `make format` - Format code using black
- `make lint` - Lint code using flake8
- `make clean` - Remove cache files
- `make all` - Run all commands (install, format, lint, test)

### Example Usage

```bash
# Install dependencies
make install

# Run tests
make test

# Format code
make format

# Check code quality
make lint

# Clean up cache files
make clean
```

## Continuous Integration

The project uses GitHub Actions for automated testing and quality checks. The workflow:

1. **Triggers** on push and pull requests
2. **Sets up** Python 3.11 environment
3. **Installs** dependencies
4. **Runs** linting with flake8
5. **Executes** tests with coverage reporting

## Dependencies

The project uses the following Python packages (defined in `requirements.txt`):

- **pylint** - Code analysis
- **flake8** - Style guide enforcement
- **pytest** - Testing framework
- **click** - Command line interface creation
- **black** - Code formatting
- **pytest-cov** - Coverage reporting

## Development Workflow

1. **Make changes** to your Python code
2. **Format code:** `make format`
3. **Run linting:** `make lint`
4. **Run tests:** `make test`
5. **Commit changes:** `git add . && git commit -m "Your message"`
6. **Push to GitHub:** `git push origin main`
7. **Check Actions** tab for automated testing results


## Course Information

**Course:** Data Engineering Systems (IDS 706)  
**Assignment:** Week 1 Template Setup  
**Institution:** Duke University

---

*This template provides a foundation for Python projects in the Data Engineering Systems course, emphasizing modern development practices and automated workflows.*
