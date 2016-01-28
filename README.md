# vimrc



## for neo-vim

```
cd ~/workspace
git clone git@github.com:moskito518/vimrc.git
cd ~/.config
curl -fLo ~/.config/nvim/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
cd nvim
ln -s ~/workspace/vimrc/cache_dir cache_dir
ln -s ~/workspace/vimrc/colors colors
ln -s ~/workspace/vimrc/init.vim init.vim
ln -s ~/workspace/vimrc/ycm_extra_conf.py ycm_extra_conf.py
mkdir .backup
mkdir .swp
nvim
:PlugInstall
cd ~/.config/nvim/plugged
cd YouCompleteMe && ./install.py --clang-completer --tern-completer
cd ../tern_for_vim && npm install
ln -s ~/workspace/vimrc/.tern-config ~/.tern-config

```

## for Vim/Gvim/MacVim

```
cd ~/
ln -s ~/.config/nvim ~/.vim
ln -s ~/.config/nvim/init.vim ~/.vimrc

```
