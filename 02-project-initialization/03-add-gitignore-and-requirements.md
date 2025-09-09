# 🟠 03-add-gitignore-and-requirements.md

This page provides instructions to add common files to a new project repository.

- `.gitignore` is used to keep things out of GitHub like .venv and secrets
- `requirements.txt` is a good way to list and install external dependencies

## Before Starting

Open your repository in VS Code.

## Task 1. Create `.gitignore`

Create a new file in your root repo folder named exactly: `.gitignore`
IMPORTANT: Spelling, capitalization, and name are critical.
If the name or location is not exact, it will not work.

Find the `.gitignore` file in the root of this [pro-analytics-01](https://github.com/denisecase/pro-analytics-01/) repo and paste the entire contents into your `.gitignore` file.
This is a good starting point for many Python projects.
Actual `.gitignore` contents will vary by project.

## Task 2. Create `requirements.txt`

Create a new file in your root project folder named exactly: `requirements.txt`.
IMPORTANT: Spelling, capitalization, and name are critical. If the name or location is not exact, the commands we provide will not work.

Find the `requirements.txt` file in the root of this [pro-analytics-01](https://github.com/denisecase/pro-analytics-01/) repo and paste the entire contents into your `requirements.txt`file.
This is a good starting point for many Python projects.
Actual `requirements.txt` contents will vary by project.

<details>
<summary><strong>OPTIONAL/ADVANCED: Try <code>pyproject.toml</code> instead of <code>requirements.txt</code></strong></summary>

If you're trying the advanced Option B workflow (`uv` + `pyproject.toml`),  
you can create a `pyproject.toml` file instead of `requirements.txt`.

### Task 2. Advanced Option B: Create `pyproject.toml` instead

Create a file named exactly `pyproject.toml` in your root project folder.

Paste in the following starter content:

```toml
[project]
name = "pro-analytics-01"  # change to your repo name
version = "0.1.0"
description = "Example project using pyproject.toml instead of requirements.txt"
dependencies = [
    # Core package management
    "pip",
    "setuptools",
    "wheel",

    # Logging
    "loguru",

    # Text-to-speech
    "pyttsx3",

    # Jupyter ecosystem
    "ipython",
    "jupyter",
    "ipykernel",
    "ipywidgets",
    "nbdime",
    "jupyterlab-git",

    # Visualization
    "matplotlib",
    "seaborn"
]

[project.optional-dependencies]
# Development-only tools
dev = [
    "ruff",
    "pytest"
]

[build-system]
requires = ["setuptools", "wheel"]
build-backend = "setuptools.build_meta"

[tool.uv]

```

Just like with `requirements.txt`, we adjust the `dependencies` list in `pyproject.toml` to match the external packages needed for the project.

</details>

---

## Experience

**IMPORTANT**: Read through the files - try to understand the purpose of these files.
Know how and why we vary the contents.
Experience comes from working with these files and understanding how to manage them for a project.

---

[🟠 Continue with Part 2: Project Initialization](PROJECT-INITIALIZATION.md)
