# toolbag
My scripts and other assorted dev tools

## Conventions

1. Don't use file extensions on scripts in `bin/`. E.g. `foobar` not `foobar.sh` or `foobar.py`. Less typing overrides proper naming in this case.
1. Use `#!/usr/bin/env NAME` as the shebang line. 
1. Shell scripts are written for bash, even though I use zsh as an interactive shell.
1. Python scripts can assume a "recent" version of python3.

## Using

Where `{{PATH_TO_THIS_REPO}}` is the actual absolute path to the directory where you've cloned this repository:

### In `~/.profile` or wherever

```
source "{{PATH_TO_THIS_REPO}}/dotfiles/command_aliases.sh"
export PATH=$PATH:{{PATH_TO_THIS_REPO}}/bin
```

### In `~/.gitconfig`

```
[core]
	excludesfile = {{PATH_TO_THIS_REPO}}/dotfiles/gitignore_global

[include]
	path = {{PATH_TO_THIS_REPO}}/dotfiles/gitconfig
```