# 🔵 03-install-dependencies.md

This page explains how to install external dependencies for a Python project.

## Python Standard Library

We do not need to install packages from the Python Standard Library - they are included with our version. The standard library includes helpful packages like pathlib, sqlite3, os, sys, time, and more. See the index.

## External Dependencies

External dependencies are libraries, packages, and modules beyond the standard library and include common packages like pandas, numpy, seaborn, and matplotlib.

These must be installed into our local project virtual environment to use them in our code.

## Before Starting

Open your project repository in VS Code.
Open a terminal.

These commands:

1. Activate the virtual environment (if not already active).
2. Install and upgrade key packaging tools in .venv.
3. Install and upgrade all project and development dependencies.

<details>
<summary><strong>Windows PowerShell (recommended Option A + requirements.txt)</strong></summary>

```powershell
.\.venv\Scripts\activate
py -m pip install --upgrade pip setuptools wheel
py -m pip install --upgrade -r requirements.txt
```

</details>

<details>
<summary><strong>Windows PowerShell (advanced Option B + pyproject.toml)</strong></summary>

```powershell
.\.venv\Scripts\activate
uv pip install --upgrade pip setuptools wheel
uv pip install --upgrade -e .[dev]
```

</details>

<details>
<summary><strong>Mac/Linux/WSL (recommended Option A + requirements.txt)</strong></summary>

```shell
source .venv/bin/activate
python3 -m pip install --upgrade pip setuptools wheel
python3 -m pip install --upgrade -r requirements.txt
```

</details>

<details>
<summary><strong>Mac/Linux/WSL (advanced Option B + pyproject.toml)</strong></summary>

```shell
source .venv/bin/activate
uv pip install --upgrade pip setuptools wheel
uv pip install --upgrade -e .[dev]
```

</details>

---

## Dependencies Evolve Over Time

Which external packages we need tend to evolve over time.
We don't always know the full list when we begin.
For example, it's common to add in matplotlib or seaborn once we have interesting results to visualize.

## Experience

Learn how and when to add external dependencies to `requirements.txt` (or `pyproject.toml`) and repeat this process as needed to make use of the powerful free ecosystem for Python projects.
Explore popular external packages like requests and more to see why they get used.

---

[🔵 Continue with Part 3: Repeatable Workflow](REPEATABLE-WORKFLOW.md)
