# Dotfiles

This repository contains my personal dotfiles and configuration for a more productive command-line experience. It includes setup instructions for **macOS**, **Ubuntu**, and **Kali Linux**.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Installation](#installation)
  - [macOS](#macos)
  - [Ubuntu](#ubuntu)
  - [Kali Linux](#kali-linux)
- [Configuration](#configuration)
- [Features](#features)
- [Customization](#customization)

## Prerequisites

Before installing the dotfiles, ensure you have the following tools installed:

- **Zsh**: A powerful shell that is an alternative to Bash.
- **Homebrew** (for macOS): A package manager for installing software.
- **APT** (for Ubuntu and Kali): The default package manager.

## Installation

### macOS

1. **Install Homebrew** (if not already installed):
   ```bash
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   ```

2. **Install required packages**:
   ```bash
   brew install kubectx fzf starship sshpass
   ```

### Ubuntu

1. **Update the package list**:
   ```bash
   sudo apt update
   ```

2. **Install required packages**:
   ```bash
   sudo apt install -y kubectx fzf starship sshpass
   ```

### Kali Linux

1. **Update the package list**:
   ```bash
   sudo apt update
   ```

2. **Install required packages**:
   ```bash
   sudo apt install -y kubectx fzf starship sshpass
   ```

### Configuration

After installing the necessary tools, copy the configuration files to their respective locations:

```bash
cp starship.toml ~/.config/starship.toml
cp .zshrc ~/.zshrc
cp .zsh_aliases ~/.zsh_aliases
```

### Additional Configuration

- Ensure that `~/.config/starship.toml` is configured according to your preferences. You can refer to the [Starship documentation](https://starship.rs/config/) for customization options.
- Update your `.zshrc` to include any additional aliases or settings you require.

## Features

- **kubectx**: Easily switch between Kubernetes contexts.
- **fzf**: A powerful command-line fuzzy finder.
- **Starship**: A fast, customizable prompt for any shell.
- **sshpass**: A utility for non-interactive password authentication with SSH.

## Customization

Feel free to customize any of the dotfiles as per your requirements. For example:

- Modify the `.zsh_aliases` file to add your custom aliases.
- Update the `starship.toml` file to change the appearance of your command prompt.

## Contributing

If you have suggestions or improvements for these dotfiles, feel free to submit a pull request!
