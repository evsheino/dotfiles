My dotfiles. Based on https://github.com/sontek/dotfiles/tree/vim .

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

### Only install and build vim files
Because this bit is pretty portable

    ./install.sh vim

### Restore old source Files
To replace installed files with the originals:

    ./install.sh restore

Note that if there was not an original version, the installed links will not be removed.

### Updating the vim packages

See http://stackoverflow.com/questions/1030169/easy-way-pull-latest-of-all-submodules

## Requirements
### Shell
* bash

### Vim
* python
  * flake8
  * rope
* ag (https://github.com/ggreer/the_silver_searcher)
* powerline fonts (https://github.com/powerline/fonts)
