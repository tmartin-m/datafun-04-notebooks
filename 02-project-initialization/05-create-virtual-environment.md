# 05-create-virtual-environment.md

This page provides instructions to create a place in your project repository folder that will hold the Python virtual environment for the project. 
It provides an isolated Python environment for the project, so we don't mess up the global Python used by our machine. 

This is typically just done once at the beginning of a project.
If it gets messed up, we can delete .venv and recreate it at any time. 


## Before Starting

Open your project repository in VS Code. 

We'll open a new terminal in VS Code and run a single command to create a new .venv folder for the local project virtual environment.

## Windows Users - Task 1. Create .venv

Run the following command from the project root directory.
 
On Windows, Use PowerShell (not cmd):

```shell
py -m venv .venv
```

## Mac/Linux Users - Task 1. Create .venv

Run the following command from the project root directory.

On Mac/Linux, Use zsh or bash:

```shell
python3 -m venv .venv
```

## Accept VS Code Suggestions

If VS Code asks: We noticed a new environment has been created. 
Do you want to select it for the workspace folder?
Click Yes. 

## ADVANCED OPTION (Only Use When Required)

Python versions matter. In many projects we can use the most recent version of Python 3.
However, using tools like Apache Kafka or Apache Spark
may require an earlier version of Python (it takes a while to get all the code updated).

To use those tools in a project, we may need to install a specific earlier version of Python
 and specify the required version when we create the virtual environment. 
 For example:

On Windows, Use PowerShell (not cmd): `py -3.11 -m venv .venv`

On Mac/Linux, Use zsh or bash: `python3 -3.11 -m venv .venv`
