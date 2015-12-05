My dotfiles. Based on https://github.com/sontek/dotfiles/tree/vim .

## Files
_vim
    my vim dir
_vimrc
    my vim configuration

## Instructions
Install script by sontek.

### Creating source files
Any file which matches the shell glob `_*` will be linked into `$HOME` as a symlink with the first `_`  replaced with a `.`

For example:

    _bashrc

becomes

    ${HOME}/.bashrc

### Installing source files
It's as simple as running:

    ./install.sh

From this top-level directory.

### Only install and build vim Files
Because this bit is pretty portable

    ./install.sh vim

### Restore old source Files
To replace installed files with the originals:

    ./install.sh restore

Note that if there was not an original version, the installed links will not be removed.

## Requirements
### Shell
* bash

### Vim
* python
  * pep8
  * pyflakes
  * rope
* ag (https://github.com/ggreer/the_silver_searcher)
* powerline fonts (https://github.com/powerline/fonts)
