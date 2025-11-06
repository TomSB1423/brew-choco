# Fresh Start Kit

For when I need to get a new pc... again

## What's included

This repository contains package management scripts for setting up a PC:

- **Brewfile** - Homebrew packages and casks for macOS
- **choco.ps1** - Chocolatey packages for Windows

## Usage

### macOS (Homebrew)

```bash
# Install Homebrew first if not already installed
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

# Install all packages from Brewfile
brew bundle install
```

### Windows (Chocolatey)

```powershell
# Install Chocolatey first if not already installed
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))

# Run the installation script
.\choco.ps1
```
