# 03-windows-install-python-git-vscode.md

This page provides instructions to install or verify Python, Git, and Visual Studio Code on a Windows machine using the Winget package manager.

## Steps to Install or Verify

Open a PowerShell terminal and run the following commands:

```powershell
winget install --id Python.Python.3
winget install --id Git.Git
winget install --id Microsoft.VisualStudioCode
python --version
pip --version
git --version
code --version
```