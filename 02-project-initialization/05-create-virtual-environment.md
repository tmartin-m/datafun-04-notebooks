# 🟠 05-create-virtual-environment.md

This page provides instructions to create a place in your project repository folder that will hold the Python virtual environment for the project. 
It provides an isolated Python environment for the project, so we don't mess up the global Python used by our machine. 

This is typically just done once at the beginning of a project.
If it gets messed up, we can delete .venv and recreate it at any time. 


## Before Starting

Open your project repository in VS Code. 

We'll open a new terminal in VS Code and run a single command to create a new .venv folder for the local project virtual environment.

## Windows Users - Create .venv (Recommended Option A)

Run the following command from the project root directory.
 
On Windows, Use PowerShell (not cmd):

```shell
py -m venv .venv
```

If you see: `Could not find platform independent libraries <prefix>` - it is just a notice and doesn't seem to cause any issues. 

## Mac/Linux Users - Create .venv (Recommended Option A)

Run the following command from the project root directory.

On Mac/Linux, Use zsh or bash:

```shell
python3 -m venv .venv
```

## Accept VS Code Suggestions

If VS Code asks: We noticed a new environment has been created. 
Do you want to select it for the workspace folder?
Click Yes. 

---

<details>
<summary><strong>OPTIONAL/ADVANCED OPTION A (Only if Older Python Version is Needed)</strong></summary>

*Do not continue with this section unless you are using complex tools like Apache Kafka or Apache Spark that may take a while to catch up to the latest version of Python. Know these instructions are here when you need them later.*

Most projects can use the latest Python 3.x, but some tools (like Apache Kafka or Apache Spark) may require an older version.
First, see the machine setup instructions to install additional versions of Python. 
Then, specify the required version when creating the virtual environment. 
For example:

### On Windows, Use PowerShell (NOT cmd)

```powershell
py -3.11 -m venv .venv
```

### On Mac/Linux, Use Default Terminal (e.g., zsh or bash)

```shell
pyenv local 3.11.11
python3 -m venv .venv
```

</details>

---

<details>
<summary><strong>OPTIONAL/ADVANCED OPTION B: Create `.venv` with `uv` (advanced)</strong></summary>

The latest virtual environment manager [`uv`](https://github.com/astral-sh/uv) is fast and works across platforms.

If you've already installed `uv` (see Part 1: Machine Setup), you can create your `.venv` with:

```bash
uv venv
```

This creates the same `.venv` folder, ready for activation and use.

This works on **Windows (PowerShell)**, **macOS**, **Linux**, and **WSL**.

IMPORTANT: Remember to use Option B commands in the Repeatable Workflow as well. 

</details>


---

<details>
<summary><strong>OPTIONAL/ADVANCED OPTION B: Create `.venv` with `uv` (advanced) (Only if Older Python Version is Needed)</strong></summary>

The latest virtual environment manager [`uv`](https://github.com/astral-sh/uv) is fast and works across platforms.

If you've already installed `uv` (see Part 1: Machine Setup), you can create your `.venv` with:

```bash
uv venv
```

This creates the same `.venv` folder, ready for activation and use.

This works on **Windows (PowerShell)**, **macOS**, **Linux**, and **WSL**.

IMPORTANT: Remember to use Option B commands in the Repeatable Workflow as well. 

</details>


---

[🟠 Finished with Part 2: Project Initialization](PROJECT-INITIALIZATION.md)
