# 03-mac-install-python-git-vscode.md

This page provides instructions to install or verify Python, Git, and Visual Studio Code on a macOS machine using the Homebrew package manager.

## Steps to Install or Verify

Open a terminal and run the following commands:

```zsh
brew update
brew install python git --cask visual-studio-code
brew install pyenv

python3 --version
pip3 --version
git --version
code --version
pyenv --version
```

## Multiple Versions of Python with pyenv

If you need to add an earlier version of Python (e.g. to use with complex tools such as Kafka or Spark), use pyenv to install additional Python versions like so:

```zsh
pyenv install 3.11.11
```
