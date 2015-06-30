vim-python-ide
==============

Personal Vim configuration files for developing Python projects on OS X and Linux

## How to install

Clone the repo to your local disk first:

```bash
git clone https://github.com/messense/vim-python-ide.git ~/.vim-python-ide
```

Init vim bundle and powerlines Git Repo
```bash
git clone https://github.com/gmarik/Vundle.vim.git ~/.vim/bundle/Vundle.vim
git clone https://github.com/powerline/powerline.git ~/.vim/bundle/powerline
```

Init submodules
```bash
cd ~/.vim-python-ide
git submodule update --init --recursive
# build vimproc
cd .vim/bundle/vimproc.vim && make
```

Softlink `.vim` and `.vimrc` to your HOME directory:

```bash
ln -s ~/.vim-python-ide/.vim ~/.vim
ln -s ~/.vim-python-ide/.vimrc ~/.vimrc
```

You should install fonts to make powerline complete work, please check https://github.com/powerline/fonts:

```bash
;this is just an example

git clone https://github.com/powerline/fonts
cd fonts
./install

```


You may need to install some Python package to make all this work:

    [sudo] pip install -U jedi flake8 pyflakes

## Bonus - screenrc

There is also a screen configuration file `.screenrc` in this project. Using it by:

```bash
ln -s ~/.vim-python-ide/.screenrc ~/.screenrc
```

### Key mappings:

* shortcut prefix: C-\
* F2 new screen
* F3 previous screen
* F4 next screen
* F6 detach screen
* F8 rename screen
