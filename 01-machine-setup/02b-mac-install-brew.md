# 02-mac-install-brew.md

This page provides instructions to install or verify the Homebrew package manager on a macOS machine.

The Homebrew package manager simplifies the installation of software and tools on macOS.


## Steps to Verify Homebrew

Open a terminal and run the following commands:

```zsh
brew update
brew --version
```

## Steps to Install Homebrew

If Homebrew is not already installed, install it, update it, and verify:
```zsh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
brew update
brew --version
```

