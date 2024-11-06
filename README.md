# My dotfiles

This directory contains the dotfiles for my system ([youtube video](https://www.youtube.com/watch?v=y6XCebnB9gs)).

## Requirements

Ensure you have the following installed on your system:

### Git

```
sudo apt install -y git
```

### Stow

```
sudo apt install -y stow
```

## Installation

First, check out the dotfiles repo in your $HOME directory using git

```
git clone git@github.com:dreamsofautonomy/dotfiles.git
cd dotfiles
```

then use GNU stow to create symlinks from `~/*` to `~/dotfiles/*.` Make sure to rename existing config files/directories that
will conflict with the ones in this repo

```
stow .
```

Finally, update the git submodules with

```
git submodule update
```
