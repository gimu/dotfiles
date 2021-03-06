dotfiles
========

The old configuration can be found [here](https://github.com/gimu/dotfiles-legacy).                                               
This repository is aimed to work on Arch Linux (with a few tweaks probably on another distribution too).

![Juicy Preview](https://raw.githubusercontent.com/gimu/dotfiles/master/preview.jpg)


## Installation
Full installation with backup and packages (Arch Linux):

```
$ ./setup.sh
```

### Requirements
[Stow](https://www.gnu.org/software/stow/manual/stow.html) should be available via your package manager.

- `$ sudo pacman -S stow`
- `$ sudo apt-get install stow`
- `$ yum install stow`

Optionally clone it [from source](https://savannah.gnu.org/git/?group=stow) and [build it](http://git.savannah.gnu.org/cgit/stow.git/tree/INSTALL).

### Usage
Stow will create symlinks for files in the parent directory from where you executed the command. Therefore, the cloned repository should be placed in your home directory `~/dotfiles`, you will otherwise have to use the `-d` flag with the repository location.

#### Examples (executed in ~/dotfiles)
Installing emacs configurations: `$ stow emacs`.                     
Uninstalling emacs configurations: `$ stow -D emacs`.

#### Other directories
Use `$ stow -t destination_folder` to symlink configurations that are not stored in the home folder.

## Requirements
This setup uses [i3-gaps](https://github.com/Airblader/i3) and [polybar](https://github.com/jaagr/polybar).
